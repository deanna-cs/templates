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