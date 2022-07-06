# Changelog Template Guide - Rob

## What is a Changelog?

A changelog is a reverse-chronological, comprehensive listing of all significant and noteworthy changes to a software project from the initial release to its current version. Simply put, changelogs keep track of all technology-related changes to a software application.

Its primary purpose is to record important codebase changes and updates in a single document in a format and language that is valuable to the development teams, especially developers, to have an accurate and reliable history of the application changes from its origin to its current state.

Its value in an OSS environment is considerably more significant due to the reuse, enhancement, and redistribution of the open source application by developers worldwide.

## Benefits of using Changelogs

Changelogs can help various groups within the OSS environment work efficiently by documenting notable software and related application changes and other technical information in a single up to date document delivered with each software release or patch update. These include internal OSS developers, OSS contributors and co-developers worldwide, QA engineers, software designers, system architects, and other technical team members and individuals.

Changelogs can help developers resolve application issues and bugs quickly by reviewing changelogs, identifying specific change(s) that likely introduced the bug, and quickly fixing, testing, and updating the codebase. Developers can understand why a particular change was made, who made it and why, which parts of the software other team members are working on, and the overall software product progression and direction. Developers can see software change history in one document located in a central place. Without this information available in on place consistently, developers could end up spending time looking through various technical documents, source code, comments, or commit messages to understand what changed, why it changed, and how to confidently change their software to account for the change. Additionally, developers using OSS applications don't have access to a traditional help desk to answer technical questions and offer guidance, so a changelog is their main source of all the changes to the application.

Changelogs track and report on such changes as deletions, new features, feature enhancements, deprecations, security-related updates, etc., for each release in one easily accessible document. The absence of specific change information could result in confusion, software issues and bugs, general uncertainty, and loss of collaboration and teamwork for the developers and development teams. Inconsistently maintained or published changelogs can also lead to compliance issues and negatively impact customer and shareholder relationships.

Without this level of backward-looking information, identification and correction of software issues could take longer, leading to code inconsistencies and product degradation that could result in lower customer satisfaction with the product.

Well-maintained changelogs can offer developers a view of the direction and progression of the project and product progression. It can help visualize the team's progress towards implementing new functionalities that benefit end users and guide them towards creating and implementing functionality that benefits the users, as well as following coding practices and tools consistent with the company's vision and goals.

Changelogs are an excellent communication tool between the OSS development teams, the larger OSS development community and co-developers, and other technical folks worldwide. A changelog keeps open source community members up to date with software changes. A clearly formatted and consistently created changelogs can help build confidence in the product among the development community and allows them to make quality product improvements.

Changelogs are a valuable tool in collecting actionable metrics and insights into the software product through the collection of bugs-to-feature ratios. This can help in strategic planning and possibly have a positive business impact by determining whether the team should focus on new features and functionality or on creating bug-free code by focusing on software design and updating development toolsets. Without these or similar metrics, sub-optimal development processes or practices might not be identified and corrected, leading to potential negative business consequences.

They can also be a helpful adjunct resource in the QA/QC process by providing additional details for changes to the software in the context of why, when, and who.

Changelogs are a good source to help track and eliminate conceptual inconsistencies in the codebase arising due to quick fixes or changes that might have missed the QA process or a test case. Going back in time and identifying when a specific change causing the codebase inconsistency was made, by whom, and the context for the change can help resolve code inconsistencies. Conflicting development concepts in an application can lead to performance issues that can be difficult to identify and resolve and might lead to an inefficient and ineffective product or design.

Changelogs can also help someone re-learn and understand code logic and onboard new developers to the project. They can also increase developer buy-in and commitment to OSS projects by highlighting the developers' names who contributed to making significant and noteworthy software changes and updates.

Changelogs can keep product users engaged and excited about changes and the updates that can help them perform their functions more effectively and efficiently, leading to product loyalty and use. Power users are another group who read changelogs and are eager to learn about new changes that may help product growth. They can influence product choice, selection, and evaluation criteria by sharing their experience with the product and accurate and timely documentation, including changelogs and other technical documentation. 

Well-maintained and consistently delivered changelogs can attract future customers and employees through social media and other industry-specific organizations and conferences. Up to date project documentation, including changelogs, can increase the adoption of new development standards and tools and build developer loyalty through empowerment and a sense of ownership of the end product. Engaging with customers in an OSS environment can lead to negative consequences without consistent and accurate documentation.

## Changelogs vs. Release Notes

**NOTE**: What can really help to emphasize the differences between release notes and changelogs: some examples of language. Slack has funny release notes, maybe Microsoft Word? - **Deanna**

As both changelogs and release notes reflect changes to a software application in the OSS domain, they are sometimes referred to as "Change Documents." Although sometimes referred to interchangeably, they are key differences, not least being their audience.

Changelogs are developer-centric and are written in a technical language. Its content is focused on technical changes to the software - who made the change, why it was made, and the context for the change. It links to specific issues or bugs that were the cause of the change and lists and groups these changes in specific headings and titles to help other developers understand the overall changes in a consistent format. It may include code snippets to elaborate changes. It is a time-based record of all software changes since the product's first release. They can be used internally or externally.

Release notes, on the other hand, are end-user-focused and emphasize software changes in that context. They inform the users in plain, concise, and jargon-free language of the changes and highlight how they will help them perform their work more efficiently. Release notes can be both internal and external.

## What are the guiding principles for creating Changelogs?

