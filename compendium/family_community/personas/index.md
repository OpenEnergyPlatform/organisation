# Personas and Use-Cases

Personas are fictional but representative users of the Open Energy Platform (OEP).
They make our assumptions about users explicit, so that design decisions and
evaluations refer to concrete needs instead of an abstract "user".
Use-cases describe the tasks these personas perform on the platform.

## Origin and validity

The personas were first written in the SIROP project and revised in October 2026
for the evaluation of the new OEP start page. Both versions are based on the
experience of the OEP developer groups from development, support and community work.
They are not based on systematic user research such as interviews or usage analyses.

The personas are therefore working assumptions. Each evaluation is also a check of the
personas: findings that contradict a persona are recorded and used in the next revision.


## Concept

Each persona is placed along two dimensions: the **role** it takes on the platform and
its **preferred interaction mode**.

### User role

The roles follow the [OEP user concept](../../family_members/software-architecture/open-energy-platform.md#users).

| Role        | Description                                                                                             |
|-------------|---------------------------------------------------------------------------------------------------------|
| Consumer    | Searches, inspects, compares and retrieves data, scenarios and documentation.                           |
| Contributor | Publishes data, metadata, scenario bundles, ontology terms or code.                                     |
| Reviewer    | Checks the contributions of others, for example in the Open Peer Review, and improves metadata quality. |

A persona has one primary role. It can take on other roles in individual user stories.

### Interaction mode

The interaction mode describes how a persona *prefers* to work with the platform.
It is not an exclusive skill: a persona with the mode data can also use the web interface.
The modes replace the earlier categories *Qualitist*, *Quantitist* and *Apinist*.

| Mode | Description                                                                                                        | Earlier category |
|------|--------------------------------------------------------------------------------------------------------------------|------------------|
| Web  | Works with graphical interfaces, forms and guided workflows. Does not program.                                     | Qualitist        |
| Data | Downloads tables and analyses them with standard tools such as spreadsheets, statistics software or short scripts. | Quantitist       |
| Code | Accesses the platform programmatically via the API and libraries, writes scripts and automates workflows.          | Apinist          |

### Persona matrix

|                 | Web                                    | Data                                             | Code                                         |
|-----------------|----------------------------------------|--------------------------------------------------|----------------------------------------------|
| **Consumer**    | [Alix Agency](personas.md#alix-agency) | [Charles Champion](personas.md#charles-champion) | [Elisa Energy](personas.md#elisa-energy)     |
| **Contributor** | [Bob Branch](personas.md#bob-branch)   | [Mona Modeling](personas.md#mona-modeling)       | [Fred Framework](personas.md#fred-framework) |
| **Reviewer**    |                                        | [Diana Diligence](personas.md#diana-diligence)   |                                              |


### Structure of a persona

Every persona contains these main sections.

| Section                    | Content                                                                                   |
|----------------------------|-------------------------------------------------------------------------------------------|
| Role and mode              | Primary role and preferred interaction mode                                               |
| Focus                      | One sentence that distinguishes the persona's task from those of the other personas       |
| Context                    | Two to three sentences: work environment and the occasion for using the OEP               |
| Goals                      | Two to three prioritised goals, phrased as intended results                               |
| Obstacles and requirements | Concrete obstacles, the requirement each one implies for the OEP, and the expected result |
| Skills and tools           | Only skills and tools that affect how the persona interacts with the platform             |
| Accessibility              | Individual requirements, if identified                                                    |
| Entry points               | The start-page elements where the persona is expected to begin                            |
| User stories               | Three to four stories, each linked to one [use-case](use-cases.md)                        |
| Success                    | How the persona recognises that a task has been completed successfully                    |

Personal details such as age, family status or hobbies are left out
unless they change how the persona uses the platform.
Such details invite caricature in role play and do not inform design decisions.

## Accessibility

Accessibility is a requirement for the whole platform, not for individual personas.
Independent of the personas, the OEP should

- be fully operable by keyboard,
- provide sufficient colour contrast for text and interface elements,
- never convey information by colour alone, for example in charts, status indicators or badges,
- provide text alternatives for images and charts,
- show error messages that state the cause and a possible solution.

Personas only list individual accessibility requirements that go beyond these.

## Terminology

The personas and use-cases use the following terms consistently.

| Term                       | Meaning                                                                                             |
|----------------------------|-----------------------------------------------------------------------------------------------------|
| Scenario study             | A publication, usually a report, that develops and compares one or more scenarios                   |
| Scenario                   | A consistent description of a possible future energy system within a scenario study                 |
| Scenario bundle            | The OEP description of a scenario study that links its scenarios, models, datasets and publications |
| Model                      | Software that computes scenarios; described in a model factsheet                                    |
| Framework                  | Software used to build models; described in a framework factsheet                                   |
| Dataset                    | A data resource on the OEP, consisting of one or more tables and their metadata                     |
| Metadata                   | Description of a dataset in the Open Energy Metadata (OEMetadata) format                            |
| Open Peer Review           | The OEP process in which a reviewer checks the metadata of a dataset before publication             |
| Open Energy Ontology (OEO) | The shared vocabulary of the Open Energy Family, used to annotate metadata                          |
