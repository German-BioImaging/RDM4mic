Shared resources of RDM4mic group.

## Describe your local OMERO installation
[Template](SystemDescription_OMERO.pptx)

  To get the requested information from your OMERO system, you can use the following omero hql command to query the OMERO database(https://docs.openmicroscopy.org/omero/5.6.0/developers/GettingStarted.html#omero-hql), running with an OMERO administrator account:
  
**Number of users:**  

```>>omero hql -q --all "select count(e) from Experimenter e"```

**Activated user (ignore deactivated user accounts):**

```>>omero hql -q "select count(DISTINCT e.omeName) from Experimenter e join e.groupExperimenterMap m join m.parent as g where g.name = 'user'"```

**Daily active (in this example: on 21.09.2021):** 

```>>omero hql --all "select count(DISTINCT e.experimenter.omeName) from Event e where e.time > cast('2021-09-21 00:00', timestamp) and e.time < cast('2021-09-22 00:00',timestamp) "```

**Active (in this example: logged in user of last half year):**

```>>omero hql --all "select count(DISTINCT e.experimenter.omeName) from Event e where e.time > cast('2021-06-08 00:00', timestamp) and e.time < cast('2021-12-08 00:00',timestamp) "```

**Monthly increase storage (in this example:  total size of the images uploaded in September in byte ):**

```>>omero hql --all “select SUM(o.size) from OriginalFile o, FilesetEntry f, Fileset i, Event e WHERE o.id=f.originalFile AND f.fileset=i.id AND i.details.creationEvent.id=e.id AND e.time < cast('2021-10-01 00:00',timestamp) AND e.time >= cast('2021-09-01 00:00',timestamp)  AND i.id in (select fileset from Image)"```
