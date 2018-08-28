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
