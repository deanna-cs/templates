# Changelog Template Guide - Rob

## Disclaimer

**NOTE**: Leaving this section in for now. Eventually, the project will decide how/if to include this language on future templates.

The target audience for this version of the Changelog Template Guide - and the accompanying Changelog Template - is the Open Source Software (OSS) domain. However, closed source or proprietary software environments can also use these documents, either as is or with modifications based on need. The end users referred to in this document, and the accompanying template, may belong to one of the following groups:

- Internal developers and team members of the OSS organizations.
- External developers and team members of the OSS user community who use existing codebase.

## What is a Changelog, and what's its purpose?

A changelog is a reverse-chronological, comprehensive listing of all significant and noteworthy changes to a software or technology project's versioned release from the initial release to its current state. In other words, they keep track of all technology-related changes to a software application. 

Created to help software developers and open source contributors track all significant codebase changes between releases. It lets the developers know what changed, when it changed, and whom, providing a context for past changes and decisions.

Changelog history can offer a view into the direction and progression of the project and the software product, help visualize team's progression towards implementing new functionality that benefits end users, and guides them towards creating and implementing functionality that benefit the users and follow coding practices and tools consistent with the company's vision and goals, and can make corrections, if needed.

## What information do they contain?

**NOTE**: we might find duplicate content related to this section. **Deanna**

Changelogs currently do not have a formal standard or format in the OSS domain, however, there are recommended approaches for content, formatting, cadence, and consistency. These include:

