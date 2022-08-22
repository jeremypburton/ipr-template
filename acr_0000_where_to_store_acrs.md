# Where to Store Architecture Council Reviews

---
## Date - 22 August 2022


---
# Summary

We're embarking on a process of formalising our architecture council reivew process, generating Architecture Council Review documents, which will be the bsais for tracking key design decisions within hipages. 

We have a number of places where documentation can live and a number of formats it can take - in Confluence, in github, surfaced into Backyard. This review seeks to address where makes the most sense for this documentation to live.


---
# Outcome


---
# Decision Maker

Moh Khalil (Head of Architecture)


---
# Interested Parties

Architecture Council, Teach Lead Guild


---
# Domains

This is around Architecture and Engineering Process as it applies to all domains


---
# Informed

All Engineering Managers
All Engineers


---
# Context

On of the goals of performing Architecture Council Reviews is to socialise decisions, make them transparent, and enable discoverability of previous technical dicisions of significance with hipages. Its of no use having a bunch of these documents if they're not easy to find and aren't able to help our engineering team learn as they come about. As we encourage teams to formally document these decisions more and more, we want to be able to expose those decisions in the most appropriate place.

We currently have a number of places where these could be exposed:
* In Confluence using Confluence's markup
* In Github - either in a central repository or close to the systems being described ("doc-as-code")
* In Backyard - this can surface documentation from Github or elsewhere
* Through Google Docs stored in Google Drive
* A combination of the above

In the past, hipages adopted an RFC process. RFCs were generally stored in Github in a central location - [https://github.com/hipagesgroup/rfcs](https://github.com/hipagesgroup/rfcs). This has both pros and cons. 

We want all Engineers to be able to publish, collaborate, read, and discover data. 
* In order to *publish*, Engineers need to be able to easily format documents in a way that can convey the right level of information; they need to have access and persmission to write to the target system.
* In order to *collaborate*, the chosen solution should make it easy for multiple authors to make changes to a document.
* In order to *read* these documents, it should be easy for any participants to see the formatted version of the document
* *Discovery* for these documents means it should be easy to find them, there should be the ability for searching and finding of these ARCs by engineers, whether they're familiar with a specific domain or not.

Finally inspiration can be taken from [Architecture Decision Records](https://adr.github.io/) when considering the outcomes here, as this is effectively what we are creating with ARCs. 


---
# Constraints, Assumptions, Risks

It's valuable to be able to version control what we do.

This information is sensitive as it is core IP of hipages, and should be treated as such.

There are already a number of places to go to find information at hipages. Any decision taken for this piece of work should take this into account, considering information sprawl and consistency of where our documentation lives. 

The audience for ACRs is usually other enginers, but could be product managers and designers, depending on the context.


---
# Options

The following options are for consideration

### Option 1 - Published in Confluence

Concluence is hipage's wiki tool of choice. All hipages staff have access - both to read and write, and it is a tool built around collaboration. It has a search function, and it's own markup language. 

| *Pros* | *Cons* | 
| --- | --- |
| All users have access to read, write and collaborate (not just Engineers) | There is a lot of old information in Confluence - new documentation runs the risk of being hard to find amongst the masses of outdated info. |
| Discovery/search is provided | Documentation does not appear close to the code. Is this a con? Does this kind of documentation need to exist close to the code? |
| A lot of other documentation is already in place in Confluence | Markup is challenging for some formatting | 
| IDM is managed centrally through Jumpcloud. | There is not good muscle memory in documenting in Confluence from the current Engineering team |
| Can be published to Backyard as somewhere for documentation to be viewed | |
---

### Option 2 - Stored in Github - written in Markup, stored in a central "ADR" repository

We currently store our RFCs in a central repository in Github, written in Markup. This puts them in a known place allowing for discovery. This option mimics this the current proces.

A mechanism for publication is required for this method - where will the documentation be surfaced for reading and discovery - will it just be the repo (allowing the github UI to render); should Wikis within GitHub be used; or published to Confluence or Backyard as part of a build process?

| *Pros* | *Cons* | 
| --- | --- |
| One single place for ACRs | Not everyone in hipages has access to github |
| Markdown is a markup language that is familiar to engineers | Documentation doesn't necessasrily live close to the systems it describes (since it's in another repo) |
| Having a central place allows for easy finding of all docs. They are centrally located | Permissions are not granular |
| All engineers have access to Github | No drag and drop for things such as images (these need to be added to the repo manually, then referenced in the doc) |
| This provides full version control and diff support| Readable tables aren't great in Markdown |
| It's possible to publish to Confluence through tooling should Confluence be determined to be a valuable place| Requires readers to have access to the publication mechanism |
| Offline access is possible when repo is cloned and kept up to date ||
| Can edit files directly with a Github interface ||
| Full PR workflow if desired ||
| Can integrate to Github Actions if there is a need ||
| Easy to index docs and create an ongoing record for further discovery ||
---

### Option 3 - Stored in Github - written in Markup, stored in a domain respository

This option is the same as option 2, but involves storing the doc closer to the team. This could be in a domain specific repo. 

| *Pros* | *Cons* | 
| --- | --- |
| As per option 2, but with the docs being closer to the teams producing them | Increased overhads when teams move around, or domain boundaries change |
| Finer grained permissions available if required | A decision may cross domains, or maybe move around depending on what happens within the conversation |
| | Discovery is more difficult |
| | Documentation becomes more fragmented |
| | Still not necessarily close to the code | 

---

### Option 4 - Stored in Github - written in Markup, stored in the service repository

This option is the same as options 2 and 3, but the document is stored next in the service's repository itself, perhaps in a directory such as `docs`. 


| *Pros* | *Cons* | 
| --- | --- |
| Close to the code it talks to | Much harder discovery - if searching for prior art on a decision, you need to know which repo to go to |
| Fine grained access control | Some decisions may cross service boundaries, so then which repo does it go in? |
| | Documentation becomes fragmented across lots of repos | 

---
# Outcome

Attendees: List of those at the meeting including who they represent.
Apologies: List of those who could not make it.

Once the ACR has concluded, in addition to updating the summary with the decision, outline which decision was chosen and why.

Include any acknowledge consequences and/or risk mitigation steps. This should include an assessment of impact on system health.
