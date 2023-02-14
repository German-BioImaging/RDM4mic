###### tags: `meeting notes` `TODO?`
# Meeting notes RDM4mic 16.05.2022 and 17.05.2022

## Introduction Session
* Christian Schmidt: DKFZ HD, NFDI4BI coordinator, project office I3D:bio
* Thomas Zobel: RDM4Mic Co-Chair, WWU Münster Imaging Network. OMERO Instance since 2018 (in Münster) Co-Applicant in the NFDI4BIOIMAGE Initiative, Task Area 5, Thomas.Zobel@wwu.de
* Carsten Fortmann Grote: MPI Plön, OMERO instance running. Many other RDM tools in place
* Jens Wendt: WWU Münster (with Thomas), resp. for OMERO, image analysis, software related things
* Sarah Weischer: Post-doc Münster Imaging Network. Image Analysis
* Tom Boissonnet: HHU, I3D:bio, with Stefanie Weidtkamp-Peters
* Moritz Hoevels, UzK, Computing Center, concerned with RDM, CECAD, working with Astrid Schauss and Peter Zentis
* Wiebke Möbius: MPI Multidisc. Sciences, Göttingen, Head of EM Facility. Interested in RDM and OMERO
* Michele Bortolomeazzi: DKFZ HD, OMERO administrator. michele.bortolomeazzi@dkfz-heidelberg.de
* Silke Tulok: Light and EM Facility, Med Fac Dresden. Currently setting up OMERO
* Johannes Koch: Uni DUE, learned a lot about OMERO, we use it now for the CRC
* Johannes Balkenhol: Würzburg, Bioinformatics and Imaging Facility, with Katrin Heinze. Uni Würzburg wants to have improved RDM until 2024.
* Thomas Müller-Reichert: TU Dresden Medical School. Currently setting up OMERO
* Luiz Gadelha: Balance of the Microverse Excellence Cluster, OMERO is installed
* Julia Dohle: CellNanOS Osnabrück, working with Susanne Kunis, I3D:bio
* Janina Hanne: German BioImaging, managing director
* Olaf Selchow: Freelancer, Image Data Management, Microscopy Workflows
* Angela Naumann: LIC Freiburg with R. Nitschke
* Arne Fallisch: LIC Freiburg with R. Nitschke, in the phase of setting up OMERO for the QUAREP community, also managing the institution webservers. Nextcloud with LDAO connection etc. for QUAREP already set up
* Lukas Hellmann: Uni Mainz, in the process of setting up OMERO, interested in connected OMERO with iRODS for archiving
* Alfonso Schiavi, Düsseldorf,
* Niraj Kandpal: CECAD, UzK, with Peter Zentis and A. Schauss, worked with OMERO and metadata
* Roland Nitschke: Head, LIC Freiburg, coordinating several OMERO installations at Freiburg, CIBBS, Med Faculty, Metrology Database for I3D:bio
* Marcel Kirchner: MPI for Ageing, Cologne, currently setting up OMERO
* Göktug Islamoglu: CIBBS Freiburg, developing a web interface to handle zar file formats for OMERO. User friendly back-up storage for zar.file formats
* Tobias Wernet: LIC Freiburg, I3D:bio team, setting up different OMERO instances
* Peter Zentis: CECAD imaging facility, Cologne.
* Ralph Palmisano: Head of Optical Imaging center in Erlangen. OMERO running since 11 years. Was one of the first OMERO users, when Jason Swedlow started it
* Inga Patarcic: MDC Berlin, RDM manager, OMERO is in test phase. On-premise version in due time planned, inga.patarcic@mdc-berlin.de
* Josh Moore: OME Team & GerBI. Original OMERO designer, still running the developers team. On the NFDI4BI grant and supporting I3D:bio
* Fabian Reinisch: Goethe Uni Frankfurt, wants to learn about RDM and OMERO use in particular. Professionalize RDM.
* Timo Lin: Uni Mainz, IT for Biology, want to set up OMERO instance
* Martin Hohmuth: Uni Jena, ExC Balance of the Microverse. OMERO is running. Also working on another platform
* Hella Hartmann (hella.hartmann(at)tu-dresden.de): Light Microscopy Facility at CMCB, TU Dresden. Watching OMERO developing for some time. Plan to have OMERO installed, too
* Monica Valencia-Schneider, UzK, Computing Center


