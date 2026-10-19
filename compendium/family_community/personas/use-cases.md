# Use-Cases

Use-cases describe the tasks the [personas](personas.md) perform on the Open Energy Platform.
They are the shared reference for design decisions and evaluations:
issues, test tasks and findings refer to the use-case ID.
Each user story of a persona refers to exactly one use-case.

The role-level description of what consumers, contributors and reviewers do on the platform
is part of the [OEP documentation](../../family_members/software-architecture/open-energy-platform.md#use-cases).
This page breaks these roles down into concrete tasks. Terms are defined in the
[terminology](index.md#terminology).

## Overview

| ID              | Use-case                                                   | Role                  | Personas       | Expected start-page entry point      |
|-----------------|------------------------------------------------------------|-----------------------|----------------|--------------------------------------|
| [UC-01](#uc-01) | Find scenario studies for a region or topic                | Consumer              | Alix           | Scenario Bundles                     |
| [UC-02](#uc-02) | Compare projected values of an indicator across scenarios  | Consumer              | Charles        | Scenario Bundles                     |
| [UC-03](#uc-03) | Compare input assumptions across scenarios                 | Consumer              | Diana          | Scenario Bundles, Database           |
| [UC-04](#uc-04) | Find the contributions of an institution                   | Consumer              | Alix           | Database, Scenario Bundles           |
| [UC-05](#uc-05) | Find a dataset and assess its fit                          | Consumer              | Elisa, Charles | Database                             |
| [UC-06](#uc-06) | Retrieve data via the API                                  | Consumer              | Elisa          | API                                  |
| [UC-07](#uc-07) | Create a chart with source and licence information         | Consumer              | Charles        | Database                             |
| [UC-08](#uc-08) | Identify gaps across scenario studies                      | Consumer              | Bob            | Scenario Bundles                     |
| [UC-09](#uc-09) | Find models and their use in scenarios                     | Consumer              | Mona           | No dedicated entry on the start page |
| [UC-10](#uc-10) | Find getting-started resources                             | Consumer              | Elisa          | Academy                              |
| [UC-11](#uc-11) | Understand the requirements for publishing on the OEP      | Consumer, Contributor | Alix           | Open Science, Academy                |
| [UC-12](#uc-12) | Publish a scenario study as a scenario bundle              | Contributor           | Bob, Mona      | Scenario Bundles                     |
| [UC-13](#uc-13) | Choose an open licence                                     | Contributor           | Bob            | Open Science                         |
| [UC-14](#uc-14) | Upload a dataset with metadata                             | Contributor           | Mona           | Database, Academy                    |
| [UC-15](#uc-15) | Check metadata before publication                          | Contributor           | Mona           | Database                             |
| [UC-16](#uc-16) | Upload and update data via the API                         | Contributor           | Fred           | API                                  |
| [UC-17](#uc-17) | Contribute to OEP software development                     | Contributor           | Fred           | Open Energy Community                |
| [UC-18](#uc-18) | Assess the quality, licence and review status of a dataset | Consumer, Reviewer    | Fred           | Database                             |
| [UC-19](#uc-19) | Review a dataset in the Open Peer Review                   | Reviewer              | Diana          | Database                             |
| [UC-20](#uc-20) | Propose terms for the Open Energy Ontology                 | Reviewer, Contributor | Diana          | Ontology, Open Energy Community      |

!!! Note
    The entry points refer to the elements of the start page:
    Database, Scenario Bundles, Ontology, Academy, API, Open Science and Open Energy Community.
    They describe where a user is *expected* to begin, not a verified path.
    UC-09 has no dedicated entry on the new start page; the evaluation should show whether one is needed.

## Use-case descriptions

### Find and understand

<a id="uc-01"></a>

#### UC-01: Find scenario studies for a region or topic

- **Role:** Consumer
- **Personas:** Alix
- **Expected entry point:** Scenario Bundles
- **Success criterion:** The usernames the relevant scenario studies, the institutions behind them and the scenarios they contain.

<a id="uc-02"></a>

#### UC-02: Compare projected values of an indicator across scenarios

- **Role:** Consumer
- **Personas:** Charles
- **Expected entry point:** Scenario Bundles
- **Success criterion:** The user sees the values of one indicator for the same region and target year from at least two scenarios, online or as a download.

<a id="uc-03"></a>

#### UC-03: Compare input assumptions across scenarios

- **Role:** Consumer
- **Personas:** Diana
- **Expected entry point:** Scenario Bundles, Database
- **Success criterion:** The user identifies the values of one input assumption, for example GDP or an energy price, in at least two scenarios.

<a id="uc-04"></a>

#### UC-04: Find the contributions of an institution

- **Role:** Consumer
- **Personas:** Alix
- **Expected entry point:** Database, Scenario Bundles
- **Success criterion:** The user lists all datasets and scenario bundles published by a given institution.

<a id="uc-05"></a>

#### UC-05: Find a dataset and assess its fit

- **Role:** Consumer
- **Personas:** Elisa, Charles
- **Expected entry point:** Database
- **Success criterion:** Before downloading, the user knows the content, spatial and temporal coverage and licence of a dataset.

<a id="uc-06"></a>

#### UC-06: Retrieve data via the API

- **Role:** Consumer
- **Personas:** Elisa
- **Expected entry point:** API
- **Success criterion:** The user retrieves a filtered table with a script, using only the documentation.

<a id="uc-07"></a>

#### UC-07: Create a chart with source and licence information

- **Role:** Consumer
- **Personas:** Charles
- **Expected entry point:** Database
- **Success criterion:** The user exports a chart that states source, licence and a link to the underlying data.

<a id="uc-08"></a>

#### UC-08: Identify gaps across scenario studies

- **Role:** Consumer
- **Personas:** Bob
- **Expected entry point:** Scenario Bundles
- **Success criterion:** The user sees which regions, sectors and target years existing scenario studies cover.

<a id="uc-09"></a>

#### UC-09: Find models and their use in scenarios

- **Role:** Consumer
- **Personas:** Mona
- **Expected entry point:** No dedicated entry on the start page
- **Success criterion:** The user finds the model factsheet and the scenarios computed with it.

<a id="uc-10"></a>

#### UC-10: Find getting-started resources

- **Role:** Consumer
- **Personas:** Elisa
- **Expected entry point:** Academy
- **Success criterion:** The user reaches one page that leads to all getting-started material.

### Publish

<a id="uc-11"></a>

#### UC-11: Understand the requirements for publishing on the OEP

- **Role:** Consumer, Contributor
- **Personas:** Alix
- **Expected entry point:** Open Science, Academy
- **Success criterion:** The user can state which data, metadata and licence information a publication requires.

<a id="uc-12"></a>

#### UC-12: Publish a scenario study as a scenario bundle

- **Role:** Contributor
- **Personas:** Bob, Mona
- **Expected entry point:** Scenario Bundles
- **Success criterion:** A scenario bundle exists that links the study with its scenarios, models and datasets.

<a id="uc-13"></a>

#### UC-13: Choose an open licence

- **Role:** Contributor
- **Personas:** Bob
- **Expected entry point:** Open Science
- **Success criterion:** The user selects a licence and can explain what it permits for reuse.

<a id="uc-14"></a>

#### UC-14: Upload a dataset with metadata

- **Role:** Contributor
- **Personas:** Mona
- **Expected entry point:** Database, Academy
- **Success criterion:** A table with OEMetadata is uploaded and submitted for review.

<a id="uc-15"></a>

#### UC-15: Check metadata before publication

- **Role:** Contributor
- **Personas:** Mona
- **Expected entry point:** Database
- **Success criterion:** The user knows whether the metadata is complete and formally valid against OEMetadata. Scientific quality is checked in UC-19.

<a id="uc-16"></a>

#### UC-16: Upload and update data via the API

- **Role:** Contributor
- **Personas:** Fred
- **Expected entry point:** API
- **Success criterion:** A script creates or updates a table with metadata; errors state their cause.

<a id="uc-17"></a>

#### UC-17: Contribute to OEP software development

- **Role:** Contributor
- **Personas:** Fred
- **Expected entry point:** Open Energy Community
- **Success criterion:** The user finds the repository, the contribution guidelines and suitable open issues.

### Review and curate

<a id="uc-18"></a>

#### UC-18: Assess the quality, licence and review status of a dataset

- **Role:** Consumer, Reviewer
- **Personas:** Fred
- **Expected entry point:** Database
- **Success criterion:** The user identifies the licence, the completeness of the metadata and the review status without relying on colour.

<a id="uc-19"></a>

#### UC-19: Review a dataset in the Open Peer Review

- **Role:** Reviewer
- **Personas:** Diana
- **Expected entry point:** Database
- **Success criterion:** The reviewer completes a review against documented criteria; the contributor sees the feedback.

<a id="uc-20"></a>

#### UC-20: Propose terms for the Open Energy Ontology

- **Role:** Reviewer, Contributor
- **Personas:** Diana
- **Expected entry point:** Ontology, Open Energy Community
- **Success criterion:** The user submits a term proposal and can follow the decision on it.

## Start page evaluation tasks

The tasks below test whether the start page leads each persona to the right place.
They are written as situations, not as instructions, and avoid the labels used on the page,
so that testers have to find the way themselves.

| Persona          | Task                                                                                                                                                                                       | Use-case     |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| Alix Agency      | Your agency plans a new study on the heat transition in Germany. Find out which institutions have already published scenarios for Germany.                                                 | UC-01        |
| Alix Agency      | A contractor states that all results have been published. Check what this institution has made available.                                                                                  | UC-04        |
| Charles Champion | For a statement, you need the projected share of renewable energy in 2045 from at least two scenarios. Find the figures and check whether you may publish them.                            | UC-02        |
| Elisa Energy     | For your course assignment, you need power plant data for one federal state. Find a suitable dataset and check whether you can load it from Python without downloading a file.             | UC-05, UC-06 |
| Bob Branch       | You want to make your group's latest scenario study visible on the platform. Find out what you need to do and which licence to choose.                                                     | UC-12, UC-13 |
| Mona Modeling    | Your funding body requires you to publish your model results as open data. Find out how to upload them and how you can check your metadata before submission.                              | UC-14, UC-15 |
| Fred Framework   | You want to fix a bug you noticed on the platform. Find out where and how to contribute. Also check whether all status information on the page can be read without distinguishing colours. | UC-17, UC-18 |
| Diana Diligence  | You want to add economic concepts to the ontology used on the platform. Find out how to propose a term.                                                                                    | UC-20        |

