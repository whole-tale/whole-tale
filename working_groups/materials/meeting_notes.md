2017-07-11 Meeting Agenda

Agenda
- MDF Brief Update (5 min)
- Early user solicitation
- WholeTale Demo (10 minutes)
- Feedback
- WholeTale Summer Intern Update: Jiming Chen, Logan Ward (12 min)
- Jennifer Use Case effort (WT Intern)
- Interest in defining an {ingester/processor} {API, framework} to generate metadata from files (Max Hutch) [5, 10] minutes
  - Can we develop a general framework for ingesting data of different types from various sources
  - Interest from MDF side here as they have developed a similar system
  - Citrine has a model for doing so too
  - Most efforts are somewhat manual and specific to an individual repo

https://opensource.ncsa.illinois.edu/confluence/display/CATS/Extractors


2017-03-06 Meeting Agenda

- New Members
- Brief overview of WT/MDF
- Citrine 
  - Host a large database and interested in analyzing these data
  - Using ML to analyze datasets
- Publication discussion (Kyle)
  - What types of data/analysis are related to publications
- What efforts already exist to support publication of data/methods
  - What are the issues with these approaches?
- What repositories or databases should we prioritize adding to MDF?
- Journal of chem
  - No question about data/process
  - Basically just if reviewer asks
  - No requirements or guidelines
  - Common across journals
- Nature publishing is starting to ask for data statements
  - Maybe email the authors
  - Mostly just start thinking about
- Some journals are starting to ask for things for specific data types (data is sufficiently common - maybe 10% of papers in the journal are about this and sufficiently well defined)
  - “Reports of new potential energy surfaces in JCPEffective 04 August 2016, the Journal requires that all papers on new potential energy surfaces must be accompanied by a tape archive (e.g., PES.tar) file containing a computer program that can be used to generate the potential and preferably also its forces for use in classical trajectory calculations. The only exception will be potentials that are simple enough to be reconstructed SOLELY from the information given in the paper.The computer program can be written in any modern computer language, but the compiler that the authors used (including its version number) must be specified, and the program must be accompanied by example input and output files that reproduce some of the key results presented in the paper. The PES.tar file will be made available to the referees to give them the option to examine it. If the manuscript is accepted for publication, the PES.tar file will be published as supplementary material.”
  - http://www.nature.com/sdata/publish/for-authors#aims-scope
- Analyses
- People are not typically publishing processes
  - Some people, but not many
- Are there agreed upon processes
  - No
- Zenodo can associate DOIs with releases
  - See if we can find some DOIs
- Binder can execute Git notebooks
  - General agreement that there is movement in this direction
- Is there a driving force?
  - Likely not, just early adopters
- Very big disconnect between younger and older crowd
  - Potentially things changing as younger take over
- What would it show to demonstrate value?
  - When people start to feel like they’re being left behind by not doing it
  - Increased citations
    - Bio paper shows increased with bio pub
  - Reproducing published data could help to encourage
  - Some of the things citrine is doing really helps, losing intimidation factor
    - Citrine - for any tools there is a higher barrier to use than what we think. A lot of time spent installing python. 
    - 1-1 time helping people use them
    - Potentially anecdotal evidence from working with groups showing improvement in productivity
    - Taylor sparks (Utah) mentioned in article that he got 6 papers by using citrine tools
  - Fear that someone will steal my data before I can.
    - Citrine: provide a private data that can be used on the platform - When they finish paper its simple to then publish data
    - Come up with as many ways as they can to keep a linkage between when someone uses a dataset to link to that dataset (e.g., credit)
    - People are concerned that others might take the data and not know the history of the sample. WIthout that knowledge analyses might not make sense. 
    - Lucas - originally worried that data will be misinterpreted. But it hasn't been that bad
- What data types would be of most interest for deep indexing?
  - E.g., we built a parser for VASP


- Discussion of representative notebooks (can we create a shared repository for these?)
  - Logan
    - Took an open dataset published in UConn Journal of Chem physics
      - Published dataset on their own database, processed data files
      - Did not publish process, software for training the model
    - ML model to determine force around an atom, common in MD
    - 3 notebooks 
    - Downsampling, reproduce figures from the paper
  - Can we get a collection of notebooks from group members
    - Logan will share his, others will send Lucas
    - Max has lots of Citrine ones open 

- Internship proposal (Kyle): Reproducing published analyses and applying to new datasets
  - Reproducing publications?
    - Least impactful (not so excited)
  - Combining datasets 
    - This seems like it would be most interesting
    - Max has example of improving accuracy by combining datasets
    - Elif has lots of examples working on center-scale projects would be motivating for the community to combine. Facilitating interactions between large groups of collaborators. Merging all their datasets together. 
