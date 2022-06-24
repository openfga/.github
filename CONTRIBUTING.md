# Contributing to OpenFGA

It takes a lot of work from a lot of people to build a great authorization system. This document provides an outline for interacting with the OpenFGA community and its governance structure, as well as the nitty-gritty details how to write, test, and submit code changes. If you run into any trouble, email us at [community@openfga.dev](mailto:community@openfga.dev) or ask for help in our [Discord][discord] community.

## Contribution process

OpenFGA welcomes feedback and contributions from anyone who might be interested in helping the project.

The [core team](https://github.com/orgs/openfga/teams/core) is here to help. This is the group of people responsible for organizing the backlog of [issues](https://github.com/openfga/openfga/issues), reviewing [pull requests](https://github.com/openfga/openfga/pulls), and all code within this repository. The core team is working to keep the OpenFGA product aligned with its [design principles](https://github.com/openfga/rfcs/blob/main/DESIGN_PRINCIPLES.md), and to make it easy for anyone to take part in building and shaping OpenFGA's development and roadmap.

If you are planning to implement a new feature, you may want to submit an [RFC](https://github.com/openfga/rfcs/) first - it's not necessary for every change, but requesting feedback early can help save time and effort. See ["When the RFC process is necessary"](https://github.com/openfga/rfcs#when-the-rfc-process-is-necessary) for more information.

The rest of this document describes how to contribute code, but there are many other ways to contribute that are incredibly helpful: helping others in Discussions and Discord, providing feedback on RFCs and releases, triaging Issues, improving the documentation - any little bit helps.

## Commits

Check out the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) website to get ideas about how an ideal commit should be structured: 

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

The commit contains the following structural elements, to communicate intent to the consumers of your library:

1. fix: a commit of the type fix patches a bug in your codebase (this correlates with PATCH in Semantic Versioning).

1. feat: a commit of the type feat introduces a new feature to the codebase (this correlates with MINOR in Semantic Versioning).

1. BREAKING CHANGE: a commit that has a footer BREAKING CHANGE:, or appends a ! after the type/scope, introduces a breaking API change (correlating with MAJOR in Semantic Versioning). A BREAKING CHANGE can be part of commits of any type.

1. types other than fix: and feat: are allowed, for example @commitlint/config-conventional (based on the the Angular convention) recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.

1. footers other than BREAKING CHANGE: <description> may be provided and follow a convention similar to git trailer format.

## Pull request requirements

When you're ready, submit a pull request!

* As with any community interaction, you must follow the [Code of Conduct](./CODE_OF_CONDUCT.md).

* All changes must have adequate test coverage. For instruction on writing and running the various test suites, see Testing your changes.

* If relevant, add a changelog entry.

* All contributors should sign the [Contributor License Agreement](https://cla-assistant.io/okta/). If you haven't signed it, you'll get prompted to sign it the first time you submit a Pull Request.

* The documentation should be updated (in a separate, linked PR), but if you're not confident in your technical writing you may skip this step.

* All changes are required to be [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0) Licensed.

* Dependencies & sub dependencies have to have compatible licenses. The existing repositories have [FOSSA checks](https://fossa.com/) integrated as part of their Github Actions CI/CD workflow. New repositories will need to have similar checks in place.

* New contributions have to pass several security tests. The existing repositories have [Snyk](https://snyk.io/) and [Semgrep](https://semgrep.dev/) integrated as part of their Github Actions CI/CD workflow. New repositories will need to have similar checks in place.

* Contributions should introduce minimal to no dependencies. This helps with maintenance as well as security and legal considerations.

### Structure and Behaviour

In an ideal world, every pull request is small, but the codebase is large and sometimes complex changes cannot be avoided. To ease PR reviews, there are a few practices we've found helpful:

* Focus your commits so that they only change a single component at a time.

* Isolate [structure changes from behaviour changes][sb-changes] and label the commits appropriately - even better, batch commits of the same type into contiguous blocks.

* Give clear prose justifications for your changes in the commit messages - it's not unusual that you do some digging to uncover the motivation for a change, but if you don't mention it in the commit message the diff can feel pretty opaque.

[coc]: [https://github.com/openfga/openfga/CODE_OF_CONDUCT.md]
[discord]: [https://discord.com/invite/pvbNmqC]
