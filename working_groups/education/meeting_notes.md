# Education and Training WG Meeting Notes


2/22/2019
=========
April, Cheryl, Craig

* Agenda
    * Room informatoin
        * http://www.ncsa.illinois.edu/about/facilities/events
        * Room 1040
    * Workshop
        * Thu-Mai
            * Landscape and how we're supporting it
            * "Pre-producibility" data quality
            * Journal and checklists
            * How the repository supports research transparency
        * Presenters draft 1 - 2 questions for audience
        * Evaluation
            * What are the most important things?
            * Sticky notes -- put it up there
            * Force them to get active
            * Questions via sticky notes
    * Working-workshop
        * Curriculum sprints
    * Travel
        * Hotel recommendations
    * Actions:
        * Craig: 
            * Google folder
        * April:
            * Presentation/travel + structure for curriculum dev

## 2/1/2019 Reproducible Research Workshop meeting notes
April, Matt, Thu-Mai, Cheryl, Craig

* Agenda
  * Working workshop
  * Meeting our goals
* Proposed working workshop
    * March 7-8?
        * Arrive Mar 6th and tentatively leave Mar 8 afternoon.
        * Morning presentations on Mar 6th
    * 1.5 - 2 day
        * < 0.5 shorter workshop with presentations
        * 1 - 1.5 working
    * Short workshop format
        * Two options:
            * Mini-training/April's existing material ++
            * Position presentations/engaging with like-minded folks (preferred format)
                * How big of an audience?
                    * Max 40-50?
                * Potential topics:
                    * Victoria/Bertram: Intro
                    * April: Summary of types of outreach + CodeOcean
                    * Thu-Mai: 
                        * Sharing/repository
                        * Curation/quality workflows?
                        * Verification?
                    * Matt: Computational physics perspective; reproducibility metrics
                    * ? Neal/Elizabeth: Carpentries perspective
                    * ? Binder
                * Questions to inform the curriculum development
                    * ACS: What are the main learning objectives?
                    * CW: Where are the gaps?
                    * MK: What space should tooling occupy in the course?
                    * TMC: Researchers want others to select the tools
                        * ACS: Discoverability; how to choose tools
                    * Discussion of Docker (and other things) and archiving
                        * But also archiving source code (and data)
                        * Which tools are best for which side of the spectrum?
                            * Github is not archiving, but better than nothing
                            * Containers are better than Readmes
                        * Discussion of Github v Git
                            * There is guidance to use Github for researchers to share
        * Discussion
            * Victoria is interested in talking, probably Bertram too
            * April has out-of-the-box non-CO
            * Matt has 
            * Who is the audience?
                * Whole Tale team
                * UIUC community
            * Do we need to do evaluation?
                * Can we evaluate what happened in the workshop
            * What would be more helpful?
  * Getting things going again -- meeting our goals
      * Concept map
      * Mapping RR curriculum to other carpentry lessons
          * Is the RR material really intended to lead to the other carpentries?
      * What is the best use of our time? What will we do during the meeting?
          * Concept map/reverse instructional design -- having some sense for ourselves/a start on that.

## 11/20/2018 Reproducible Research Workshop meeting notes
Thu-Mai Christian, Matt Kraftczyk, Bertram Ludaescher, Cheryl Thompson, Craig Willis

* Craig: 
    * We have forked the carpentries repos, and are creating issues based on updates we think will improve
    * https://github.com/computational-reproducibility-workshop
    * There is an organization that creates a website that brings the curriculum together
    * Issues are being managed using Github projects:
       * https://github.com/orgs/computational-reproducibility-workshop/projects/1    
* Thu-Mai: 
    * Looking at the existing material, can we bridge data curation and researcher communities (management/practice)
    * How can we introduce the management concepts to be meaningful to researchers?
    * April: Can we identify the points at which we can make these connections? Or make them better?
        * Practical but rooted in a greater mission
        * Principles and dissemination?
    * Craig:
        * Can we/should we expose the researcher to the curation workflow?
        * Thu-Mai: There's a discrepency between what they think is complete and what is complete
        * April: We talked about starting people with an example of something that isn't complete and have them get it going
            * How far can we take it?
        * Craig:
            * Discussion of expanding the "gapminder" example.
            * Can we expand this -- data + code, put them in the position of the re-user or curator?
            * Thu-Mai: Discussion of different missing pieces (needs more metadata or documentation)
            * Matt:
                * Has examples in C/C++ and Matlab
                * Craig: We're trying to keep things modular
