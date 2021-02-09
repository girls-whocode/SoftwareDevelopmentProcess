# Development Document Process

<details><summary>Menu Map</summary>
<p>

* [Home](../README.md)
  * [Development Cycle](Dev_Cycle.md)
  * [Documentation Scopes](Documentation_Scopes.md)  
    * [**Dev Documentation** :arrow\_backward: (Current Page) ](Document_Design.md)
    * [Markdown Language Guide](Markdown_Language_Guide.md)
      * [Block Quotes](md_pages/Blockquotes_Tutorial.md)
      * [Colors](md_pages/Colors_Tutorial.md)
      * [Emojis](md_pages/Emojis_Tutorial.md)
      * [Emphasis](md_pages/Emphasis_Tutorial.md)
      * [Footnotes](md_pages/Footnotes_Tutorial.md)
      * [Headings](md_pages/Headings_Tutorial.md)
      * [Horizontal Rules](md_pages/Horizontal_Ruiles_Tutorial.md)
      * [Line Breaks](md_pages/Line_Breaks_Tutorial.md)
      * [Links](md_pages/Links_Tutorial.md)
      * [Lists](md_pages/Lists_Tutorial.md)
      * [Math](md_pages/Math_Tutorial.md)
      * [Paragraphs](md_pages/Paragraphs_Tutorial.md)
      * [Syntax Highlighted Code](md_pages/Syntax_Highlighed_Code_Tutorial.md)
      * [Tables](md_pages/Tables_Tutorial.md)
    * [Markdown Lint Guide](Markdown_Lint_Guide.md)
    * [Your README.md](Create_README.md)
  * [Software versioning](Software_Versioning.md)
  * [Source Control](Source_Control.md)  
  * [Code Reviews](Code_Reviews.md)  
  * [Coding Standards](Coding_Standards.md)  
  * [Project references](Project_References.md) 

</p>
</details>

## Requirements

Note: If you find yourself writing long versions of these documents, it’s probably not going to work.  These should be relatively brief.  If there’s complex functionality or some R&D that needs to be done, that should be noted.

### A main description of the problem that the software solution should solve.  Includes/May Include:

* Existing problems or triggering event

* Current systems

* Actors/Stakeholders (users and others) involved

* User Stories – descriptions of what the user wants

* Goals for product

* Expected ROI and how to measure

* Anticipated Support

* Orthogonal Requirements (Anything that has to be created or altered in order to fulfill the primary requirements)

* New Hardware Requirements/purchases/costs

* Systems that will have to be altered (Databases, file/web servers, etc)

* Users and what training/skills they will need

* Access Control

* Risks – what could go wrong and what needs to be done to mitigate such risk

* What approvals and signoffs are needed and when?

* How is SQA to be carried out, how will releases be staged? Deployed? Rolled back?



## Functional Specifications

### Top Level but detailed description of software function.

* Primary functions

* Primary control paths

* Orthogonal control paths, if any

* Menu Items, what they do beyond the above mentioned.

* Is anything running in the background?  Any other special behavior?

* Alerting system?

###Detailed Design

* Architecture (with Diagrams)

  * Design Methodologies

  * Frameworks To Be Used

  * Major Modules and components

* Data Design –

  * internal and external data handling, any serious internal data structures?

  * Data sources—file store, DB (MPCS) etc

* Interfaces

  * UI for Primary Actors

  * UI for Service, Monitoring, Maintenance, Deploy

  * Other contexts

  * Programming Interfaces (standards)

  * External communication interfaces (network, web, exposed programmable, etc)

  * Access control on external interfaces

* Milestones

  * What preliminary work needs to be done?

  * What will be the first internal working slice or version?

  * What will be the first proof of concept that is demonstrable for the users?

  * What is good enough for a first release?

  * What, if any, items should be left incomplete until the first release?

Now take user stories based on functional specifications and code against them according to the design. Write tests for technical requirements and code against those as well.

## Policy Docs

ROI/CBA  - Jon

Coding Standard - C#, .NET done

Rails Coding Standard - done

Interface Policy

Access Control Policy - Todd

* create a web service for all apps to return credentials (eliminate the need for secure info stored in the clear in the registry/local drive)
* get a cert to sign our exes to prevent windows alerts and in the future apply group policy against non-signed apps.
* create an access control policy that is single-signon for all web apps, desktop apps, etc.  via AD, etc. (fix mtirails)
* create an access control policy for the web interface calls themselves
* as part of coding standard have a changelog - maybe a linked to sharepoint doc?

Doug Bolte

* Requirements User Stories Author Doc - done
* Structured Summary of work done/to do - done

Allison update Gitlab