- Version number for the release
  - [Semantic Versioning](https://semver.org/)

- Date Format
  - [ISO 8601 Standard](https://www.iso.org/iso-8601-date-and-time-format.html)

- Types of changes
  - Added, changed, deprecated, removed, fixed, etc. **NOTE**: Might link out to GitHub docs?
**Deanna**. [GitHub Docs](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases)

- Who made them and Why
  - Dev name, email

- Links to additional relevant details
  - Specific issues, feature requests, Git tag, issue number, etc.

---

## Reasons to use Changelogs

---

Changelogs can help various groups within the OSS environment work more efficiently by providing software-related application changes and other technical information in a single up to date document delivered with each software release or patch update. There are several groups of software development team who benefit from a changelog. These include internal OSS developers, OSS contributors and co-developers worldwide, QA, software designers, system architects, and other technical team members and individuals.

Changelogs can help developers quickly resolve application issues and bugs by reviewing changelogs, identifying a specific change that likely introduced the bug, and quickly fixing, testing, and updating the codebase. They may also be able to focus on specific changes that might have caused the issue by reviewing changes to the codebase. Without this level of backward-looking information, the identification and correction of software issues, including bug fixing, could take longer, leading to code inconsistencies that could result in lower customer satisfaction with the product.

Changelogs are an excellent communication tool between OSS development teams, the larger OSS development community and co-developers, and other technical folks worldwide. Changelogs are one of the handfuls of documents that keeps these community members up to date with software changes and allows them to confidently make consistent application changes. Without these technical docs, there would be lots of miscommunication, loss of productivity, and general loss of confidence and product engagement. **REVIEW** Understanding what is at risk, the time and effort spent maintaining an up to date changelog seems to be relatively insignificant.

Changelogs are a good tool to provide actionable metrics and insights into the software product through the collection of bugs-to-feature ratios, which can help in strategic planning and having a positive impact on the business. These metrics can help decide if the team should focus on new features and functionality, or concentrate on learning and updating tool sets in designing and creating bug-free code. In the absence of these or similar metrics, business processes or practices might not be corrected leading to potential negative consequences.

They can also be an helpful adjunct resource in the QA/QC process by providing additional details for changes to the software in the context of why, when, and who.

Changelogs are a good source to help in tracking and eliminating conceptual inconsistencies in the codebase that may arise due to a quick fix or a change that might have missed the QA process, or a test case, by going back in time and identifying when a specific change causing the inconsistency was made, by whom, and the context for the change. Inconsistent development concepts in an application can lead to performance issues that can be difficult to identify and resolve that could lead to an inefficient and ineffective product or design.

Changelogs track and report on all notable software changes, including additions, deletions, new features, feature enhancements, deprecations, security-related updates, etc., for each release in one easily accessible document. Clearly formatted and consistently created changelogs can help build confidence in the product among the development community. This 

the OSS developers, software engineers, and the larger open source development community build confidence in the authenticity of the information contained in the changelogs can make changes to their software confidently. Developers can also understand why a particular change was made, who made it, and why, understanding which parts of the software other team members are working on, and the overall software product progression and direction. Developers can see software change history in one document located in a central place. Without this document, developers could waste looking through various technical documents, source code, comments, or commit messages to understand what changed, why it changed, and how to alter the software at their end to account for the software change. Also, developers using OSS applications don't have access to a traditional help-desk to answer their technical questions and other technical issues, so a changelog is their main source of all things technical.

Changelogs can also help someone re-learn and understand code logic and onboard new developers to the project. They can also increase developer buy-in and commitment to OSS projects by highlighting the developers' names who contributed to making significant and noteworthy software changes and updates.

Changelogs can keep product users in the loop, engaged, and excited about changes and the updates that can help them perform their functions more effectively and efficiently, which leads to product loyalty and use. Power users are another group of users who read Changelogs and are keen to learn of new changes and how they help the product grow. They can influence the product choice, selection, and evaluation criteria by sharing their experience with the product, accurate and timely documentation, including Changelogs, and the company's commitment to its products. Changelogs and also attract future customers and employees through social media and other industry-specific organizations and conferences. Up to date project documentation, including Changelogs, can increase the adoption of new development standards and tools and build developer loyalty through empowerment and a sense of ownership of the end product. Without providing accurate documentation on a consistent basis, engaging with the customers through documentation in an OSS environment can lead to negative consequences.

## Changelogs vs. Release Notes

**NOTE**: What can really help to emphasize the differences between release notes and changelogs: some examples of language. Slack has funny release notes, maybe Microsoft Word? - **Deanna**

As both changelogs and release notes reflect changes to a software application in the OSS domain and are sometimes referred to as "Change Documents". Although sometimes referred to interchangeably, there are key differences between them, not least being their audience.

Changelogs are developer-centric and are written in a technical language. It's content is focused on technical changes to the software - who made the change, why it was made, and the context for the change. It links to specific issues or bugs that were the cause for the change and lists and groups these changes in specific headings and titles to help other developers understand the overall changes in a consistent format. It is a time-based record of all software changes since the first release of the product. They can be used internally or externally.

Release notes on the other hand, are end user-focused and emphasize software changes in that context. They inform the users in plain, concise, and jargon-free language of the changes and highlight how these changes will help the users perform their tasks more efficiently. Release notes can be both internal and external.

## What are the guiding principles for creating Changelogs?

Changelogs are meant for humans to read and interpret and, therefore, should be in human-readable text. It should communicate the technical change, such as bug fixes, new/updated features, deprecation, removal, security updates, etc., who made them, and its context, the why. Changelog contents should be sorted by importance; more critical changes on top followed by less important ones. Changes that are less important or noteworthy, such as code refactoring and efficiency, should not be included. Each change entry should provide a link to additional details and information, such as git commits, issue number/tracker, etc. Changelog publishing cadence should ideally coincide with each software release or patch update. Create an "Unreleased" section at the top of the changelog file to track current release work and change the unreleased tag with the next release date and version when ready to publish. As in all documentation, it is good practice to review the changelog file for accuracy and completeness before publishing.

## Why (or when) not to use a changelog?

**NOTE**: **Really** make sure that we highlight that changelogs are very technical and aimed for technical users

**NOTE**: We could remove this section and incorporate it into the early parts of the document where we describe what changelogs are

A changelog may not be the best tool for end user communication in a traditional a recommended document to share with traditional software application end users for the below reasons:

- Changelog language and details are technical by definition and thus may not be quite as beneficial as release notes for non-technical application end users.
- It may be difficult for non-technical end users, should they be expected to understand and implement application-level changes or incorporate new changes into their workflow, and may discourage user engagement with the software.

## Who writes (or creates) Changelogs?

TODO: finalize below verbiage.

- Changelogs are generally created and maintained by the software developers as they have the most **current knowledge of what changed** (functions, methods, etc.) why it changed (CR, TR, RFC, etc.), and when it changed (date, release number, etc.) and who made the change (name, email).
- It can also be written by other technical team members, such as architects, project managers, software designers, tech writers/documentation team, etc.

## Who benefits from a changelog and what are the benefits?

**NOTE:** See “What are the benefits and uses of Changelogs, Why create them, and Who can benefit from them” in above sections.

## Who uses changelogs and how is it used?

**NOTE:** See “What are the benefits and uses of Changelogs, Why create them, and Who can benefit from them” in above sections.

## Who/What: Negative impacts of not maintaining well-formatted and up to date changelogs?

**NOTE:** We can fold this into benefits section - **Deanna**

- End users (OSS devs and co-devs) not aware of deprecations, removals, and security updates.
- End users in the dark about bug fixes, new features, and other updates.
- Risks of mistakes and misunderstandings.
- Productivity and collaboration issues and confusion among project team and OSS development community
Loss of credibility for the company.
- Versioning conflicts .
- Security issues.
- Compliance issues.
- Customer & shareholder relationships are negatively impacted.

## Where will users find the changelog?

- Blog posts; as Markdown (.md) files in a github repo; changelog section of a software or its website; on “what’s new” in android and apple apps stores.

## File names

- Changelog Names: Changelog, CHANGELOG.md, CHANGES.md, HISTORY.txt, NEWS.txt, etc.

## Format

No standard or formal format as of the writing of this doc.Some good advice on:

- What a format should be?
  - For version #, use Semantic Versioning.
  - For date, use ISO date format.
  - Include name and email of the dev.
  - Include reason for change.
  - Use links for additional info related to a change, such as git commit, issue #, etc.
- What should be included?
  - Types of changes: bug fixes, additions, new features, deprecations, removals, security changes.
- What types of tags to use?
  - Added, Changed, Deprecated, Security, etc.
  - Combine similar changes under one tag.

## When is a changelog created?

- Changelog is a historical file and is recommended to be continuously updated during software development up until the code is ready to be deployed in a new release.

## When will the changelog be available to the end users?

- Changelog cadence should coincide with each new software release.