* Discussion of examples:
    * April:
        * Documentation exercises are hard for people in the room who didn't create the data
        * Her exercises include data collection because of this
        * Thu-Mai: This is useful -- a basic example. There are sometimes people with no exposure at all.
        * Bertram: Comment on dependencies/co-dependencies
            * Can there be an exercise that shows 2+ input files
            * There's an error in the input file
            * Workflow diagram of dependencies between file states
            * Tools that display dependencies -- overall data flow?
            * April: Reference to Gitbook Reproducible...(URL?)
                * Example of workflow from collection to publication
            * There's code and data but also flow
            * Workflow as documentation
    * Matt:
        * What would be a good example?
        * In his area, people will give you a function
        * Would this be an area to start?
            * Need to describe how to execute, input data, how to pro
        * Craig:
            * Discussion of AJPS submission
            * Multiple iterations and what needed to be changed
            * Thu-Mai: We can work backward
            * Cheryl: For data curation, we have students look at multiple examples, one that are really good, ones that aren't
* Cheryl: Q. Are we thinking about reproducibility in terms of observational reproducibility or other, e.g., simulations?
    * Matt: Doesn't see this as too different.  Usually for simulations, they'll provide an example.
    * Discussion of cleaning in the context of similulations:
        * Matt: You have to deal with cleaning/post-processing of simulation anyway.
    * April: We should focus on what type of reproducibility we'll try to bring people to.
        * Existing material doesn't have definitions per se
        * More targetted at motivations -- we need to frame it to be as meaningful as possible, even if the scenarios don't perfectly fit you.
    * Bertram: Have some scoping of the different types of reproducibility
        * Dirty data, questionable origin, statistics
        * For the purpose of this, we're focusing on: computational reproducibility...
        * Intentionally broken examples (e.g., python version not specified)
    * Note: reminder of overarching goals 
        * We are focused on computational reproducibility
        * Focused on the packaging/sharing/publishing/dissemination
            * Also for yourself
* Discussion of outline
    * Restructuring + adding "Documentation" repository/section
    * Q. Should we teach them how to move away from Excel and to Rstudio/programming?
        * Gets to the question of teaching programming. Do we or don't we?
        * April: It's hard enough to teach them to packaging/dissemination
            * Require as a prerequisite that they are using code. Make it clear.
        * Thu-Mai:
            * Make it a recommended prerequisite
            * Let's not omit them altogether
            * Can we produce primers -- reading data -- how to move from Excel to Jupyter/R/etc
            * April:
                * If someone is using Excel + code, there are non-reproducible ways to use Excel, even if they are using code
                * People come thinking that they'll learn to code, and leave disappointed
        * Consensus:
            * Develop primer material but assume prerequisite coding experience
            * Assume they know the material
* Contributors:
    * We all want to contribute
        * Introduction/Outline - April
        * Organization
        * Documentation - Craig
            * "Literate programming"/intro to Jupyter
        * Automation
        * Dissemination
        * "Examples"

### 11/7/2018 Reproducible Research Workshop meeting notes
Craig Willis, April Clyburne-Sherin, Aaron Culich