## To do:

#### Please provide the RDM4mic with the timeline for your omero installations
#### Please provide the RDM4mic with the amount of storage needed for your installation over time
#### Please provide additions or examples for the OME deployment examples (https://github.com/ome/omero-deployment-examples)



## Newbies Session "Overwhelmed by...
* Impulse Talk Christian Schmidt & Jens Wendt

#### Comments & Questions:
*    RN: need to increase acceptance in broad community, include RDM in curriculum for students
*    WM: professional RDM: RDM staff needed, how to convince management that this is necessary? 
    * TZ: manadatory to give plan for RDM in CRC grant applications
    * CS: DFG funding programs for RDM:
https://www.dfg.de/en/research_funding/programmes/infrastructure/lis/funding_opportunities/research_data/index.html
https://www.dfg.de/en/research_funding/programmes/infrastructure/lis/funding_opportunities/vigo/index.html

* JK: Team up with IT people if you are not familiar with it. Both sides are important to bring together
* JK: Change management: start with students, e.g. during microscope introductions, courses etc
* TZ: try to bring together different RDM people from the university
* JM: you will probably need someone that takes care of your omero instances
    include RDM in your grants, funding opportunities (see above)
    sharing omero instances with different institutions to reduce maintenance     load, data transfer problems
    outsourcing, having someone to come in from the outside 
    

* RN: improve interfacing of OMERO
    * TZ: mention to microscopy companies that they should include an interface to omero for easier upload directly from microscope PC
    * JM: It's tricky. I agree completely that the integration into commercial software would help, but I don't think the right motivation(s) for that exist.
    * OS: Did (some?) companies express their requirements that they would need from OMERO, in order to facilitate interfacing? I'm sure there are reasons they develop "own" solutions, as Thomas mentioned. And not only that they ignore the advantages of interfacing...
    * JM: no, I don't know of any discussions, other than PE's full integration.


* JB: new file formats, integration of -omics data?
    * JM: what type of integration would be useful? E.g. link to omics database, possible to add the links in a tabular fashion --> scripts available (TZ) : https://www.youtube.com/watch?v=NO8Me5LgxrM&list=PL-oOCWFUMH50Huf6SzsGQRgLsM1SJfZe3&index=5&t=6s <br>
    https://github.com/ome/omero-scripts/tree/develop/omero/annotation_scripts

* ST: How much storage necessary on omero system? What should be used as an estimate when setting up new instance?
    * TZ: best would be: flexible, easy expansion possible
    * OS: scalable solution is important
    * TZ: example installations (hardware config) on the ome site: 
    * JM: dependent on how many + which microscopes, which type of data, how many users
    * TZ: collection available of experiences from different institutes with omero instance

* RN: linking omero with other resources, e.g. Galaxy? Experiences, will that increase acceptance of omero?
    * JW: For data analysis: important to have good interfaces with image analysis programs!
    * TZ: important to provide means of analysis without download or copying data, as facility: provide these solutions for users, also to increase acceptance

* RN: User management: often LDAP is used, preference to have something more universal to facilitate access of international collaborators, e.g. eduroam, shivole?, orchid
    * JM: using orchid, github etc would be fairly straight forward, to do it properly would be huge project, Glencoe has a plugin that they use for website, people can login with more general mechanisms (e.g., orchid)
    * CS: recent use-case: Heidelberg scientist working in Freiburg, would like to have Freiburg collaborators login to their instance to upload data. Currently, need VPN connection/Heidelberg credentials. What are currently the solutions for this?
        * PZ: Apply for guest accounts at university to gain access, some administrative effort, often time-restricted
        * OS: Unfortunately many Universities and Resaerch institutes are pretty strict in not allowing guest accounts. I've been through this discussion a couple of times now.

        * JW: What about temporary OMERO accounts?, e.g. possible solution: maybe a "temporary" account for external users, to upload into a specific group only for upload. Then move the data in OMERO into the right group and change the owner. Change the password of the temporary account after the upload happened

            * JM: A downside of "temporary" OMERO accounts is that they can't yet be easily deleted. (See recent image.sc thread with Damir)

    * Data repositories after publication. Omero/Access from outside to view published data would prevent data duplication.
        * TZ: public group for published data, implemented for one journal in Münster (link)
        * TZ: OpenLink, creation of public links, can be downloaded without account https://github.com/sukunis/OMERO.openlink

        * TZ: together with university library: DOIs on images. Provide DOIs to journals for direct access to images from publications

