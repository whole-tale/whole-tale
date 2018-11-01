# Education and Training WG Meeting Notes

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
  