* Background:
  * We've forked existing material into new organization https://github.com/computational-reproducibility-workshop
  * Talking about [April's existing materials] and Craig's [notes after reviewing the existing carpentry materials](https://docs.google.com/document/d/1xXwpALyS20hVUpo8bwVYoLTHRZ_PzTxWGDLu6LqzQ4g/edit)
* We will use Github issues and projects in the new organization to organize what we're doing.
* Review of Craig's [notes onthe existing carpentry materials](https://docs.google.com/document/d/1xXwpALyS20hVUpo8bwVYoLTHRZ_PzTxWGDLu6LqzQ4g/edit)
  * Current materials lack some of the motivation and framing that's in April's slides
  * Modules should be more modular, covering broad concepts (platform agnostic) and RStudio/Jupyter can be plugged in for specifics
  * Discussion of [NCEAS training materials](https://nceas.github.io/sasap-training/events/reproducible-analysis-fairbanks/#preparing-for-the-workshop)
    * This is more of a programming class -- a deeper intro to R 
    * "Reproducible scientific programming" versus the higher-level things that are a barrier to reproducibility.
    * Onus is on us to clarify exactly what we're teaching. There are lots of ways of teaching "reproducibility".
    * There's not much that focuses on reuse, not just reproducibility (e.g., open source language, packaging, version control)
    * How do we differentiate: Reproducible publication, reproducible sharing?
  * Discussion of metadata 
    * Not really covered in existing material. April covers data dictionaries.
    * April is considering including data packaging
        * Frictionless data -- has a tool that creates something similar to data dictionary: https://frictionlessdata.io/
            * Upload CSV, automatically creates JSON file and tests that fields are what you say they are
            * Introduces idea of verification
    * Q. Is there a way to include a broader introduction to domain metadata schemes (e.g., DDI, EML)
  * Discussion of documentation:
    * One of the four facets, but much of the time is spent on programming in the current material
    * Q. How deep do we go into teaching the programming aspects (e.g., python/matplotlib)
        * All of the Jupyter/R/NCEAS workshops include some level of data manipulation/plotting programming examples.
  * Discussion of automation module:
    * Automated tests aren't a focus for April due to "infrequent programmers"
    * Q. Can we cover the spectrum e.g., of validation/tests -- good enough, better, best
    * Missing master scripts and relationship to reuse/reproducibility
        * This is very important for the verifiers at Odum
  * Dissemination
    * How to publish a repository instead of a file
        * Binder > Zenodo, Dataverse
        * Whole Tale > DataONE, Dataverse
  * Other
    * What about the scripts and data behind figures?
    * Discussion of reproducible "packets" for figures with their own DOI [repropacks](http://blogs.nature.com/naturejobs/2017/04/17/techblog-my-digital-toolbox-lorena-barba/)
        * Q. Can we find examples?
    * Regeneration of the figure is an easy motivator.
    * Mention of V. Sochat's [Scientific Filesystem](https://academic.oup.com/gigascience/article/7/5/giy023/4931737)
  * What's next?
    * Create issues or implement clear things, using PR's if desired.
    * Introduce master script concept to existing material
    * More of the broader/general concepts/motivations that need to be added
    * Propose Documentation section and how to fit existing material into it
    * Next meeting 11/21


### 10/30/2018 Reproducible Research Workshop meeting notes
Craig Willis, Thu-Mai Christian, Matt Krafczyk, April Clyburne-Sherin

Thu-Mai intro (Odum Institute)
* Working with consortium for data curation for reproducibility including code review -  Curating for Reproducibility (CURE) Consortium
* How do we steward data with computational reproducibility in mind?
* Q. CW - do you teach reproducible research at Odum?
  * Odum supports journals, so we would do this before they publish
  * At Cornell Institute (CISER) for they have have a pre-publication service
  * At Yale they provide the service for their researchers
  * There aren't lots of people that can do it
* Q. MK - what are the languages?
  * R and Stata 
  * M+ and GIS applications
  * For stata, they require the scripts

Background for this meeting: 
* Review of previous meeting notes (below)
* Revisited: Why use the Carpentry model?
  * ACS - has been evaluating shorter curriculum, would like it to be discoverable/open, would benefit from community improvement.
  * Q. MK - How does it work?
      * Via Github
  * Q. TC - CURE is interested because they have an established mechanism. What are the drawbacks?
      * Discussion of Carpentry process 
  * Q. TC - does it matter where it falls? Data/Software/Library?
      * ACS - They have tried to move away from the distinctions. RR is currently under DC.
      * CW - Thu-Mai may have audiences of both researchers and curators
      * ACS - Spoke with collaboration with Library Carpentry need and there was an interest.

Consolidation:
* Review of [Google Doc](https://docs.google.com/document/d/14WsKlQXs4A7b3tU0lpA6PgGQTvElLEfL3LYy_7NvbFU/edit)
* Revisied: Whoe is the audience:
    * Graduate students/postdocs/researchers
    * TC: librarians/curators, maybe separate curriculum
        * Librarians are train-the-trainer
    * MK: What type of researchers? Works with physicists.  Only 1/55 reviewed had a Jupyter notebook. Many people in the field don't use them.
        * CW: Material should be modular
        * MK: People don't understand what's missing to make their stuff reproducible. It would be good to include examples -- real problems real researchers have.
            * Group agrees
        * TC: Uses these types of examples to motivate other sessions
        * ACS: We liked Matt's suggestion in the notes, but the hard part is finding the right ones. Also examples of Woodbridge to replicate Jupyter notebook. Just sharing code isn't enough.
        * MK: what types of examples to make available? Let people find the one that's closest to their work.
    * ACS: Can possibly survey in advance to suit 
    * ACS: Have they had exposure to scientific programming?
        * Initially no. May not have had SWC. May not know how to use Git. Any Git introduction needs to be simple.
        * TC: Git is hit or miss.
        * MK: Teaching merge etc is harder.
        * ACS: What about Github?
    * MK: Can we talk about complex topics like Git that have a general conceptual framework with different implementations?
        * Managing versions, branches, histories, etc.
        * Git does it one way, Github another, Box another
        * ACS: Best step is to pick a core audience for the first run, then start to expand.
        * TC: Basic git concepts using Legos? Force11
* Discussion of high-level organization based on ACS and Carpentry existing materials:
  * Intro/Motivation
  * Organization
      * Creating one repo
      * Project structure
      * Separating code/data
  * Documentation
      * Specification of environment/package versions
          * Dependencies from readmes to containers
      * Project README
      * Data documentation
      * Literate programming (e.g., Notebooks)
  * Version control
      * Q. Tension - to Git or not to Git? What about Github? CLI can be intimidating.
      * Q. How to teach versioning otherwise? Box users? 
          * Naming conventions, converting to read-only at some point.
          * OSF 
  * Automation
      * Creating master script
  * Dissemination
      * License
      * Publishing
          * General best practices
* Additional comments:
    * Create your own dataset or have one with known problems. Hands on example.
    * How much programming do we incorporate? Variable naming, etc. v assume SWC experience/
    * Using Github
    * How to share a container (Docker overview)
    * Versioning
    * Sharing as collaboration v sharing as making available to community. 
    * Publication as distinct from collaboration
    * Publication as release
    * Librarians should know what literate programming is without needing to know how to do it.
    * Finding the right examples -- to demonstrate practices.
    * Platforms are one way that are translatable to workstations.
    * Dependencies -- also includes say compiler/install flags
    * Publishing
        * Need to archive a version and mint identifiers that can be cross-linked to publications.
        * MK: Publishing as installation or release?
        * TC: What is the purpose of publishing and how you package and for whom. Is it for reuse, or just for the record, or for collaboration.
        * MK: Main reason is the record -- so others can get it and run it.  Importance of sharing code even if you can't install and run (can still read it); more detailed than your paper.
    * What about verification/validation?
* Next steps:
    * Fork the Jupyter workshop
    * https://github.com/computational-reproducibility-workshop
    * Thu-Mai: @RDA next week

### 2018-10-17
Craig Willis, April Clyburne-Sherin

* ACS: There is a gap in discipline agnostic computational reproducibility practical hands-on workshop. CO/WT/Binder are in a place to address this.  
* Elizabeth Wickes (UIUC iSchool, Carpentries executive council) expressed interest in running [Reproducible Research using Jupyter Notebooks](https://reproducible-science-curriculum.github.io/workshop-RR-Jupyter/) at UIUC
* Discussion of [proposed Workshop](https://docs.google.com/document/d/14WsKlQXs4A7b3tU0lpA6PgGQTvElLEfL3LYy_7NvbFU/edit?usp=sharing)
* Q. Carpentries model or not?
  * There is value in the shared curriculum and existing recognition of Carpentries
  * However, there is no official RR curriculum, so it's unclear whether it can be an "official" workshop
* Q. How does material become official?
  * Need to ask community 
  * There are others interested in RR material incorporated into Carpentries
* Q. Jupyter v RStudio?
  * Some existing material is very R-centric. For some communities, language/tool selection is important.
  * Carpentry workshops tend to focus on a single language
  * We lean toward notebooks
  * Acknowledged that there is some concern about teaching programming using notebooks, but notebooks are good for packaging RR
* Q. Can we assume they've had software carpentry?
  * There is a space for people who are not proficient in programming
  * Need to balance with more advanced users 
* Q. 2-day v shorter?
  * There's a tension -- some people won't sign up for 2 days but will complain if 
  * Can we somehow split into 1-day software/data 1-day RR?
  * Maybe a problem with overall narrative
* Next steps:
    * Sorting the content for workshop
* Looked at two different modules
    * http://swcarpentry.github.io/r-novice-gapminder/guide/
    * https://reproducible-science-curriculum.github.io/workshop-RR-Jupyter/
        * A little about organization, but mostly literate programming with Jupyter
* What's missing from CO
    * Not much time on organization
    * Not much time on literate programming
* Real world example/hands-on is more compelling than a lecture.
   * BYO data and code and try to run it? Or find a good public example
* Version control/Git
   * Command line Git is not for everyone
   * Github/Gitlab is easier intro
   * Important to have a place where your stuff is (regardless of whether Github)
* Dependencies
   * Good to cover importance of environment
* Demonstrating publishing
   * General best practices (platorm agnostic)
   * Pathways for different tools
   * Share repo, mint identifier for version of record
* What's missing?
    * Licensing
* How to proceed
    * We have a sense of how things could come together from the existing material.
    * Could create a repo to bring the narrative together
    * Git issue/schedule call/meeting with Matt + other stakeholders
        * Where would the material go?
        * Fork reproducible-science-curriculum or become members?
        * https://carpentries.topicbox.com/
    * Logistics 
* Deadlines
    * Outline of consolidated lesson plan by Nov 9
    * First pass at more detailed plan by Nov 30

### 2018-09-19
Craig Willis, April Clyburne-Sherin
* April has existing training material, much is which is platform agnostic, and is interested in sharing with a wider group of instructors. 11 exercises, 2-4 hour course.
     * A version of the training slide deck can be found here: [Preparing your data and code for computationally reproducible publication](https://docs.google.com/presentation/d/1vgKdbFYSiEvDuOp11xgOifosl5qsQoKPgMW5HY5pK0o/edit?usp=sharing).
     * A general outline to the existing workshop is below:
         * Computational reproducibility
              * Crisis or opportunity?
              * Facets of reproducibility
         * Organization
              * Exercise 1: Data collection
              * Exercise 2: One repository
              * Exercise 3: Separate code & data
         * Documentation
              * Exercise 4: Specify a run environment
              * Exercise 5: Specify dependencies
              * Exercise 6: Create a README
              * Exercise 7: Create a data dictionary
         * Automation
              * Exercise 8: Create a master script
              * Exercise 9: Create relative paths
          * Dissemination
              * Exercise 10: Specify a license
              * Exercise 11: Publish your code
     * Would be a good fit for Carpentries (thinking about learning objectives, efficacy) and she has already started discussions with Library Carpentry group to bring reproducibility resources into the library.
* For researchers, there is an increasing demand for training in computational reproducibility. 
* Possible next steps:
  * Discussed idea of WT running a workshop at NCSA on computational reproducibility
  * This could be a two-day workshop. Per earlier discussions with Neal, aim for early in the semester (January 2019?)
* Actions:
  * Draft preliminary plan and circulate with WT stakeholders by Oct 5th
  * Solicit input from Carpentry community as well as DataONE/NCEAS and Berkeley. 
  * Will need to define who the community is and who will facilitate  

### 2018-09-18
Craig Willis
* Notes from discussions at Whole Tale [Chicago Workshop](https://wholetale.org/2018/06/26/working-group-workshop.html) and [PresQT meeting](https://presqt.crc.nd.edu/index.php/2-uncategorised/28-agenda-implementation-kickoff-mtg)
* Discussed possibility of WT leading/contributing to carpentries material related to research reproducibility or to run courses based on existing materials.
* PresQT meeting discussions with Vicky Steeves (NYU, ReproZip) and April Clyburne-Sherin (CodeOcean) about concept of carpentries-esque training 
* Jane Wyngaard (ND, CRC) pointed to existing materials in Carpentries community
   *  [R and RS data carpentry materials](https://datacarpentry.org/rr-workshop/)
   * [Community discussion thread with many RS resources suggested](https://carpentries.topicbox.com/groups/discuss/T88876b4d533302bf-M1974b2ac585a09add1ca2675) (resources follow)
   * https://datacarpentry.org/blog/2015/12/reproducible-research-curriculum
   * https://github.com/Reproducible-Science-Curriculum: Note contributions from Tracy Teal (Carpentries), Chris Holdgraf (Berkeley), Matthew Collins (at WT Workshop)
   * http://www.datacarpentry.org/rr-workshop/
   * https://ropensci.github.io/reproducibility-guide/
   * https://www.practicereproducibleresearch.org/
   * https://2016-oslo-repeatability.readthedocs.io/en/latest/
   * https://www.coursera.org/learn/reproducible-research
* Matt Jones provided via email:
   * "We teach a reproducible research course in R that has 2 day, 5 day, and 3 week variants.  Materials for the 2 day and 5 day variant that we taught in August are here 
     * https://nceas.github.io/sasap-training/materials/reproducible_research_in_r_anchorage/
     * http://training.arcticdata.io/materials/arctic-data-center-training/
* Results of quick search based on this activity
   * https://datacarpentry.org/rr-literate-programming/
   * https://datacarpentry.org/rr-version-control/
   * http://ropensci.github.io/reproducibility-guide/sections/introduction/
   * https://nbis-reproducible-research.readthedocs.io/en/latest/
   * http://eriqande.github.io/rep-res-web/
   * http://ocw.jhsph.edu/index.cfm/go/viewCourse/course/repdata/coursePage/syllabus/
   * https://osf.io/vkhbt/
   * https://www.icpsr.umich.edu/icpsrweb/sumprog/courses/0235
   * https://www.force11.org/fsci/2018/course-abstracts
   * http://adsabs.harvard.edu/abs/2015AGUFMIN43D..07J
   * http://blogs.nature.com/naturejobs/2018/06/11/git-the-reproducibility-tool-scientists-love-to-hate/
   * https://www.natureindex.com/news-blog/when-it-comes-to-reproducible-science-git-is-code-for-success
   * https://www.xsede.org/web/reproducibility



### 2018-08-30
Craig Willis, Neal Davis

Meeting with Neal Davis, UIUC liaison, about possible integrations of WT into Carpentry curriculum and process for running Carpentry workshops at UIUC.

TL;DR: 
* We could easily coordinate with Neal to run a Whole Tale-centric carpentry workshop at NCSA. 
* Getting WT material into the official curriculum would be more challenging (and probably doesn't make sense, at least not yet).
* We would need to define the required curriculum, define audience, when to run (beginning of semester best for students).  He suggests a minimum of 10 attendees.
* Would need to decide on how to handle expenses (WT pays or pass cost to attendees. He indicated that free is bad unless attendance mandatory)

ACTIONS:
* What does the curriculum need to look like
* When and to Whom?
* Expenses/catering: Pay for workshop or pass the cost on to attendees
* Experience: free is bad unless attendance mandatory
* Scheduling: Meet with Neal, beginning of semester is better for students, minimum of 10 attendees

Notes:
* The Carpentries
   * International community of instructors that develop a curriculum
   * https://carpentries.org/
   * https://datacarpentry.org/lessons/
* We have a local "chapter" of probably 15 active instructors
   * Put together 2-day workshops
   * Supported by CSE@NCSA
   * NCSA supports with access to 1040
   * Research IT pays for affiliation for the University
   * iSchool also involved
   * Would like to have different centers of activity
* Upcoming workshops
   * Will do a workshop at the end of Sept for IGB
      * Targeting researchers  (masters and above)
      * Computational lab skills
      * How do you manage data/process
      * 9/27 - 28 Topical - genomics, ecology, 
   * Software carpentry: 9/6 - 7
   * Data carpentry: 3 this month?
* Working with other groups/projects
   * They arrange the space, groups pay a flat fee
   * Example grant-funded projects include KnowEng, CIS
   * Several local instructors
* Discussion of native environments:
   * 3/4 of students are running Windows, explicitly require a laptop
   * Use Binder as a backup if student's environment is problematic
* Discussion of WT partner institutions 
   * Run it here to get started
   * Maybe at partner institutions or run at a conference
   * Official requirement by Carpentry foundation
      * At least one certified instructor
      * Teach a certain minimum set of topics
      * Command line, version control, programming
* What we need to do?
   * What is the goal of the WT session
   * What is the minimum prior point to get there
   * Normally plan on a 2-day workshop
* Cost@NCSA
   * Room for free when run at cost (no AV support)
   * Charge $40 per student for two days of breakfast + lunch
   * ~$1500
  
  
### 2018-08-30

* Circulated draft call for applications https://docs.google.com/document/d/15ODQP4Gm6yBjoTxgmvORhDAmC0mmZUG8QJVJqNkF0uY/edit and draft program proposal for feedback https://docs.google.com/document/d/1u9n8ZwnbqnUUvNtsY-21jFytv4kmEXDEbVt5YKUViz8/edit.
  
### 2018-08-23
Craig Willis, Bertram Ludaescher

Discussion of benefit of proposal:
* Is there a benefit to working with RDA? Yes, there is overlap and the PI team has discussed how we can better integrate with RDA working groups.
* This could be an opportunity to bring new energy to some of the working groups and explore specific issues of overlap with RDA (data citation, software citation, reproducibility, provenance, composite research objects, etc).
* Craig will draft a call for applications for review.

### 2018-08-22 
* Craig met with Inna Kouper, RDA/US ECF PI, to discuss possible options
* Drafted proposal for joint WT - RDA/US ECF fellowship


### 2018-08-13
Bertram, Kacper, Craig

* Bertram to contact Beth Plale regarding RDA fellows program.
  