* RN: data protection and safety: guest accounts might be problematic when storing personal data(?), less of a problem for orchid (?)
    * JM: Omero only needs e-mail address and name


## New deployment of OMERO 
* **Impulse Talk by S. Tulok:** Perspective from a light microscopist, limited to no IT or computer-science experience
* Research Campus in Dresden: Biopolis Dresden Imaging Platform, a lokal, multiinstituional platform for imaging (light and electron). TU Dresden + MPI-CBG + DZNE (Helmholtz) + Uni Clinics --> a lot of data transfering required for the users
* BioDIP community hence is very interested in a common infrastructure framework for bioimaging.
* CFCI (Silke) belongs to the Faculty of Medicine of the TU Dresden (has a reserach part & a facility part)
    * facility: 100 active users, 35 RGs
    * management currently: via internal NAS or via TUD server
    * RG (T. Müller-Reichert): Study mitosis, meiosis, etc. Use a lot of microscopy techniques, acquiring large datasets
    * 3 - 4 international collaboration partners. Data sharing for this exchange is difficult right now
* Want to use OMERO with the new slide scanner that was approved in Nov. 2021
    * Problem: TUD very slow at uni-wide implementation
    * Hence: Only OMERO for Faculty of Medicine
* Med Fac IT appreciated OMERO as a good use case
* Organizing hardware and storage for the system was not easy.
    * IT wants to have a clear amount of data to plan for

**Impulse Talk by M. Bortolomeazzi:**
* Installation: openstack --> ubuntu docker image including omero.web, and server (NFS storage), LDAP for user management
* Setting up an installation with docker was quick and easy. There are great examples from OME at: https://github.com/ome/omero-deployment-examples
* Only a few things are more difficult compared to the "standard installation":
    * Configuration changes (plugins, performances): create custom dockerfile from the examples from OME
    * System Administration (backup, log rotation): needs interfaces with docker service. We started from the documentation for the "standard" installation and adapted the examples/recommendations to a docker-based setup.
    * Setting up automatic import, from outside the local filesystem
        * Omero "dropbox" would be nice (not possible with our storage configuration)
        * Currently: cron job with custom script to check if there are new images

* Server up and running, not yet open to users
* Small test cohort to test potential issues, scalibility etc. Recruited in collaboration with our Light Microscopy Facility. Christian and I presented OMERO to the users and discussed their image data management needs after they had an introduction to the slidescanner.
* automatic import from different systems:
    * Axioscan slide scanner: import w/o keeping controller computer busy
    * Resolve: spatial transcriptomics: integration of metadata, inclusion of  transcript counts?
* Facility: 600 users


### Discussion:
* RN: When asking for numbers, e.g. what amount of imaging data is acquired, often a underestimation is given. How to get correct numbers?
* TZ: RDM4mic would like to collect data from different omero installations
* CFG: Working on automatic upload as well; currently working on it for CT scanner data, metadata in big yaml/json file; easy parsing and upload metadata as key-value pairs, small GUI written 
    * MB: cron job to check whether new data has been added every hour, folder structure is similar, so far just copying data to server(?); future: inplace import
    * CFG: How about metadata? 
    * MB: So far only from folder structure. In discussion with company to provide configurations together with the tiff images. Metadata from config file not yet implemented


## Update I3D:bio, E. May

https://gerbi-gmb.de/i3dbio/