Changelogs are meant for humans to read and interpret and, therefore, should be in human-readable text. It should communicate the technical change, such as bug fixes, new/updated features, deprecation, removal, security updates, etc., who made them, and its context, the why. Changelog contents should be sorted by importance; more critical changes on top followed by less important ones. Changes that are less important or noteworthy, such as code refactoring and efficiency, should not be included. Each change entry should link to additional details and information, such as git commits, issue number/tracker, etc. Changelog publishing cadence should ideally coincide with each software release or patch update. It is recommended to create an "Unreleased" section at the top of the changelog file to track current release work and change the unreleased tag with the next release date and version when ready to publish.

## Who should create Changelogs?

Individual software developers who make the changes and updates are best positioned to update a changelog when the software is changed. When the software is ready to be released, the development team lead or the designee can verify and confirm the changelog information for accuracy before publishing.

Other development team members can also be responsible for maintaining, updating, verifying, and publishing the changelog by collaborating with the developers for each release cycle.

# How to write good changelogs 

Writing a good changelog starts with identifying your audience. You may need to create a changelog for an internal audience, like project stakeholders or engineering staff members. Alternatively, you might need a changelog for an external audience, like customers involved with testing your product or end users. Before you create your changelog, you must think about who your audience is and what their needs are. 

But you must remember the one thing both audiences have in common: they both want to know *what's* changed, *why* it changed, and *how* the changes impacts them. The content you include in your changelog can help them find that information.

## What should changelogs include?

Changelogs should include a reverse-chronologically ordered list of changes you make to your software project. The structure of a changelog can vary from project to project, but at bare minimum, they contain the following sections:

* Added: for new features
* Changed: for changes in any existing functionality 
* Fixed: for any bug fixes

Changelogs can also include other information, such as:

* Highlights
* Upcoming
* Any deprecated features
* Resolved security vulnerabilities
* Previously supported integrations 
* Breaking changes
* Migrations

As you build your changelog, you'll need to decide what sections your changelog must have. If you're in the early stages of working on your software project, you might need an "added", "changed", and "fixed" section to start. As your project evolves, you can add other sections, like "deprecated" or "migrations."

### Highlights

If there is any important information you want to call out for your users, do that here. Some use cases for this section might include calling out any breaking changes or deprecated features. For example, if you're going to deprecate a highly-used feature in an upcoming release, you might want to call that out here. 

### Upcoming

Adding a "Upcoming" section to your changelog template is a great way to let your users know about features coming down the pipeline. For example, if your users have been requesting a particular feature for some time—and if the engineering team has started work on it–you can add that feature to this section. It's also a great way to show your end users that you listen to their feedback and seek to find ways to implement features that meet their needs.

### Deprecation

Features that were deprecated for a release can be added to this section. You may also want to add a brief explanation of why the feature was deprecated and also, recommended alternative methods or features to use instead.

## Guiding principles for changelogs 

There are several principles to follow as you develop a changelog for your software project.

### Write changelog entries that answer the "why"

When writing changelogs, you shouldn't only say what you did—you should explain *why* you dod it. For example, rather than saying, "We implemented this function," explain why you implemented the function. A good template to use is "{Verb} + {Why}." A revised entry might be, "Implented function to improve application response times." 

Adding the "why" to your changelog entries helps your users to understand the context of the change. If you consistently indicate the benefits or improvements of the changes you make, your users will see that your team is user-focused and committed to improving their experience with your project.

### (Open source) Acknowledge your contributors

If your software project is an open source project, you likely have one, two, or perhaps a large number of people who contribute to your project. When creating your changelog for a release, consider giving credit to your project's contributors. 

If you use GitHub or GitLab for your open source project, you can tag them in the changelog itself, or you can include a link to the pull request they created:

```
## [1.2.0] - 2022-03-12

### Added
* Tutorial on using Python by @claudiogentry
* Implement new `get_personal_projects` function (#35484)
```

Alternatively, you can choose to add a section to your changelog that lists all of the contributors for a release.

```
## [1.2.0] - 2022-03-12

### Contributors - thank you
* @claudiogentry
* @bschmidt
* @thesophiewilliams
```

Crediting your contributors has several benefits:

1. It's the best, most visible way to acknowledge your contributors and thank them for their work. 
2. It can encourage first-time contributors, to your project or open source software in general, to continue contributing to the project. 
3. It can help to foster a healthy, open source community. 

### Use semantic versioning

Semantic versioning is the industry-standard way of communicating changes to a software project. The version format typically follows an X.Y.Z (Major.Minor.Patch) format, like 1.1.2. To indicate changes to your software project, you change the version number. For example, 1.1.3 indicates that a backwards-compatible bug fix was implemented for that particular release. 

If you don't use semantic versioning for your software project, it is recommended that you do. However, not all projects are the same. If your project uses a different convention for indicating software versions, it is important to highlight this information somewhere in the changelog or in a README file. Whatever schema you use, make sure to be consistent.

### Document changes that impact end users

Not everything needs to be included in your changelog. It's important to make sure that you only include changes that impact your end users, especially if your changelog is for them. New or deprecated features are especially important to document, as your end users are mostly likely to be interested in that information. 

If you find that your changelog has information for multiple audiences in one document, consider creating a changelog specifically for your end users and one for internal team members or internal stakeholders to keep your changelog focused.

## Changelog automation

There are two ways you can generate a changelog: through manually creating one or through using a tool that can generate a changelog from your commits. If you're interested in learning more about changelog automation, see the [changelog deep dive document](changelog-deep-dive-guide.md).