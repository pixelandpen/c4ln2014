Code4Lib North 2014
====================

May 1-2, 2014
London Public Library

Thursday sessions
-----------

Sam Popowich and John Fink
A brief overview of modern configuration management and deploy tools; or, why your bash scripts are not scalable.
-----------

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
  
Geoffrey Allen  
Using library systems to mould public school libraries  
-----------

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

Dave Mitchell   
Opening library data from a hostile data source   
----------

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

Grant Campbell  
An XML Framework for Teaching RDA   
---------

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

Ruth Collings   
It's not paranoia if they're really watching you: library patron privacy   
----------

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

Michael Ridley
CRKN's Integrated Digital Scholarship Ecosystem (IDSE) Project: Overview & Feedback
--------

Kim Martin
Preliminary findings from The Effects of Digital Technology on Seniors (EDITS) Project
-----------

Scott Cowan
RDA relationship designators as linked data: solutions to problems?
-----------

Sarah Simpkin
Let's all go to the hackfest! #hackUOBiblio update
-----------

Chris Gray  
Teaching SQL to Librarians at Software Carpentry bootcamp 
----------

 