(talk recorded)
* I3D:bio, now funded by DFG (lis: library and information systems)
* RDM4mic/Omero: community initiative, exchange of expertise, mutual support
--> no funding
* I3D:bio: acquire funding dedicated to bioimaging RDM; focus on omero-based image datamanagement
* omero: most widely used,according to NFDI4BIOIMAGE community survey
* Co-applicants: S. Weidtkamp-Peters, S. Kunis, K. Bernhardt, R. Nitschke, E. Ferrando-May, GerBi
* LIS program at DFG: https://www.dfg.de/foerderung/programme/infrastruktur/lis/lis_foerderangebote/forschungsdaten/index.html
* Imnplementation:
    * facilitate management and sharing of imaging data, including image metadata
    * Metadata annotation big bottle-neck for Image Data Workflow --> OMERO as a possible solution
    * open repositories for publishing, e.g. BIA (BioImage Archive), IDR
    * Analysis&processing on (cloud)clusters, utilizing tools like Galaxy
    * Image reuse, data mining of repositories
* Division of I3D:bio in 3 Workpackages:
    * Deployment, main aim: have someone to help you with omero installation
    * Technical Infrastructure, main aim: storage concepts, tools, integration of metadata
    * Communication & Training (Coordination, Networking, Training/Meetings, Evaluation)



## Update NFDI, E. May

* enable data management according to FAIR principles
* 70 mio / year, for up to 30 consortia of all scientific fields
* science-drive, collaboration accros all NFDI consortia (no competition), connect internationally (integration), invest in people (cultural change)
* NFDI only nation-wide group so far
* Bioimage participated in 3rd call (2021), to be prepared; (in the meantime: I3D:bio)
* 15 proposals in review phase now
* March 2022: panel review: online discussion session (WP, More, Mallm, Kreshuk, May); received comments, answers to reviewers' comments submitted; waiting for recommendation of expert committee (expected soon, June 13th)
* final decision: GWK (Gemeinsame Wissenschaftskonferenz, political organ, research ministries of states, federal ministry), expected Nov 2022
* If funded: start Jan 2023
* Data stewards to help new institutions to implement the infrastructure and software and to offer initial training ; research software eng. for actual development in close coordination with the community
* Division in 4 Workpackages: 
    * Standardization of bioimage data type
    * Scalable infrastructure for FAIR image data
    * Maximize reach of reproducible image analysis workflows in community, incl. AI-based image analysis methods
    * Capacitate researches for FAIR image datamanagement
* 6 Task areas:
    * Image (meta)data formats and standardization (Weidtkamp-Peters, Kunis, Moore)
    * Tech infrastructure and cloud ressources (Blank-Burian, Grüning)
    * Mulimodal data linking and integration (Mallm, Zuschratter)
    * Bioimage informatics and analysis (Figge, Kreshuk)
    * Training and community integration (Haase, Zobel)
    * Coordination, governance and networking (Weidtkamp-Peters, May)

Contact: Christian Schmidt (nfdi4bioimage@uni-konstanz.de)

#### Questions:
* JW: BioImageArchive, plans for DOI?
    * CS: Upload to BioImageArchive not yet easy, submission: https://www.ebi.ac.uk/bioimage-archive/submit/
DOI workflow planned





## NFDI4BI survey presentation (J. Hanne)
* community effort to address the state-of-the-art in bioimaging RDM
* questionnaire was drafted by the NFDI4BI initiative, conducted as online survey in 
* link to the survey paper publication (added after the meeting): https://doi.org/10.12688/f1000research.121714.1


