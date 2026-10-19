# Personas

The seven personas represent the main user groups of the Open Energy Platform.
The [concept](index.md#concept) explains the roles, interaction modes and structure of the personas.
Use-case IDs refer to [Use-Cases](use-cases.md).

| Persona                               | Role        | Preferred mode | Focus                                                          | Expected entry points               |
|---------------------------------------|-------------|----------------|----------------------------------------------------------------|-------------------------------------|
| [Alix Agency](#alix-agency)           | Consumer    | Web            | Prepare commissioning decisions and verify contract fulfilment | Scenario Bundles, Database          |
| [Charles Champion](#charles-champion) | Consumer    | Data           | Analyse scenario results and communicate them publicly         | Scenario Bundles, Database          |
| [Elisa Energy](#elisa-energy)         | Consumer    | Code           | Integrate data programmatically into a model                   | Database, API, Academy              |
| [Bob Branch](#bob-branch)             | Contributor | Web            | Publish research results without technical hurdles             | Scenario Bundles, Open Science      |
| [Mona Modeling](#mona-modeling)       | Contributor | Data           | Provide and document research data in a structured way         | Database, Scenario Bundles, Academy |
| [Fred Framework](#fred-framework)     | Contributor | Code           | Use the interfaces and contribute technically                  | API, Open Energy Community          |
| [Diana Diligence](#diana-diligence)   | Reviewer    | Data           | Assess data quality and scientific comparability               | Database, Ontology                  |

---

## Alix Agency

![Alix Agency](../../img/personas/alix.png)

**Role:** Consumer · **Preferred mode:** Web

**Focus.** Alix prepares commissioning decisions and checks whether contractors have
published what was agreed. She does not analyse data herself.

**Context.** Project officer at a government agency that commissions energy and climate
scenario studies. She prepares the content of calls for tenders and supervises the
contractors; the head of unit takes the final decision. Her work follows one process:
research existing models and studies, define publication requirements, verify the publications.

**Goals**

- Know which models and scenario studies and institutions already exist before a project is commissioned.
- Include clear, verifiable publication requirements in contracts.
- Confirm that a contractor has met these requirements before final payment.

**Obstacles and requirements**

| Obstacle                                                       | Requirement for the OEP                                                  | Expected result                                           |
|----------------------------------------------------------------|--------------------------------------------------------------------------|-----------------------------------------------------------|
| Technical terms such as git, API or ontology are not explained | Plain-language labels; explanations of technical terms where they appear | Alix finds her way without asking colleagues              |
| Information on studies is spread over several pages            | Search and filter scenario studies by region and topic                   | An overview of existing studies in minutes                |
| Publications of an institution cannot be listed in one place   | A view of all contributions of an institution                            | Contract fulfilment can be checked without technical help |

**Skills and tools.** Office software on Windows, no programming. Reads English well,
but technical terminology in English slows her down.

**Accessibility.** No specific individual accessibility requirements identified.

**Entry points.** Scenario Bundles, Database

**User stories**

- As Alix, I want to find the scenario studies for Germany and the institutions that produced them, so that I can scope a new call for tenders. ([UC-01](use-cases.md#uc-01))
- As Alix, I want a non-technical summary of the requirements for publishing on the OEP, so that I can include them in contracts. ([UC-11](use-cases.md#uc-11))
- As Alix, I want to see all datasets and scenario bundles an institution has published, so that I can confirm the contractor has met the publication obligations. ([UC-04](use-cases.md#uc-04))

**Success.** Alix can list the relevant existing studies for a call, and she can check a
contractor's publications against the requirements in the contract.

---

## Charles Champion

![Charles Champion](../../img/personas/charles.png)

**Role:** Consumer · **Preferred mode:** Data

**Focus.** Charles compares published scenario results to communicate them to the public.
Unlike Diana, he does not assess the scientific quality of the scenarios.

**Context.** Policy analyst at a climate NGO. He prepares statements and campaign material
that compare, for example, the projected share of renewable energy or the greenhouse gas
emissions by sector across scenarios for the same target year.

**Goals**

- Compare projected values of the same indicator across several scenarios.
- Publish charts that are traceable through source, licence and underlying data.

**Obstacles and requirements**

| Obstacle                                                                    | Requirement for the OEP                                 | Expected result                                     |
|-----------------------------------------------------------------------------|---------------------------------------------------------|-----------------------------------------------------|
| Relevant data are difficult to find among extensive descriptive information | Direct links from a scenario to its result data         | Charles reaches the figures he needs in a few steps |
| Data of one scenario are spread over several tables without guidance        | Overview of the tables belonging to a scenario          | Fewer wrong or incomplete downloads                 |
| Licence and source of a dataset are not visible at a glance                 | Licence and citation shown with every dataset and chart | Charts can be published with correct attribution    |

**Skills and tools.** Spreadsheets and office tools, no programming.

**Accessibility.** No specific individual accessibility requirements identified.

**Entry points.** Scenario Bundles, Database

**User stories**

- As Charles, I want to compare the projected values of the same indicator across scenarios for the same region and target year, so that I can show how far the scenarios diverge. ([UC-02](use-cases.md#uc-02))
- As Charles, I want to find the dataset behind a scenario result and see whether its licence allows publication, so that I can use it in campaign material. ([UC-05](use-cases.md#uc-05))
- As Charles, I want to create a chart from selected data and export it with source and licence information, so that others can trace the figures. ([UC-07](use-cases.md#uc-07))

**Success.** Charles can publish a chart comparing several scenarios that states its source
and licence and points to the underlying data.

---

## Elisa Energy

![Elisa Energy](../../img/personas/elisa.png)

**Role:** Consumer · **Preferred mode:** Code

**Focus.** Elisa integrates data from the OEP into her own model by program code.
She neither publishes nor reviews data.

**Context.** Master's student in renewable energy systems. For a course assignment,
she builds a model of one federal state and needs the installed capacity of power plants
by technology and municipality as input.

**Goals**

- Find out whether a suitable dataset exists before investing time in it.
- Load the data directly into her model instead of downloading files.

**Obstacles and requirements**

| Obstacle                                               | Requirement for the OEP                                                                         | Expected result                                 |
|--------------------------------------------------------|-------------------------------------------------------------------------------------------------|-------------------------------------------------|
| Unclear whether a dataset fits before downloading it   | Preview of content, spatial coverage and metadata in the search results and on the dataset page | Fewer unsuitable downloads                      |
| No end-to-end example from search to model input       | Tutorial that queries a table and loads it in Python or R                                       | Elisa has working code in one session           |
| Unclear API parameters, for example for filtering rows | API reference with examples for each parameter                                                  | Elisa can adapt the example to her region       |
| Documentation is fragmented across multiple locations  | A single entry point for getting-started resources                                              | Elisa does not have to search for documentation |

**Skills and tools.** R and some Python, basic database knowledge.

**Accessibility.** No specific individual accessibility requirements identified.

**Entry points.** Database, API, Academy

**User stories**

- As Elisa, I want to search for datasets by topic and region and preview their content, so that I can decide whether a dataset fits my model. ([UC-05](use-cases.md#uc-05))
- As Elisa, I want an example that retrieves a filtered table via the API in Python or R, so that my model reads the data directly. ([UC-06](use-cases.md#uc-06))
- As Elisa, I want a single entry point for getting-started resources, so that I know where to begin. ([UC-10](use-cases.md#uc-10))

**Success.** Elisa's model retrieves the required data automatically from the OEP.

---

## Bob Branch

![Bob Branch](../../img/personas/bob.png)

**Role:** Contributor · **Preferred mode:** Web

**Focus.** Bob publishes the scenario studies of his group without having to learn technical
workflows. Unlike Mona, he publishes descriptions of studies, not data.

**Context.** Senior researcher in environmental studies who leads several projects.
He wants to make the scenario studies of his group findable and citable and uses
existing studies to identify topics for new project proposals. He has little time for
technical publication processes.

**Goals**

- Publish his group's scenario studies in a structured, citable form.
- Identify research gaps across existing scenario studies.

**Obstacles and requirements**

| Obstacle                                          | Requirement for the OEP                                 | Expected result                                        |
|---------------------------------------------------|---------------------------------------------------------|--------------------------------------------------------|
| Workflows that require git, GitHub or programming | Web forms with examples for each field                  | Bob publishes a study without technical help           |
| Uncertainty about which open licence to choose    | Short explanation of common licences and a decision aid | Bob selects a licence and understands its consequences |
| Missing source attribution in other publications  | Citation information for each scenario bundle           | His work is cited correctly                            |

**Skills and tools.** Office software and statistics tools. No experience with
licences or collaborative workflows. Reads English well, writes it less confidently.

**Accessibility.** No specific individual accessibility requirements identified.

**Entry points.** Scenario Bundles, Open Science

**User stories**

- As Bob, I want to describe a scenario study and its scenarios in web forms, so that others can find and cite it. ([UC-12](use-cases.md#uc-12))
- As Bob, I want to understand which licence suits my publications, so that I can publish without legal uncertainty. ([UC-13](use-cases.md#uc-13))
- As Bob, I want to see which regions, sectors and target years existing scenario studies cover, so that I can identify gaps for a project proposal. ([UC-08](use-cases.md#uc-08))

**Success.** Bob's study is published as a scenario bundle with a licence and citation
information, and he can name gaps in existing studies.

---

## Mona Modelling

![Mona Modelling](../../img/personas/mona.png)

**Role:** Contributor · **Preferred mode:** Data

**Focus.** Mona is responsible for the scientific provision and documentation of her results.
Unlike Fred, she does not build technical integrations.

**Context.** Junior researcher in energy system modelling at a research institute.
She works on publicly funded scenario studies whose funding body requires publication
of the results as open data.

**Goals**

- Publish her results with the metadata required by her funding body.
- Document how her results were produced, by linking data, model and study.
- Keep track of which models other groups use (research need, separate from publishing).

**Obstacles and requirements**

| Obstacle                                                              | Requirement for the OEP                                                  | Expected result                                    |
|-----------------------------------------------------------------------|--------------------------------------------------------------------------|----------------------------------------------------|
| The upload of data and metadata has many unstructured steps           | A process that guides her from table to published dataset                | Publication within the time planned in the project |
| She does not know whether her metadata is complete and formally valid | Check for completeness and validity against OEMetadata before submission | Fewer revisions in the review                      |
| Scientific quality is only checked after submission                   | Clear review criteria, known in advance                                  | Mona can prepare her data accordingly              |

**Skills and tools.** Python and databases, uses APIs to gather model input.

**Accessibility.** No specific individual accessibility requirements identified.

**Entry points.** Database, Scenario Bundles, Academy

**User stories**

- As Mona, I want to publish my model results with the metadata my funding body requires, without studying the metadata specification in detail, so that I meet the obligation within the project time. ([UC-14](use-cases.md#uc-14))
- As Mona, I want to know before submission whether my metadata is complete and formally valid, so that the review concentrates on content. ([UC-15](use-cases.md#uc-15))
- As Mona, I want to link my datasets, my model and my study in a scenario bundle, so that others can trace how the results were produced. ([UC-12](use-cases.md#uc-12))
- As Mona, I want to find which scenarios were computed with a given model, so that I can compare its use with my own. ([UC-09](use-cases.md#uc-09))

**Success.** Mona's dataset passes the review and is linked to her model and study
in a scenario bundle.

---

## Fred Framework

![Fred Framework](../../img/personas/fred.png)

**Role:** Contributor · **Preferred mode:** Code

**Focus.** Fred builds technical integrations with the OEP and contributes to its software.
He does not curate the scientific content of datasets.

**Context.** Data scientist and open source developer. Maintains his own open source
projects and contributes to others. He wants to update datasets on the OEP automatically
from his data pipeline.

**Goals**

- Upload and update datasets automatically via the API.
- Contribute bug fixes to the OEP.
- Use data with complete, traceable metadata and a documented review status.

**Obstacles and requirements**

| Obstacle                                                                     | Requirement for the OEP                                             | Expected result                                      |
|------------------------------------------------------------------------------|---------------------------------------------------------------------|------------------------------------------------------|
| Inconsistent behaviour or outdated documentation quickly blocks his workflow | API reference that matches the implementation; versioned changes    | Fred's pipeline runs without manual intervention     |
| Error responses do not state the cause                                       | Error messages with cause and affected field                        | Fred fixes failed uploads without contacting support |
| Contribution process is hard to find                                         | Visible link to repository, contribution guidelines and open issues | Fred submits a pull request without asking           |

**Skills and tools.** Python, REST APIs, git and GitHub.

**Accessibility.** Red-green colour vision deficiency. Charts, status indicators and badges
must be distinguishable without colour (see [platform requirements](index.md#accessibility)).

**Entry points.** API, Open Energy Community

**User stories**

- As Fred, I want to upload and update tables with metadata via the API, so that my pipeline publishes new data automatically. ([UC-16](use-cases.md#uc-16))
- As Fred, I want to find the contribution guidelines and open issues of the OEP, so that I can contribute bug fixes. ([UC-17](use-cases.md#uc-17))
- As Fred, I want to see the licence, metadata completeness and review status of a dataset, so that I only build on reviewed data. ([UC-18](use-cases.md#uc-18))

**Success.** Fred's pipeline updates a dataset on the OEP without manual steps, and his
pull request is accepted.

---

## Diana Diligence

![Diana Diligence](../../img/personas/diana.png)

**Role:** Reviewer · **Preferred mode:** Data

**Focus.** Diana assesses the quality and scientific comparability of data published by others.
Unlike Charles, she examines the assumptions behind the results, not only the results.

**Context.** Postdoctoral researcher in economics who studies the economic and distributional
effects of energy and climate policy. She compares the economic input assumptions of
scenarios for her own work. As a reviewer in the Open Peer Review, she checks datasets
of other contributors. When she finds that economic concepts are missing from the
Open Energy Ontology during a review, she proposes new terms.

**Goals**

- Compare economic input assumptions (GDP, energy prices) across scenarios.
- Improve the quality of published datasets through reviews.
- Have economic concepts represented in the Open Energy Ontology.

**Obstacles and requirements**

| Obstacle                                          | Requirement for the OEP                                   | Expected result                                    |
|---------------------------------------------------|-----------------------------------------------------------|----------------------------------------------------|
| No clear review criteria                          | Documented criteria for each metadata field               | Reviews are consistent across reviewers            |
| Decisions on ontology proposals are not traceable | Documented process and decision record for term proposals | Diana knows the status of her proposals            |
| Input assumptions are hidden in result tables     | Assumptions labelled and annotated with ontology terms    | Assumptions of different scenarios can be compared |

**Skills and tools.** Office software on macOS, some Python and SQL.

**Accessibility.** No specific individual accessibility requirements identified.

**Entry points.** Database, Ontology

**User stories**

- As Diana, I want to compare the economic input assumptions of several scenarios, so that I can calibrate my own model. ([UC-03](use-cases.md#uc-03))
- As Diana, I want to review the metadata of a submitted dataset against documented criteria, so that my review is consistent with those of others. ([UC-19](use-cases.md#uc-19))
- As Diana, I want to propose an economic term for the Open Energy Ontology and follow the decision on it, so that missing concepts can be used in annotations. ([UC-20](use-cases.md#uc-20))

**Success.** Diana completes a review based on documented criteria, and her term proposal
receives a traceable decision.

---

## Attribution

Images by **studio4rt** on Freepik.
