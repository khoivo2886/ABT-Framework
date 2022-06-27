# ABT-Framework

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

A simple native Android application that shows a list of cities which user can search to view location of city on maps
## Features
- Support a thoundsand of cities.
- Support auto-complete when user input city name.
- Display location of selected city

# Action Based Testing Framework
Action Based Testing Framework (ABTF) allows automating End-to-End UI test via `Espresso` lib. `Kotlin` is language being used in framework to write test script.

#### Table of Contents
1.  [Description](#description)
2.  [Structure](#installation)
3.  [Usage](#usage)
    *   [Code of conduct](#code-of-conduct)
    *   [Community Guidelines](#community-guidelines)
    *   [Contributor Agreement](#contributor-agreement)
6.  [Reporting Issues](#reporting-issues)
7.  [Statement of Support](#statement-of-support)
8.  [License](#license)

## <a id="description"></a>Description

- This framework is using **Action Based Testing method (ABTM)** which represents the continued evolution of the keyword driven testing approach, which uses keywords to create and automate the majority of tests.
- ABT provides a powerful framework for organizing test design, automation and execution around keywords. In ABT, keywords are called **actions**-to make the concept absolutely clear. Actions are the tasks that are executed during a test. Rather than automating an entire test as one long script, tests are assembled using individual actions. Non-technical test engineers and business analysts can then define their tests as a series of these automated actions.
- ABT test case takes place in a class called as test class. Actions, test data, and any necessary GUI interface information are stored separately and referenced by the main test class.


## <a id="installation"></a>Installation

The tools and executable for DAF have been containerized with docker for convenience. Use the latest version by pulling the container below.

```bash
docker pull delphix/automation-framework
```
### <a id="delphix-yaml"></a>The delphix.yaml file

The `delphix.yaml` file is the configuration file that defines the data management as code strategy for the project. Create a `delphix.yaml` file based on this guide: [Configure Delphix YAML](./configure-delphix-yaml.md)

## <a id="usage"></a>Usage

Create an `.env` file with the following values:
*   GIT_BRANCH=
*   DELPHIX_PASS=
*   DELPHIX_USER=
*   DELPHIX_ENGINE=
*   GIT_EVENT=
*   GIT_COMMIT=

Optionally, the `GIT_EVENT` can be set by a GitHub Webhook Payload file: `payload.json`.<br /><br />
Run the docker container with your project mounted as a volume and environment file instantiated.

```bash
docker run -v ${PWD}:/daf/app --env-file ${PWD}/.env delphix/automation-framework
```

## <a id="links"></a>Links

*   [Creating GitHub Webhooks](https://developer.github.com/webhooks/creating/)
*   [Setting Docker Environment Variables](https://docs.docker.com/engine/reference/commandline/run/#set-environment-variables--e---env---env-file)

## <a id="contribute"></a>Contribute

1.  Fork the project.
2.  Make your bug fix or new feature.
3.  Add tests for your code.
4.  Send a pull request.

Contributions must be signed as `User Name <user@email.com>`. Make sure to [set up Git with user name and email address](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup). Bug fixes should branch from the current stable branch. New features should be based on the `master` branch.

#### <a id="code-of-conduct"></a>Code of Conduct

This project operates under the [Delphix Code of Conduct](https://delphix.github.io/code-of-conduct.html). By participating in this project you agree to abide by its terms.

#### <a id="contributor-agreement"></a>Contributor Agreement

All contributors are required to sign the Delphix Contributor agreement prior to contributing code to an open source repository. This process is handled automatically by [cla-assistant](https://cla-assistant.io/). Simply open a pull request and a bot will automatically check to see if you have signed the latest agreement. If not, you will be prompted to do so as part of the pull request process.


## <a id="reporting_issues"></a>Reporting Issues

Issues should be reported in the GitHub repo's issue tab. Include a link to it.

## <a id="statement-of-support"></a>Statement of Support

This software is provided as-is, without warranty of any kind or commercial support through Delphix. See the associated license for additional details. Questions, issues, feature requests, and contributions should be directed to the community as outlined in the [Delphix Community Guidelines](https://delphix.github.io/community-guidelines.html).

## <a id="license"></a>License

This is code is licensed under the Apache License 2.0. Full license is available [here](./LICENSE).
