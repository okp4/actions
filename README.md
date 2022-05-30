# GitHub actions

> The repository of GitHub CI/CD workflows used @[okp4].

[![status](https://img.shields.io/github/workflow/status/okp4/actions/Lint?style=for-the-badge)](https://github.com/okp4/actions/actions/workflows/lint.yml) [![license](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg?style=for-the-badge)](https://opensource.org/licenses/BSD-3-Clause) [![conventional commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=for-the-badge)](https://conventionalcommits.org)

## 💡 Purpose

This is a collection of GitHub Actions that we use for our projects @[okp4] and that can be useful to others.

All the workflows and actions defined in this repository promotes the practices of CI (i.e. Continuous Integration) and CD (Continuous Deployment|Delivery) and enable the automation of operations that cover the following categories:

- Code quality
- Code review
- Dependency management
- Build
- Deployment
- Testing
- Publishing
- Utilities

## ⚙️ Workflows

The actions are organized arount serveral workflows, described hereafter.

### 💚 Lint

[workflows/lint.yml](src/.github/workflows/lint.yml)

Part of the code quality analysis, ensure the homogeneity of the codebase.

The workflow contains a large set of jobs to deal with different project typologies (technology, programming language...).

### 🧪 Test

[workflows/test.yml](src/.github/workflows/test.yml)

Executes the tests present in the codebase.

The workflow contains a large set of jobs to deal with different project typologies (technology, programming language...).

### 🏭 Build

[workflows/build.yml](src/.github/workflows/build.yml)

Build the different artifacts produced from the codebase.

The workflow contains a large set of jobs to deal with different project typologies (technology, programming language...).

### 🚀 Publish

[workflows/publish.yml](src/.github/workflows/publish.yml)

Publish the different artifacts produced from the codebase.

The workflow contains a large set of jobs to deal with different project typologies (technology, programming language...).

### 🪄 Auto merge

[workflows/auto-merge.yml](src/.github/workflows/auto-merge.yml)

Automatically merges a Pull request satisfying conditions (i.e. `dependabot` PR targeting minor or patch updates).

### 🙏 Give thanks

[workflows/thank.yml](src/.github/workflows/thank.yml)

Give thanks to the used dependencies by starring the corresponding GitHub repositories.

### 🎨 Export draw.io

[workflows/export-drawio.yml](src/.github/workflows/export-drawio.yml)

Export [draw.io](https://app.diagrams.net/) diagrams to usable png files.

### ☸️ K8S cluster graphs

[workflows/k8s-cluster-graphs.yml](src/.github/workflows/k8s-cluster-graphs.yml)

Create Kubernetes cluster graphs representing its state using the `kubectl` [graph plugin](https://github.com/steveteuber/kubectl-graph).

## 🧑‍💻 Usage

The workflows contains reusable GitHub actions jobs that can be used as a base recipe for your own workflows. Just pick the ones you're interrested in and add them to your `.github/workflows/xxxx.yml` workflow file in your repository.

### 🛡 Access Token

Most jobs need a specific access token with appropriate permissions to run correctly. This token is named `OKP4_TOKEN`, and is defined at the level of the organization. If needed, read the documentation on creating a [PA token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).

[okp4]: https://okp4.network
