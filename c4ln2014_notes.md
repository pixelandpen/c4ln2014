Code4Lib North 2014
====================

May 1-2, 2014
London Public Library

Thursday sessions
-----------

A brief overview of modern configuration management and deploy tools; or, why your bash scripts are not scalable.
-----------
- Sam Popowich and John Fink
- UofAlberta - moving from CF/Java; adopting Ruby/Blacklght/Hydra/Rails
- adopting devopsy approach
- bash scripts 
  - don't scale
  - break if things missing
  - don't work on multiple architectures
  - don't lend themselves to tests
- configuration management == IT automation == automated configuration
- it's a way of documenting your systems; the files are just code -- can be put in
  git
- way of making incremental, repeatable, testable changes on 1+ systems at a
  time
- Puppet - mature project; Ruby; write manifests in Ruby-like domain specific
  language (DSL)
- Chef - mature; Ruby and Erlang; pure-Ruby DSL to write recipes; usually have a
  Chef server to monitor, but can also use Chef Solo to have one machine install
  on another
- Ansible - Python; uses YAML to write playbooks
- Vagrant - wrapper (usually) around VirtualBox; Ruby
- Docker - virtualizes within containers (specific to amd64); lightweight; quick
  startup/teardown times; easy DSL to config
  
Using library systems to mould public school libraries  
-----------
- Geoffrey Allen  
- Waterloo Region District School Board - library services supervisor (1 of 6 IT
  supervisors)
