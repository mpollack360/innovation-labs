<!-- TOC -->

- [1. Innovation Labs](#1-innovation-labs)
- [2. Version Control](#2-version-control)
  - [2.1. Branches](#21-branches)
  - [2.2. Commits](#22-commits)
    - [2.2.1. Use the Imperative](#221-use-the-imperative)
    - [2.2.2. Use the Body to Explain the Background and Reasoning, not the Implementation](#222-use-the-body-to-explain-the-background-and-reasoning-not-the-implementation)
    - [2.2.3. Subject Line Standard Terminology](#223-subject-line-standard-terminology)
  - [2.3. Documentation](#23-documentation)
  - [2.4. Pull Requests](#24-pull-requests)
  - [2.5. Deploy](#25-deploy)
- [3. Done](#3-done)

<!-- /TOC -->

# 1. Innovation Labs
<a id="markdown-innovation-labs" name="innovation-labs"></a>
The Innovation Lab is the opportunity for OCI to showcase our collective capabilities in solving business problems using technology in new and innovative ways. These demonstrations will be installed in the office to allow those visiting the OCI office to explore our solutions.

More information on Innovation Labs can be found in the [Project.Innovation Labs](https://drive.google.com/drive/u/2/folders/0AK8RZHbfxVSqUk9PVA) shared Google Drive

# 2. Version Control
<a id="markdown-version-control" name="version-control"></a>
Innovation Lab projects use a [trunk based development](https://trunkbaseddevelopment.com/) branching strategy.

[Trunk-based Development vs. Git Flow](https://www.toptal.com/software/trunk-based-development-git-flow)

## Branches
<a id="markdown-branches" name="branches"></a>
Branch names must be in [kebab-case](https://en.toolpage.org/tool/kebabcase).

## Commits
<a id="markdown-commits" name="commits"></a>
Innovation Lab projects use the [conventional commit](https://www.conventionalcommits.org/en/v1.0.0-beta.4/) specification for commits.

https://github.com/talos-systems/conform

### Use the Imperative
<a id="markdown-use-the-imperative" name="use-the-imperative"></a>

In keeping with the standard output of git itself, all commit subject lines must be written using the imperative:

Your commit subject line must be able to complete the sentence 

> If applied, this commit will ...

If it doesn't, it's non-conformant. The body may use any style you want. 

### Use the Body to Explain the Background and Reasoning, not the Implementation
<a id="markdown-use-the-body-to-explain-the-background-and-reasoning-not-the-implementation" name="use-the-body-to-explain-the-background-and-reasoning-not-the-implementation"></a>

*Especially* if the diff is rather large or extremely clustered, you can save all fellow developers some time by explaining *why* you did *what*.

When possible the addition of screenshots, recorded gifs or other visual media is recommended.

### Subject Line Standard Terminology
<a id="markdown-subject-line-standard-terminology" name="subject-line-standard-terminology"></a>

First Word | Meaning
--- | --
Add | Create a capability e.g. feature, test, dependency.
Cut | Remove a capability e.g. feature, test, dependency.
Fix | Fix an issue e.g. bug, typo, accident, misstatement.
Bump | Increase the version of something e.g. dependency.
Make | Change the build process, or tooling, or infra.
Start | Begin doing something; e.g. create a feature flag.
Stop | End doing something; e.g. remove a feature flag.
Refactor | A code change that MUST be just a refactoring.
Reformat | Refactor of formatting, e.g. omit whitespace.
Optimize | Refactor of performance, e.g. speed up code.
Document | Refactor of documentation, e.g. help files.

## 2.3. Documentation
<a id="markdown-documentation" name="documentation"></a>
In cases where the impact of a change is such that it is affects a fundamental component of the system additional documentation is needed above what is presented in commit messages. This is by discretion, but it is advised to err on the side of more documentation than less.

## 2.4. Pull Requests
<a id="markdown-pull-requests" name="pull-requests"></a>

Pull requests require a minimum of one reviewer to accept changes prior to merge. It is the responsibility of the person submitting the pull request to schedule a code review.

[Google Engineering - Code Review Developer Guide](https://google.github.io/eng-practices/review/)

## 2.5. Deploy
<a id="markdown-deploy" name="deploy"></a>

Once a pull request is merged the changed will be automatically deployed to the appropriate environment.

# 3. Done
<a id="markdown-done" name="done"></a>
A task is complete when
- All acceptance criteria have been met
- Implementation has been code reviewed
- All automated tests pass (e.g: Unit, end-to-end testing)
- All manual tests pass (e.g: Functional, user interface testing)
- Necessary documentation is reviewed
- Implementation is deployed to the appropriate environment

