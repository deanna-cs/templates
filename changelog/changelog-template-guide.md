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

### Highlights

TODO add some content here

### Upcoming

TODO add some content here

### Deprecation

TODO add some content here

As you build your changelog, you'll need to decide what sections your changelog must have. If you're in the early stages of working on your software project, you might need an "added", "changed", and "fixed" section to start. As your project evolves, you can add other sections, like "deprecated" or "migrations." 

## Guiding principles for changelogs 

There are several principles to follow as you develop a changelog for your software project. TODO better intro text 

### Write changelog entries that answer the "why"

TODO You shouldn't say what you did, but *why* you did it. Instead of saying, "We implemented this function through using this library, etc etc, say something like, "Improved process of something to better do thing."

NOTE Understanding the context of the change -> important

NOTE This might be a manual process? If you're using automation would it pull in the name of the PR or the last commit before the changelog was generated? hmmm

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

If you don't use semantic versioning for your software project, it is recommended that you do. However, not all projects are the same. If your project uses a different convention for indicating software versions, it is important to highlight this information somewhere in the changelog or in a README file.

NOTE Whatever scheme you use for your versioning, be consistent in it; don't change when you feel like it

### Document changes that impact end users

TODO Telling your users that you switched SSGs doesn't impact them; breaking changes to your API does. 

## Changelog automation

TODO It's the best