- 118 school libraries, 4 political regions
- 7,000 staff in WRDSB
- 70,000 students ages 3-18
- 16 secondary school teacher-librarians
- 4 elementary teacher-librarians (was 102 years ago)
- 0 library consultants
- 120ish library clerks - require minimum of high school
- just replaced 20 year old SirsiDynex ILS this year - going with Insignia
  Software (http://www.insigniasoftware.com/insignia/ils.htm)
- 1 goal: help make our school libraries a place of learning and development by 
  easing discovery and access to educational resources.
- need to enforce good cataloguing
- e.g. quinturakids.com - of cloud/cluster for aiding with search and discovery
- DRM is non-starter for school board
- single-sign on is easy to implement from systems point of view, but vendors
  don't have/allow it sometimes
- videos were converted to Flash originally, to work in classroom PCs/Macs,
  but now not available for iPads in classroom
- admin machines (~150) use Silverlight; they are asking vendor to rewrite in
  HTML5
- @gaufredus
- redesigning WRDSB website to use RWD rather than mobile apps for each platform
- giving up on computer labs - just have mobile devices in classroom instead
- Barry Wellman - social media lab
- clustering seems to have gone out of vogue; possible reason is that it is 
  difficult to create a helpful cluster because there is so much data now -- 
  needs to be pruned in order to have a helpful cluster 

Opening library data from a hostile data source   
----------
- Dave Mitchell   
- vendor would share data, but wouldn't share data structure
- 2001 - moved to Innovative Interfaces; could only have data access IF they had
  Oracle
- Now use Sierra - promises that things were to be more open
- The "new items" lists are the most popular portion of the website now - about
  33% of traffic
- Produce about 260 RSS feeds a day - through data dumps and screen scrapes,
  with scripts polling regularly
- Sierra DNA - uses PostgreSQL database, but is limited to 5 connections
- Dave is now recreating old polling application, using Sierra DNA
- PostgreSQL has built-in replication - could have a copy that they can use that
  is not limited 

An XML Framework for Teaching RDA   
---------
- Grant Campbell  
- Teaches cataloguing at FIMS - gcampbel@uwo.ca
- Cataloguing rules not based on AACR2 
- RDA (Resource Description and Access) based on FRBR - work, expression, manifestation, and item
- RDA designed for efficiencies/flexibility of new database tech, but also
  designed to handle legacy technologies (MARC)
- MARC and ISDB formats are barrier for sharing info cross-platform
- BIBFRAME - replacement for MARC; general model for expressing and connecting
  bibliographic data
- Grant created XML schema to show students bibliographic record without being
  limited to MARC
- Didn't use attributes in XML, because wanted to highlight the
  elements; using attributes would be more efficient way to create the XML
- Uses Oxygen XML editor - but in learning lab only had Dreamweaver for students
- Still need to teach students ISBD and MARC
- The conceptual transition from RDA to ISBD and MARC is very difficult for
  students not trained in AARC2
- "How much life does bibliographic data have outside a library catalogue?"
- Early vision of shared metadata faltered due to spam - "documents deceive"
 
It's not paranoia if they're really watching you: library patron privacy   
----------
- Ruth Collings  
- neuromancer.ca/c4ln2014
- Demonstrated Wireshark for network traffic sniffing
- Highlighted Heartbleed bug
- No such thing as completely secure; need to raise cost of hacking you
- On personal security level, it is about trade-offs
- Your level of paranoia is directly related to your feeling of security
- "How paranoid should I optimally be for my environmental reality?"
- Examples of why we should be paranoid:
  - badBIOS
  - Stuxnet
  - (Government sponsored) malware
  - Gender, zipcode, birth date combination are enough to identify person
  - FBI's facial recognition program
  - Target credit card breaches
- "Feeling - Model - Reality" models
- Barriers to security
  - IT infrastructure implementation i.e. not just installing the software, but
    configuring for optimal security
  - Vendor security - e.g. passwords sent in the clear; Chesapeake Public
    Library's admin page for VuFind is available to public because using
    defaults
- Because of the cost of being secure, there is a trade-off
- Librarians need to think through how best to protect library patrons
- Need to use professionals/reputable vendors to ensure security
  - Not necessarily - e.g. Target was OK'd by security professionals doing
    security audit a few months before the breach
- https://tails.boum.org/index.en.html - OS for USB/DVD that provides tools for
  safe/secure browsing and use of Internet
- One problem is the range of devices that patrons bring to library - often need
  to accommodate the lowest common denominator

Friday sessions
----------

CRKN's Integrated Digital Scholarship Ecosystem (IDSE) Project: Overview & Feedback
--------
- Michael Ridley
- Canadian Research Knowledge Network - collectively buy digital content - about
  $100M/year
- Two pieces to IDSE project:
  - environmental scan
  - find opportunities to make a difference i.e. what can CRKN do to change the
    ecosystem?
- Questions to consider:
  - What are the key challenges and opportunities in the digital scholarship
    ecosystem?
  - What would you like to see IDSE recommend?
- P.N. Edward - "Knowledge infrastructure reshapes the geography itself" 
- Infrastructure includes:
  - servers, buildings, networks
  - people
  - vision, change
- Seamless is not just ease of access, but whole integration of the access -
  e.g. tools we can use to interrogate the resources
- Collaboration and coordination are at the centre of the ecosystem
- Challenges in the IDSE:
  - Diversity of the ecosystem
  - Financial constraints
  - Traditional perceptions of the library
  - Information technology
  - Blurring of roles / adoption of new roles
  - Incentivize digital scholarship - i.e. promotion and tenure issues
  - Engaging academic leadership
- Opportunities in the IDSE:
  - Open access / new business models
  - Tool dev / toolkits / digital labs
  - Scholarly publishing and production (i.e. non-traditional publishing;
    creating "things" such as digital objects)
  - Altmetrics / evaluation / ROI
  - R&D / centres of excellence / virtual communities
  - Government receptivitiy / CFI / Industry Canada
  - Licensing / DRM / formats / standards
- We don't have a disciplined approach to R&D in library world
- CRKN engagement matrix - look at what they monitor, engage, partner or lead in
- There is a preliminary report on CRKN website
  http://crkn.ca/sites/crkn.ca/files/crkn_idse_preliminary_report_march_2014_final.pdf
- Open discussion / Q&A based on questions introduced earlier:
  - Need better metadata for CRKN packages e.g. SFX 
  - Many libraries don't even have ownership of the base IT infrastructure, so
    can't even build the tools they need
  - Need standards in place for metadata and interoperability of the objects and
    applications created
  - Long-term funding and support for projects - i.e. avoid "digital orphans"
  - Academics' viewpoint of seeing metadata as second class compared to their
    "real" data - i.e. perception of library as hand-maiden and service
    provider; there is a trend, however, to have academic librarians as integral part of
    research teams
  - We must recognize that we have special skillsets and be willing to promote our work
  - We tend to see across the entire organization; however, others can perceive we are 
    trying to take over their turf 
  - Libraries have ability to create generic solutions rather than one-off
    applications that fit a particular need

Preliminary findings from The Effects of Digital Technology on Seniors (EDITS) Project
-----------
- Kim Martin, PhD student at FIMS
- www.editsproject.com
- Started with helping seniors coming to LPL Gadget Clinics with new ebook
  readers
- Started with interviewing 10 seniors (60+) about lifelong reading, use of the
  library, computer use, changes in info behavior
  - biased sample - seniors in group came from either church seniors group or from Western Alumni 
- Roger's Diffusion of Innovations
  - Knowledge
  - Persuasion
  - Decision
    - Adoption, or
    - Rejection
  - Implementation
  - Confirmation
- Characteristics of an innovation
  - Relative advantage
  - Compatibility
  - Complexity
  - Trialability
  - Observability
- The main reason for not adopting ereader was that the books could not be
  shared
- Most respondents were at persuasion stage
- Findings:
  - Longing for materiality
  - Technology exploration
  - Technology confidence 
- Now exploring seniors' use of other technologies to compare with ereader use,
  and also investigate their information seeking habits (i.e. most had cancelled
  their newspaper subscriptions and yet never spoke about missing the physical
  paper in their hands)
- Comment that adoption of Skype is driven by desire to see children/grandchildren, 
  whereas adoption of ereader does not have same compelling reasons

RDA relationship designators as linked data: solutions to problems?
-----------
- Scott Cowan, MLIS student at FIMS
- Frustrations with catalogue:
  - Think of the user
  - Why are catalogues so hard to search?
  - The simpler the better
- Does the problem lie with the metadata we create for catalogue records, or is
  the way we encode that metadata?
- We need to scaffold our training of users - e.g. in catalogue searching
- Big data
  - e.g. Amazon, LibraryThing, NovelList
  - Privacy issues
- Linked data
  - Using RDA relationship designators e.g. artist, composer, editor
  - Add 785, 787 fields to MARC record
- Concessions...
  - Would this create reams of unnecessary links?
  - Yes, users can use Amazon, etc. but that puts large assumptions on user
- We want people to use catalogue, but subject headings and current use of
  metadata encoding make it a challenge; seems that mix of user tagging and
  control is the way to go
- Discussion / Q&A
  - GoodReads and NovelList offer embedded solutions
  - Bibliocommons
  - Every step (in adopting RDA instead of plain MARC) from data side to 
    user-facing side is really complicated
  - Need a solution other than MARC - i.e. RDA is just added to MARC/AARC2
  - The catalogue needs to help the user at an earlier stage of research process

Let's all go to the hackfest! #hackUOBiblio update
-----------
- Sarah Simpkin - GIS Librarian at UOttawa
- Held hackfast on Open Data Day
- Had people from university and beyond
- Provided data from ILL, top 200 circulating items, user count by category, IR metadata,
  website stats, and Ottawa Public Library stats
- Various ranges of experience of participants - some needed more coaching
- Congress 2015 - will have a hackfest
- Good feedback from library staff - will be holding Software Carpentry and
  workshops for staff
- Discussion / Q & A
  - Reach out to student groups
  - Having free event lowered barrier, but led to numerous no-shows
  - May need to massage data before event so it is more readily available
    (understandable, parseable) to the hackfest participants
  - Need to have a plan for how participants can share their final products
    (e.g. Dataverse, GitHub)
  - Open data community in Ottawa was helpful in promoting the event
  - York did hackfest - partnered with students that could earn credit by
    attending
  - Need to be mindful of the school branding in projects - i.e. may be legal
    issues

DRM, ebooks, privacy
----------
- David Fiander
- Vendors know what you read, how fast you read, what words you look up in
  dictionary, and what you highlighted
- In Amazon, can subscribe to other readers' notes
- Marginalia could be profitable in regards to scholarly communication - i.e.
  researchers can learn from others' notes

Teaching SQL to Librarians at Software Carpentry bootcamp 
----------
- Chris Gray  
- Background of SC 
  - Help scientists do their science well, and do it more efficiently
  - SC takes data-driven approach to learning - i.e. change their teaching
    approach based on regular feedback from bootcamps and from looking at the
    literature
  - Goal is to make research repeatable - i.e. researchers often need to provide
    not only their research data, but also the software they used to gather and
    manipulate the data
  - Use hands-on approach, and paired learning
  - Aim for bootcamp participants to be more productive in the computing
    environment they are in - i.e. if Windows user, don't give them Linux
    VirtualBox to use
  - SC now offers bootcamps for librarians
- software-carpentry.org/lessons.html - shows how the bootcamp content has been
  narrowed over the years
- Template for setting up a SC bootcamp available at https://github.com/swcarpentry/bc
- Students use red and green stickies to show instructors/helpers whether they
  are ready to proceed or not
- Many library staff use spreadsheets and email for storing data, rather than using a
  proper enterprise database
- Databases are multi-user and can enforce data integrity
- For teaching, used Sqlite and Firefox plugin, so that students could work in
  the browser

Discussion: The Angry Nerds Squad: Freeing libraries of bad tech solutions by
challenging vanilla vendor proposals 
--------
- Small organizations and consortia can't hire staff or consultants
- Idea: volunteers that would help vet/negotiate technology purchases
- People ascribe value to things based on dollar value - hard to convince people
  of the value of free software i.e. LibGuides costs money, so it is more
  valuable than using a free product
- The RFP process is often part of the problem 
  - Open source options don't get on the list because they don't respond to the open call
  - Once vendors are in the RFP system, then you have to pick one of them, even if none are
    appropriate
- Need to have clear demands of vendors during early negotiations around open
  source, open data, privacy and security issues
- OCUL had a PKP working group but it didn't have the time or expertise and
  eventually morphed into a different group
- RFP == RFQ != RFI
- There are privacy issues in the RFP process 
- "I would rather pay our staff than pay our vendor's staff." -- David Fiander

Ruby on Rails and Sinatra Tutorial
--------
- Sam Popovich
- Tutorial about creating blog in 5 minutes using Rails
- Created a Research Data Management application in Ruby at UofA
- Don't use Rails if don't have a data model or don't use data very much in the
  application
- Sinatra is way to create static website using Ruby
- Deploying Rails to production has been a pain - but getting better with
  Capistrano, Unicorn, and nginx
- Nokogiri is the way to parse XML in Ruby
- There are lots of great tutorials and guides online for Ruby and Rails