## Training material hub (CC-BY)
* session on sharing training material
* ideas on what makes a good training material ressource
* creation of collection of lecture slides/material
* change management, how to stimulate users to use omero?
* Who is giving lectures to students? Tom B. (FiJi, useful examples are needed to convince students, basic course already prepared), Thomas Z. (working with students and OMERO to get them used to it), Marcel K. (courses to master students for FiJi using data located in OMERO, OMERO figures), Peter Z. (slides for new OMERO users with the most important steps available, needed is an institute specific version, slides belong to Niraj K.), Niraj K. (Basic OMERO introduction already used and available (very detailed), meant to support the personal introduction), Angela N. (centrally organized collection wanted, maybe at GerBI)
* Video or written tutorial? Tobias W., Fabian R. and Peter Z. prefer written tutorials, but short videos could support.
* Instructions for PIs available? Tom B. smaller videos to address different backgrounds? 
* Thomas Z. make a list of all different kinds of tutorials, videos and scripts and collect the links to these resources at one place, please add the tag "omero-training" to your training material on GitHub (https://github.com/topics/omero-training)
* Carsten F.-G. Is this [workgroup for training material collection] already established? A: No, this what we want to do, Q: OMERO page is the first address to get informations about OMERO, would people search for other tutorials? 
* Peter Z. script available which prepares example taining data in OMERO for people participating in a course? Josh M. Petr W. has some scripts for this, but have to be adapted. (https://github.com/ome/training-scripts/blob/master/maintenance/preparation/import-workshop-data-prep.md)
* JH: happy to support the collection on the GerBI webpage (https://gerbi-gmb.de/resources/teaching-modules/), for adding teaching modules to the GerBi collection, contact Silke Tulok.

### People who would like to contribute in workgroup "Training Material Collection" please let Christian @ christian01.schmidt@dkfz-heidelberg.de know!


## ELN, storage concepts -- collecting feedback & questionnaire session
S. Kunis, J. Dohle

Electronic Lab Notebooks:
- develop tools for the integration of metadata from OMERO into ELNS.
Please fill in the survey:
ELN Form: https://gerbi-gmb.de/machform/view.php?id=40086

Storage concepts:
- identification of bottlenecks in the workflow of moving and storing data at your institution
Please fill in the survey:
Data Flow: https://gerbi-gmb.de/machform/view.php?id=39255


## Links
* Agenda: https://github.com/German-BioImaging/RDM4mic/blob/master/meetings/2022-05/2022-05_agenda.md
* Q&A: https://hackmd.io/Xyzp6oS9RMKXsW6TMRSIbw
* German BioImaging (GerBI): https://gerbi-gmb.de 
* RDM: https://rdmkit.elixir-europe.org/
    * https://www.forschungsdaten.info/ (only in German)
    * https://www.youtube.com/c/EuroBioImagingCommunication
    * https://rdmkit.elixir-europe.org/bioimaging_data
    
* OME: https://www.youtube.com/c/OpenMicroscopyEnvironment
    * Bulk Annotation Workflow With Omero Forms: https://www.youtube.com/watch?v=NO8Me5LgxrM&list=PL-oOCWFUMH50Huf6SzsGQRgLsM1SJfZe3&index=5&t=6s
    * Script to annotate whole projects with key-value pairs in one go using csv files: https://github.com/ome/omero-scripts/tree/develop/omero/annotation_scripts
    * OMERO Metadata Editor: https://omero-guides.readthedocs.io/en/latest/mde/docs/index.html / 
    * OMERO training on Github: https://github.com/topics/omero-training

* BioImageArchive: https://www.ebi.ac.uk/bioimage-archive/submit/
* Image Data Resource: https://idr.openmicroscopy.org/



# Day 2
## Wrap up of WG I

* J. Koch: Experienced User Training: 
    * Fiji connection, Fiji Plugin, Batch Analysis, 
    * QuPath, etc.
    * OMERO.figure
    * Image Rendering / How to apply to all
    * Key-value pairs and metadata annotation and why it matters
    * pyramidal data (e.g., IMARIS format), display in OMERO, how to handle the pyramid
    * more general: import behaviour of different file formats
* Johannes might offer a data set for training.
* Thomas has data from screens for training with OMERO.parade
* Tip: New duplicate function, that does not really copy the data, but assigns it to different groups (Script by Anna Hamacher)
    * ! This depends on the OMERO.server version

## Discussion about Work Group Session in RDM4mic
* difficult online
* What is the opinion on the work groups? Rather open discussion sessions?

## Open Discussion:
* S.Ritz: It would be great to have someone review the hardware, we plan to buy for our OMERO instance
* J. Hanne: Idea: Have an RDM class where people from the community can join. The format is open to discussion. Could include exercises, etc.
    * well received idea by the participants

## Session FAQ collection
* Intro to the tasks by Susanne

* FAQ collection contains naive questions from users which came up during training them, as well as other frequent questions. They answer who can I ask this question or is there a general answer.
* Group the FAQ: Sort by user categories (users, IT-team, RDM-team)? Design (technically) as drop-down menu or as a tree?
* Mark questions which are frequently asked
* Where will the FAQ be published? Publish user questions on image.sc and bundle the rest to send per mail? Will be tagged with 'omero'. Put on I3D:bio website?
* Set up as a Wiki? Who edits? Is it then findable? Advante of image.sc: mark solutions, people easily contribute, are looking there for answers
Link to the table: https://docs.google.com/spreadsheets/d/1m4xtucM0XjBtfQZhiJsqFtST-J64DYC_aSMZqzhPGTA/edit#gid=0



### Discussion:

* JM: Do we need to identify what are the searching habits to find these FAQ per different user group
* CFG: Google is very important. I often end up on stackoverflow

* OS: Suggestion: Prepare a checklist for people (microscopists) with questions to answer for themselves before going to the IT-department, e.g. should the server be reachable from the outside?
* Also guidelines on "how" to talk to the IT.
* Extensions (in the spreadsheet) are welcome

* TZ: Are use-case reports useful as entry point for setting up new servers?
    * well received, considered useful 
    * OS: offers to make a collection of ca 5 different installations
    * TZ: add-in the MIN installation set-up
    * SZ: collection of technical system set-ups could help, but should be made more accessible (less technical)
    * TZ: MiN usecase example can be found here: https://confluence.uni-muenster.de/display/WWUIMW/Research+Data+Management+for+Microscopy

* PZ: Collection of problems with specific microscopes and fileformats with omero --> reporting possibility (for positive and negative)
    * TZ/OS: Image.sc forum probably best place to ask/comment there
    * JM: OME Team has limits to answer all questions on image.sc e.g. 
    * Ppl who are fixing the bug, won't report back on the forum

* JM:   --> general discussion on curation needed, how can a large community can curate the FAQs, and keep data up to date
    * AR: Wiki-Format 
    * CS: Integration of image.sc and wiki image.sc. possible?
    * JM: Technically possible, but would have to be discussed with the bigger community
    * JM would offer code to extract posts from image.sc to be included in Wiki; would need additional metadata to fit the table (e.g. who can answer)
    * OS: don't overengineer it. Solid reference for the most commonly asked questions, and for installation-specific new questions will come up anyway. 

* JM: new release of OMERO, check "limitations" of previous releases, see if they have been solved, feedback to FAQ and image.sc


### FAQ maintenance team: 
I3D:bio
Olaf Selchow (in-between user and IT)
Thomas Zobel (facility)
Sarah Weischer (image analysis)
Monica Valencia-S (IT-site)


### Next Meeting:
* Format: preferred in-person, + hybrid option for presentations and talks
* Planned for September
* Who is hosting the meeting?
* Format: - open panel discussions, - split into smaller groups, including preparation of certain topics

* Potential Topics:
    * Teaching material collection
        * Basic trainig
        * advanced training
    * FAQ team
    * Use-case collection
    * Results of the ELN and Data questionaire
* PZ: how Omero integrates in RDM plans (grant applications), discussion-like, sharing experiences
* MVS: data policies in omero, templates for facilities
* MVS: costs, what kind of costs could be attached to setting up omero, how much can I add to my proposal? 
    * SK: What happens after funding period to sustain the installation?
* SK: open discussion Newbie session.
* calculation examples for storage space & costs


## Links Day 2
* Video OMERO.figure https://www.youtube.com/watch?v=Jv9f55Mbmhg
* FAQ collection: https://docs.google.com/spreadsheets/d/1m4xtucM0XjBtfQZhiJsqFtST-J64DYC_aSMZqzhPGTA/edit#gid=0

# Wishlist
* JK: Dataset and Tutorial for advanced users. Data in OMERO --> Fiji Analysis --> Automated Upload --> Populate Result Table (parade) --> Browse Data with parade 
* SR: Tutorial for different functions (figure / Aplly to all) --> Small Videos
* Fileformat behavior (single Images of different resolution, possible to delete some?)
* Data management workshop
* AN: If GERBI has trainer for such a series of an online Data Management workshop and an installation the participants can work with, that would be great idea...also to create training videos :-)
* Check list / Questions you should think about first, before you go to your it department
* More use cases / references / example installations.

# Next meeting talks:
* RDM Plans / Guidlelines used in CRCs / Theroy & practice