- Datasets to index
  - Lucas interested in more experimental data. Magnetic sensitivity. 
  - Elif interested in materials reference data (stupid that it's so time consuming, even to find something simple)
  - Citrine is pulling data points from plots as the plots themselves are not so useful.
  - Citrine not sure on how much experimental data they have vs computational 
  - 2.7 M on public DB, 2M computational

- Logistics revisited
  - Preferred meeting frequency
   - 4-6 weeks
  - Should we aim to meet in person and when (NDS 7/UIUC)
    - Send email about NDS7
  - Meeting notes and agenda on Google Drive
  - Shared storage for datasets (Petrel), Box for smaller files?
  - Other members to invite?
  - Github repo for descriptions of use case, paper draft etc.



2017 01 26 - Meeting Agenda

Introduction, welcome
- Andre - electronic properties of materials. Recently started a project with experimentalists interested in using WT/MDF to establish a pipeline
- Elif/Josh - computational materials/physics simulation group. One project with Lucas relates to creating a database of materials properties using QMC. Interested to integrate with MDF. Second project related to materials design, designing new materials for shape memory alloys. Large quantities of data, want to make open and accessible. 
- Lucas - development of benchmark code for electronic structure calculations. Been working on workflows to perform these computations, used to create DFT functionals. Working in condensed matter physics - they have a way of providing simple models. Large amounts of data. 
- Zach - improving accessibility, discoverability, usability of materials data. 
  - Note: NIST computational reproducibility - CoRR (cloud of reproducible records). Web app wrapper around sumatra and other tools.
- Raf - experimentalist at MIT,  making semiconductors. Has a long interest in data management. Interested in the intersection between materials, library science, data management. Wrote a workflow tracker, how can we make this provenance tracking capability a world wide resource. 
- Logan - recent materials grad. Building machine learning data for materials data. Looking at what we can do with MDF data (and other materials data)
- Michal - MDF team, research programmer at NCSA with a background in materials and experimental physics (electron microscopy).. Main role is outreach and looking after storage. Interests in experimental data. 
- Kyle - CS background, distributed computing, research data management. Working on MDF and WT. 
- Jonathan - working on MDF to ingest datasets and harmonize metadata formats
- Ben - leads MDF. Working with users etc. 

Brief software introduction
- NIST/MDF introduction (5 min) - Ben
- CHiMaD/NIST funded effort to enable materials data publication/discovery
- Storage allocation at NCSA/ANL
- Can publish data to MDF, and get a doi
- Working on a data discovery service (both whole datasets, and results within datasets)
- NSF Whole Tale introduction (5 min) - Kyle
- Environment for finding/importing datasets
- Frontend environment for analyzing data (e.g., using Jupyter)
- Ability to record analysis, capture frontend + raw/derived data (or references), and support sharing/publication
- Integration with publishers to complete the loop
- Focused on software glue where possible

Discussion of WG outcomes
- Building use cases for MDF/WT development
- White paper/paper based on discussions/recommendations
- Looking at (and publishing) group datasets

- Zach And Chuck Ward are planning a materials data platform integration summit (hackathon working meeting). Aim to define touch points between applications and platforms.  E.g., Independent service to run extractors (NREL, 4CeeD, BrownDog). Summerish - independent of a conference (Dayton). 
- Lucas - interested in more interactive interfaces for exploring datasets. Look at it in different ways, determine if the viz matches the model, etc. Could we develop a D3 webservice to allow general exploration (Bokeh? Plot.ly?)
- Raf - what would computation/simulation people like to see from experimentalist (metadata etc.)

Resources available for WG
- WT Hackathons
- WT Summer interns
- WT Developer time to build out WG-specific capabilities (e.g., MDF  +Jupyter integrations)
- MDF development/consultancy time to help wrangle data, explore integrations, build prototypes

What is your process and data?
- Data management discussion
- Where is your data stored, how is it accessed, embargo, etc. any problems with DMP
- Elif - use github for everything (workflows, codes, and some data)
  - Interested in starting with the simple things, e.g., making Jupyter notebooks accessible to others. 
  - Last couple of review panels have asked to look at data/software distribution with respect to DMP
- Lucas  - uses github/box
  - Also has large storage server
  - Data has not been so big that it can't be included in supplementary doc 
- Andre
  - Server with HDD, when they want to publish they would like to put the data in MDF alongside the paper
  - Workflows stored in GitHub
- Raf - using LIMS system to track provenance 	
  - Computational processes discussion
  - How is data analyzed, what types of analytics are applied, where is the field heading
  - Jupyter notebooks + workflows
  - Many people are using notebooks
- Logan - Bash scripts and Fortran
  - Most people are using Mira/BW/Nersc and campus cluster at UIUC
  - Some post processing run on supercomputer - resulting data not so big
  - Jupyter notebook then used for analytics of the resulting data, some use XMGrace/GNU plot (plotting tool)
  - Standard has been x, y and then plotting. Recently, moving to a more data science viewpoint. All data organized in a column-based - format.  Use Pandas dataframes. 
  - Provenance (e.g., parameters) is currently stored . Working to make part of the Python tool that automates input file creation and - records the params.  Pickled. Used to turn into a table depending on question. 
  - Started thinking about a schema for metadata.
  - Here’s an example from Dallas of how we might want to present data: http://magnesium.matse.illinois.edu/wsgi/graphmisfits/
  - There is merit in publishing level 0/1 data.  In some domains it's still unclear how to move from 0-1 so it makes sense to keep that raw data. 
Publication discussion
- What types of data/analysis are related to publications
- What efforts exist to support these methods
Group logistics
- Preferred meeting frequency
- Should we aim to meet in person and when (NDS 7/UIUC)
- Meeting notes and agenda on Google Drive
- Shared storage for datasets (Petrel), Box for smaller files?
- Other members to invite?
- Github repo for descriptions of use case, paper draft etc.
- Get google and github IDs
