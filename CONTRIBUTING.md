# Contributing to openXeco book

Most of openXeco's documentation pages are stored as plain text files in this dedicated openxeco-book repository.
OpenXeco book is generic documentation for openXeco including usage, API documentation, best practices, and specific configuration settings.
TODO: Add install guide reference
By cloning and regularly pulling from this repo, users can maintain their own up-to-date offline copy of openXeco documentation rather than relying solely on the web.

OpenXeco book is generated in HTML, PDF, epub, and mobi using [Honkit](https://github.com/honkit/honkit), which is a framework to write documentation in Markdown format.
The documentation is published on [book.openxeco.org](https://www.openxeco.org/).

## Documentation guidelines

The documentation is a community effort. Volunteers work hard trying to keep everything accurate and comprehensive.
If you notice a problem or some way it can be improved, please edit the documentation.

All pull requests against openXeco must pass review before being merged.
This process is designed to ensure that contributed text is accurate and non-malicious.
Once a pull request passes review, the documentation maintainer then verifies that the pull request is mechanically sound (no merge conflicts or broken links).
If so, the documentation maintainer then merges the pull request.

If you have a question about something you read in the documentation you can [open an issue](https://github.com/CybersecurityLuxembourg/openxeco-book/issues) for it.
If you see that something in the documentation should be fixed or improved, please [contribute the change](#how-to-make-a-contributution) yourself. 

## How to make a contribution

Editing the documentation is easy, so if you see that a change should be made, please contribute it!

A few notes before we get started:

- Every documentation change will be reviewed before it’s accepted. This allows us to maintain quality control and protect our users.
- If your contribution would take a lot of time, please [file an issue](https://github.com/CybersecurityLuxembourg/openxeco-book/issues) for it first so that we can make sure we’re on the same page before significant work begins. This ensures you do not spend time and effort on a contribution that we can’t accept. 

Thanks to GitHub’s interface, you can edit openXeco's documentation even if you don’t know git at all. 
All you need to do to contribute is to [fork and clone](https://guides.github.com/activities/forking/) the [openxeco-book repo](https://github.com/CybersecurityLuxembourg/openxeco-book/), make your changes, then [submit a pull request](https://help.github.com/articles/using-pull-requests/)). 
You can also [open issues](https://github.com/CybersecurityLuxembourg/openxeco-book/issues) if you find any errors or propose changes.

[GitHub workflows](https://docs.github.com/en/actions/using-workflows) (used for automatic integration) is included in openxeco-book and the book generation is tested at each commit. 
When you make a pull request, verify if your changes affect the result of the tests. 
If the checks fail, review the output at Travis and make fixes where possible. 

### For native English speakers

Most openXeco developers are not native English speakers so you're more than welcome to correct or improve our English. 
For this, you can either submit a pull request or use another way that suits you better to share your improvements with us.

## Organizational guidelines

- Do not duplicate documentation. Duplicating documentation is almost always a bad idea. There are many reasons for this. The main one is that almost all documentation has to be updated at some point. When similar documentation appears in more than one place, it is very easy for it to get updated in one place but not the others (perhaps because the person updating it doesn’t realize it’s in more than one place). Such traps are often more harmful than if the documentation never existed in the first place. The solution is to link to existing documentation rather than duplicating it. There are some exceptions to this policy (e.g., information that is certain not to change for a very long time), but they are rare.
- We maintain only one set of documentation for openXeco. We do not maintain a different set of documentation for each version of openXeco. Our single set of openXeco documentation is updated on a continual, rolling basis. Our first priority is to document all current, stable releases of openXeco. Our second priority is to document the next, upcoming release (if any) that is currently in the beta or release candidate stage.
- Instructions on how to install openXeco are held in TODO.

## Style guidelines

- Familiarize yourself with the terms defined in the [glossary](https://book.openxeco.org/GLOSSARY.html). Use these terms consistently and accurately throughout your writing.
- The language in this book is American English. All the screenshots and examples are in English.

## Markdown conventions

All the documentation is written in Markdown for maximum accessibility. When making contributions, please try to observe the following style conventions:

- Use spaces instead of tabs.
- To enable offline browsing, always use relative (rather than absolute) links, e.g., openxeco/automation/ instead of https://book.openxeco.org/automation/. Examples of exceptions:
    - URLs that appear inside code blocks (e.g., in comments and code snippets)
    - Files like README.md and CONTRIBUTING.md
- Insert a newline at, and only at, the end of each sentence. This practice results in one sentence per line, which is most appropriate for sources that consist primarily of natural language text. It results in the most useful diffs and facilitates translation into other languages while mostly preserving source readability.
- If appropriate, make numerals in numbered lists match between Markdown source and HTML output. If a user is required to read the Markdown source directly, this will make it easier to follow, e.g., numbered steps in a set of instructions.
- Use Atx-style headings: `# h1`, `## h2`, `### h3`, etc.
- When writing code blocks, use syntax highlighting where possible and use [...] for anything omitted.
([This](https://daringfireball.net/projects/markdown/) is a great source for learning about Markdown.)

## Git conventions

Please try to write good commit messages, according to the [gitchangelog guidelines](https://github.com/vaab/gitchangelog/blob/master/src/gitchangelog/gitchangelog.rc.reference)
