Meeting Minutes 15.12.2021
===

###### tags: `RDM4mic` `Meeting` `Minutes`

:::info
- **Location:** Virtual
- **Date:** Dec 15, 2021 
- **Program:** [6. RDM4mic meeting](https://github.com/German-BioImaging/RDM4mic/blob/master/meetings/2021-12/2021-12_agenda.md)
- **Host:** Thomas Zobel 
- **Organisation:** Susanne Kunis, Thomas Zobel, Stefanie Weidtkamp-Peters
- **Minutes:** Josh Moore, Susanne Kunis, Thomas Zobel, Sarah Weischer, Jens Wendt
- **Agenda:**
    1. Official Welcome `30min` [name=Susanne Kunis,Thomas Zobel]
        - Short Introduction participants
    2. Update Status facility RDM solutions `120min` [name=Susanne Kunis,Thomas Zobel, Anna Hamacher]
    3. NFDI4BIOIMAGE `30min` [name=Stefanie Weidtkamp-Peters]
    4. Feedback & QA NFDI `60min` 
    5. Organisational `30min`
    6. For newbies`90min` 




:::
## Attendees 

Format:
*Name (Affiliation, existing OMERO installation at institution, optional->name on github/image.sc, etc.)*
* Susanne Kunis (CellNanOs Uni Osnabrueck , yes, @sukunis)
* Stefanie Weidtkamp-Peters(Cai, yes, twitter @SteffiWeidtkamp, @CAi_HHU)
* Rainer Kurre (iBiOs UOS, yes,)
* Thomas Zobel (WWU Münster Imaging Network, yes, twitter @Th_Zobel, image.sc @T-Zobel, GitHub MuensterImagingNetwork) 
* Peter Hemmerich(FLI Jena, no)
* Anna Hamacher(CAI, yes, image.sc @ahamacher)
* Karen Bernhardt (UOS, yes)
* Stefan Fischer(TSM Tübingen, yes (@QBiC), twitter @steveHRO image.sc @s.fischer ) EM
* Arne Fallisch (Miap Freiburg, yes) QUAREP-Limi
* Monica Valencia-Schneider (RZ Cologne, yes)
* Peter Zentis (Cecad Cologne, yes)
* [Josh Moore](https://twitter.com/notjustmoore) (OME/GerBI, yes [IDR, Dundee])
* Johannes Koch (Duisburg/Essen, yes) LM
* Angela Naumann (Miap Freiburg, yes--lessed used)
* Roland Nitschke (Miap Freiburg,yes)
* Gebhard Stopper (CIPMM Uni Saarland, yes)
* Sandra Ritz (Mainz, yes--lessed used)
* Sabine Haxelmans (Freiburg, yes)
* Felix Bestvater (DKFZ LMF,yes -- starting)
* Ioannis Alexopoulos (Giessen IHL, yes [@iAlexopou](https://twitter.com/iAlexopou) [@CIGL_IU](https://twitter.com/CIGL_IU) )
* Kathrin Lehmann (Duisburg/Essen/UDE,yes)
* Niraj Kandpal(Cecad Cologne, yes)
* Hanka Medova (DKFZ LMF, yes --starting)
* Carsten Fortmann-Grote (MPIEvol Plön, yes)
* Martin Hohmuth (Uni Jena, yes --starting)
* Katherina Hemmen (Würzburg RVZ, no)
* Sarah Weischer (MiN Münster, twitter: @sarah_weischer)
* [Jens Wendt](https://github.com/JensWendt), [twitter](https://twitter.com/jens_wendt) (MiN Münster)
* Jordi Pujol (DKFZ, yes - starting)
* Katharina Nöh (Forschungszentrum Jülich)
* Janina Hanne (German BioImaging)
* Christian Schmidt (NFDI4BIOIMAGE)
* Luiu Gadelha ( Cluster of Excellence Balance of the Microverse Jena, yes)
* Phillip Mallm (DKFZ)
* Sascha Genehr (Uni Rostock)
* Göktug Islamogly (Istanbul Technical University)

## Welcome
- Introduction round of the participants, and a short welcome from Thomas Zobel

## Update Status facility RDM solutions 
### CellNanOs Susanne Kunis:
* Overview about Support point / OMERO Community Meetings
    * Forum/Help:
        * [https://forum.image.sc/tag/omero
](https://forum.image.sc/tag/omero
) 
        * [https://omero-guides.readthedocs.io/en/latest/
](https://omero-guides.readthedocs.io/en/latest/
)
    * Focus meetings:
        * OMERO admin international: https://forum.image.sc/t/omero-for-admins-meeting-dec-7-2021/59236/5
        * OME: https://www.openmicroscopy.org/events/
        * IRODS and OMERO: https://github.com/irods-contrib/irods_working_group_imaging
        * QUAREP-LiMi (metadata): https://quarep.org/working-groups/wg-7-metadata/
        * NGFF:  https://forum.image.sc/t/next-call-on-next-gen-bioimaging-data-tools-2022-01-27/60885
* Overview about CellNanOs OMERO installation
* Usage of OpenLink
* Other extensions can be found via [GitHub topics](https://github.com/search?q=omero&type=topics)
* OpenLink spaces are cleaned up automatically after 30 days
* Questions:
  - file attachments? adaptation possible to include more than just FileAnnotations.
  - extra password protection?
  - High Content Screening (HCS)? Untested, also no support for in-place imported data 
  - 100 day inactivation as the best way to keep system clean? One possible way, yes.
  
### CAi Anna Hamacher
* Overview of plate data
* Using of OMERO.parade on plate data to explore related metadata
* extension OMERO.parade-crossfilter (prototype)
* bottleneck of importing many plates at the same time --> need to also optimize postgresql
* QA: manual workflow?
    * workflow with the help of [knime](https://www.knime.com/
)
* [adaptions of OMERO system for many concurrent users](https://forum.image.sc/t/error-504-when-many-users-log-in-to-omero-web-simultaneously/45084)

### MiN Thomas Zobel
* Overview about MiN OMERO installation
* Another potential template would be DOI conversation for libraries
* Adaptation of Dataset-to-Plate OMERO server-side script for Olympus ScanR screen data
* Implementation of OMERO plugin for Fiji, with a generic Jython script to download, process and then upload images in Fiji from/to OMERO
* OMERO <-> DeepLearning Noise2Void via Python with user friendly GUI

## NFDI4BIOIMAGE 
* I3D:bio: Bioimage data management, OMERO-centric, starts Jan 2022
* NFDI: RDM, FAIR image data (under review, start Jan 2023)
* Survey 2021 in bioimaging community: only 25% use OMERO, most no image data management system. Discussion on challenges and needs in RDM for image data. 
* [NFDI4Bioimaging website](https://nfdi4bioimage.de/en/start/)

## Feedback
* FB: Analysis workflows with Imagej, Cellprofiler, etc. -->
    * Different possibilities for integration of ImageJ with OMERO: 
        * OMERO plugin in Fiji, 
        * `ezomero` python package, 
        * putting ImageJ libraries on the OMERO server and run as headless
    * Cellprofiler will only connect via the Python API
    * For commercial software: Huygens/VisiView provides OMERO access, Imaris/Arivis not
* CS: Datastewardship concept as service to answer these kinds of questions (included in NFDI application)
* KB: Stronger voice of the community for common file formats needed towards the companies
* RB/CS/SWP: Common file formats not so much handy for vendors, no incentive/advantage **yet**
* HM: Medical data in OMERO, problem of security issue
    * workflows could be build, but pay attention on special regulation in terms of medical data
    * More a topic for NFDI4Health, NFDI4Bioimage in contact with them, but no focus for NFDI4Bioimage
* FB: Data ownership when leaving institution --> data will remain on server independent of user status, ownership can be transferred (but is to be avoided (SK))
* RN: (general) Data ownership by students that do not have a official contract. Who owns the data? Implications for NFDI4Bioimage: big initiatives necessary to tackle these general problems. Maybe even political guidelines/laws needed to provide solid legal basis. 
* SR: Solutions for analysis on dedicated server. -->
    * Münster solution: HIVE as explained in presentation; initial upload to (OMERO) server, then analysis on the dedicated server which has very fast connection to the data/OMERO server; analysis server gets accessed remotely from the individual workstation; 
* FB: How to set up upload workflow?:
Depends on infrastructure
    * OMERO.insight
    * Watchfolders
    * Autoimport (e.g. [Smuggler](http://c0c0n3.github.io/ome-smuggler/docs/content/index.html))
    * Remote import (via OMERO.web)->Remote import via mounting a folder and CLI-import
    * [Import Solutions on GitHub](https://github.com/topics/omero-import)
* RN: Documention of image analysis pipelines/workflows.
    * SWP: Focus on open-source tools in the first step, e.g. Fiji time machine (Robert Haase), 
    * impact on commercial applications?
    * JM: First start with open source tools to show/create advantages which then act as incentives for additional users and integration into commercial applications 
* TZ: **Please send in your problems, so that they can be used as Use-cases for the NFDI**


## Organisational
* Github/Licensing of shared material:
    * Creative Commons License CC0
    * Possible to upload material with a different specific license, should be marked then

## Help and Discussion
* FB: Report of remote importing issues in OMERO insight from shares in active directory
* IA: short showcase of individual upload pipeline and bottlenecks --> SK: proposal to use CLI-importer to possibly circumvent bottlenecks
* SR: what happens with the raw data? Does OMERO keep the raw data? --> JM: From the OMERO site of view: Your raw data is kept. Be sure OMERO is backedup etc....
* FB: selling points for OMERO?
    * start using OMERO in student courses / as early as possible
    * Introduce OMERO during the introduction into mic systems
    * Be active in CRCs / Inf projects / provide Data management plans
    * OMERO.figure
    * virtual courses with OMERO
    * work on all levels
    * convince PIs
    * easy access
    * required for applying for microscopes
    * try to show groups advantages for their research
    * find PhD students with affinity to OMERO / scripting / etc. --> They might infect collegues :-)
* **Note**: Omero insight is deprecated ("in maintenance mode"). Just use for upload and some very specific functions. Working towards moving all functionalities to web browser.
* TZ: OMERO.insight offers functionality for browsing file attachments, OMERO.web does not yet.
* regarding the same issue: JM: Dealing with File attachments: Preferably just link your attachments as OMERO is not build to manage all kinds of data. There will be a need in the future as OMERO is slimmed down for other tools/addons to emerge to fill the gap of attachment handling.
* FB: Problem of who is responsible for maintenance and configuration of the OMERO server, local IT or Admin? --> maybe use `Ansible` to set up a configuration and let local IT implement it then.
* TZ: problems at generating pyramid files for certain EM and slidescanner data
    * preprocessing with [bioformats2raw](https://github.com/glencoesoftware/bioformats2raw) -> [raw2ometiff](https://github.com/glencoesoftware/raw2ometiff) and importing ome-tiff
    * `conda create -n fixme -c ome bioformats2raw raw2ometiff`
* In general preferable upload strategy: Get your file into an open file format
* RB: future of bioformats
    * JM: bioformats not fundable
    * Enabling hundreds of fileformats, make it easy for users and vendors to use them --> Community/vendors not inclined to standardize. 
    * Aim: No support for new formats. (Unless companies do it themselves.)
    * Goal: get your data out of proprietary file format into open format
    * Problem: How to migrate metadata without loss? Vendors must help.
    * GI: Experience from "construction field": agreement on [IFC file format](https://en.wikipedia.org/wiki/Industry_Foundation_Classes) during one big meeting, ISO standardized (https://www.buildingsmart.org/standards/bsi-standards/industry-foundation-classes/)
* TZ: Protocol for changing the number of possible concurrent users is in the [image.sc forum thread](https://forum.image.sc/t/error-504-when-many-users-log-in-to-omero-web-simultaneously/45084)
* Task for **I3D:bio** --> Version of OMERO with most-used plugins included (like Fiji is to ImageJ)


# Links
* https://omero-guides.readthedocs.io/projects/fiji/en/latest/installation.html?highlight=imagej
* https://github.com/imagej/imagej-omero
* Python package for easier handling of OMERO API: https://pypi.org/project/ezomero/
* Cellprofiler can be executed via Python API https://omero-guides.readthedocs.io/en/latest/cellprofiler/docs/gettingstarted.html
* QuPath work works with OMERO too!
https://omero-guides.readthedocs.io/en/latest/qupath/docs/qupath.html
* Other notebook/fiji fun: https://omero-guides.readthedocs.io/en/latest/fiji/docs/headless_notebook.html?highlight=imagej)
* Huygens integration for OMERO: https://downloads.openmicroscopy.org/presentations/2017/Users-Meeting/Lightning-Talks/Remko%20Dijkstra%20-%20Huygens%20and%20OMERO.pdf
* Napari plugin for OMERO connection: https://github.com/tlambert03/napari-omero 
* Import solutions: https://github.com/topics/omero-import  ;  http://c0c0n3.github.io/ome-smuggler/docs/content/index.html
* https://github.com/glencoesoftware/bioformats2raw
* https://github.com/glencoesoftware/raw2ometiff
File format:
    * https://en.wikipedia.org/wiki/Industry_Foundation_Classes 
    * https://www.baunetzwissen.de/bim/fachwissen/standardisierung/ifc-der-offene-standard-fuer-bim-modelle-5288161
    * https://www.buildingsmart.org/standards/bsi-standards/industry-foundation-classes/