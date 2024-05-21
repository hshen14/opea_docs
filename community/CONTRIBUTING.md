Contribution Guidelines
=======================

Thanks for considering contributing to OPEA project. The contribution process is similar with other open source projects on Github, involving an amount of open discussion in issues and feature requests between the maintainers, contributors and users.


# Table of Contents

<!-- toc -->

- [All The Ways to Contribute](#all-the-ways-to-contribute)
  - [Community Discussions](#community-discussions)
  - [Documentations](#documentations)
  - [Reporting Issues](#reporting-issues)
  - [Proposing New Features](#proposing-new-features)
  - [Submitting Pull Requests](#submitting-pull-requests)
    - [Create Pull Request](#create-pull-request)
    - [Pull Request Checklist](#pull-request-checklist)
    - [Pull Request Template](#pull-request-template)
    - [Pull Request Acceptance Criteria](#pull-request-acceptance-criteria)
    - [Pull Request Status Checks Overview](#pull-request-status-checks-overview)
- [Support](#support)
- [Contributor Covenant Code of Conduct](#contributor-covenant-code-of-conduct)

<!-- tocstop -->

# All The Ways To Contribute

## Community Discussions

OPEA users are encouraged in participating open discussions in [X/Twitter](https://twitter.com/opeadev) or mail to [info@opea.dev](mailto:info@opea.dev) to get latest updates about OPEA project. 

## Documentations

The quality of OPEA project's documentation can have a huge impact on its success. We reply on OPEA maintainers and contributors to build clear, detailed and update-to-date documentation for user.

## Reporting Issues

If OPEA user runs into some unexpected behavior, reporting the issue to the `Issues` page under the corresponding github project is the proper way to do. Please ensure there is no similar one already existing on the issue list). Please follow the Bug Report template and supply as much information as you can, and any additional insights you might have. It's helpful if the issue submitter can narrow down the problematic behavior to a minimal reproducible test case.

## Proposing New Features

OPEA communities use the RFC (request for comments) process for collaborating on substantial changes to OPEA projects. The RFC process allows the contributors to collaborate during the design process, providing clarity and validation before jumping to implementation.

*When the RFC process is needed?*

The RFC process is necessary for changes which have a substantial impact on end users, workflow, or user facing API. It generally includes:

- Changes to core workflow.
- Changes with significant architectural implications.
- changes which modify or introduce user facing interfaces.

It is not necessary for changes like:

- Bug fixes and optimizations with no semantic change.
- Small features which doesn't involve workflow or interface change, and only impact a narrow use case.

#### Step-by-Step guidelines

- Follow the [RFC Template](./rfc_template.md) to propose your idea.
- Submit the proposal to the `Issues` page of the corresponding OPEA github repository.
- Reach out to your RFC's assignee if you need any help with the RFC process.
- Amend your proposal in response to reviewer's feedback.

## Submitting Pull Requests

### Create Pull Request

If you have improvements to OPEA projects, send your pull requests to each project for review.
If you are new to GitHub, view the pull request [How To](https://help.github.com/articles/using-pull-requests/).

#### Step-by-Step guidelines

- Fork the corresponding OPEA repository using the button `Fork` in the top right corner.
- Clone your forked repository to your pc by running `git clone "url to your repo"`
- Create a new branch for your modifications by running `git checkout -b new-branch`
- Add your files with `git add -A`, commit `git commit -s -m "This is my commit message"` and push `git push origin new-branch`.
- Create a `pull request` for the project you want to contribute.

### Pull Request Checklist

Before sending your pull requests, follow the information below:

- Add unit tests to cover the code you would like to contribute.
- Follow [Developer Certificate of Origin](https://en.wikipedia.org/wiki/Developer_Certificate_of_Origin) to comply with the terms of Developer Certificate of Origin by signing off each of your commits with `-s`, e.g. `git commit -s -m 'This is my commit message'`.

### Pull Request Template

See [PR template](./pull_request_template.md)

### Pull Request Acceptance Criteria

- At least two approvals from reviewers

- All CICD tests passed

- All conversations solved

- License compatible with existing one

### Pull Request Status Checks Overview

The OPEA project use GitHub Action for CICD test.

| Test Name                           | Test Scope                                      | Test Pass Criteria |
|-------------------------------------|-------------------------------------------------|--------------------|
| [DCO](https://github.com/apps/dco/) | Use `git commit -s` to sign off                 | PASS               |
| Code Format Scan                    | pre-commit.ci [Bot]                             | PASS               |
| Code Security Scan                  | Bandit/Hadolint/Dependabot/Coverity/McAfee      | PASS               |
| Unit Test                           | Pytest scripts under tests folder               | PASS               |
| End to End Test                     | End to end tests, for example GenAI Examples    | PASS               |

# Support

Feel free to reach out to [OPEA maintainers](mailto: info@opea.dev) for support.

# Contributor Covenant Code of Conduct

This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant Code of Conduct](./CODE_OF_CONDUCT.md).