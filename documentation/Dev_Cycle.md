# Simple Development Workflow on Gitlab

[:arrow\_backward: Coding Standards](Coding_Standards.md) | [:house: Home](../README.md) | [Documentation Scopes :arrow\_forward:](Documentation_Scopes.md)
<details><summary>Menu Map</summary>
<p>

* [Home](../README.md)
  * [Code Reviews](Code_Reviews.md)
  * [Coding Standards](Coding_Standards.md)
  * [**Development Cycle** :arrow\_backward: (Current Page)](Dev_Cycle.md)
  * [Documentation Scopes](Documentation_Scopes.md)
    * [Dev Documentation](Document_Design.md)
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
  * [Project references](Project_References.md)

</p>
</details>

## Summary

This is a proposed starting point on project and dev cycle management. This includes a proposed workflow and suggestions for maintaining documentation and tracking issues from initial report to deploy.

## Caveats

* This is not the only way to approach this. It’s not a one-size fits all solution.
* A project owner/deploy person must exist for each project and they must be willing to be responsible to encourage/impose developer discipline.
* This is just that, a starting point. As we get this going, a lot of tools can be looked for continuous improvement on the quality of the software deliverables.

## Project Documentation

Each project should have an active README.md, documentation folder with user_guide, and development_guide folders respectivly, and finally an issue page. Each repo/project should have development and user documents.

### User documentation

* Basic end user training documents.

### Development documents

* A complete setup and install.
* All applications required, including IDE and additional packages.
* A basic summary/chart of what the project does and accomplishes.
* Describe all screens and their function.
* Any and all security issues and access control requirements.
* Describe interactions with other systems like datastores, config issues.
* Common technical issues that the administrator or technician may see.
* Test scripts and plans. Something that the BA or SQA can follow to test out the software. This includes sample inputs and expected outputs.

## Workflow

* New Feature Request or Help Desk Ticket/Bug Report triggers the creation of a new issue under the relevant project in Git repository.
  * Speculative fix can be written in as well as a description of the cause, steps to reproduce, etc.
* At the end of the fix, write relevant tests and make them work.
* Stage your commit (where relevant).  Ensure you aren’t commiting over someone else’s staged work.
* SQA checks stage and approves your fix/updates.   This may be an iterative process.
* Submit to project deploy manager, who may be a BA or senior dev. They have final say on anything deployed. They may send back an update for any reasons, but common reasons would include:
  * Poorly written code or otherwise non-conforming.
  * Non-optimal solution.
  * Security issue with the fix.
  * Test coverage insufficient.
  * Not sufficiently documented.
* When project deploy manager approves the change, they merge the candidate branch to master.
* Ensure that external resources have any necessary updates applied, and deploy.
* They then note when they deployed it, who deployed it, what branch was merged, when it happened, and where it was deployed.

## Branches

* To create a branch:
  * Pull master to your local machine.
  * Checkout a branch name that leads with the issue number (i.e. `<issue_no>_<description of your choosing>`).
  * Name the branch in the issue.
* At the end of the fix OR the end of the workday, commit and push, even if not completed.
  * Comment the current status on the issue.

## Documentations

* Update or create any documentation of your resolution in the issue.
* Document how the BA or SQA team should test the feature.
  * Include sample inputs and what their outputs should be.
* Include any external changes in the issue (This is important!)
  * Server config changes
  * Permission/Access control changes.
  * Scheduling scripts
  * Changes to database schema.  (included DDL is preferable)
  * Changes to any file stores
  * Changes to any deploy scripts.
  * Changes to any local config files.
* Write into the issue any documentation changes.
* Developer puts their doc changes into the actual docs (From the issue).  This is up for discussion about how best to do this.
* Deploys result in IT notices. Updates to FAQ's, technician, developer, and user documents.
* Issues are links to the issue page. Same with IT notices (besides a brief summary).
* When it is determined that the issue is addressed, the project deploy manager closes it.

## General Broadly Applying Rules

* If your solution is complicated, weird, or unusual, discuss with the lead dev before proceeding. Note it in the issue.
* Before starting, always pull master.
* All new branches on issues always branch from master with one exception below[^1].
* Lead branches with the Issue number. (i.e. `<issue_no>_<description of your choosing>`)
* Never reuse branches. When a branch is merged to master, that branch has been completed and no longer used to prevent conflicts with other branches. If the issue needs more work, create a new issue, and branch from master.
* Don’t use your name in the branch.
* Don’t put a date on the branch.
* It’s ok to tack on “ver2” or “additional_fix” if that’s what you’re doing on a branch.

[^1]: The exception about always branch from master: If two or more devs are working on a long running issue, they can share a branch.   While they can do what they want on that branch, it is recommended that they branch off of it for their separate work, then merge it back at intervals as they agree, but this really is dependent upon how tightly coupled their work is.