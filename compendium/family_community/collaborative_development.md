# Collaborative Development

__Our concept of collaborative development__

Researchers who participate in the development of the Open Energy Family are
known as "core developers". Their work involves capturing scientific processes
that can be implemented in software, gathering requirements, and developing
processes or artifacts such as software code and test results.
Additionally, they contribute to the development of specific Family Members,
like the ontology, drawing on their expertise in fields such as energy systems.
Core developers collaborate with the open community to improve and maintain the
software and troubleshoot any issues that arise.

To ensure the transparency and accessibility of the development process,
all developments are publicly planned, executed, and documented on GitHub and
in development meetings.
Core developers also have direct or indirect access to internal systems such as
servers that cannot be publicly accessible for security reasons.

While the core developers are responsible for the bulk of the development work,
the Open Energy Family is open to participation from anyone interested in
contributing.
This includes stakeholders such as other researchers in the energy system
domain who may not be directly involved in the research projects but have an
interest in the tools and services offered by the framework.

As the work of core developers requires significant effort, funding is crucial
to ensure their continued participation. It is therefore essential that
individuals are deployed as part of a research project that provides adequate
funding for their work. By embracing the collaborative spirit of Open Science,
the Open Energy Family is able to leverage the expertise and contributions of a
diverse range of stakeholders to create a more sustainable and
equitable energy system.

<figure markdown>
  ![Image title](../img/oef-concept-collaboration-developer.png){ width="600" }
  <figcaption>
    The figure shows the structure of the community (purely in regard to development): The total community is divided into two groups, which were defined in detail as personas. As shown, both groups can participate in development, but the core developers take on a special responsibility here and usually work with the support of funded research projects.
  </figcaption>
</figure>

## Collaborative software development process

The following outlines how software development is implemented collaboratively in an open-source and research environment. The previously described concept of collaborative development sets the framework for software development here.

The essential components through which software development is carried out include a tailored iterative development process aligned with our requirements and a role concept. These components will be described in detail, but it should be noted that additional practices must be employed to implement development in practice. An example is development using Git and GitHub. For collaboration, we have created detailed guidelines for naming Git branches and templates for issue creation, which are linked to the appropriate locations.

### Develope Iterative & Incrementally

We adhere to the common iterative model for software development and the software lifecycle. In the Open Energy Family, we primarily focus on continuous development of our software, which is developed and further improved in various research projects. For this reason, we view development as a process that must enable organic growth. At the same time, we recognize the need to handle various types of requirements, including fixed and long-term requirements from research projects, as well as flexible and short-term requirements arising either from users or the identification of new requirements during development. Such an approach is described in the literature as a Hybrid Development Model, as we do not exclusively follow an agile approach and do not strictly adhere to the Waterfall model in project implementation.

Our iterative process is presented here as an overview and spans the various phases of the software lifecycle. The result is an increment that is to be understood as a specific version of the software. An increment can be released and serves as the starting point for the subsequent iteration. It is important to highlight the integrated documentation and testing steps. By incorporating these tasks as integral parts of development, we ensure complete documentation, goal-oriented development through acceptance testing, and the functionality of the software at all times.

<figure markdown>
  ![Image title](../img/dev-process/iterative-dev-overview.png){ width="600" }
  <figcaption>
   Overview of an iteration of the collaborative software development process of the OpenEnergyFamily. The circle shows the software life cycle, which has been adapted to the specific requirements. The yellow boxes give an impression of the process used for each phase. A summary of the process is then shown next to it.
  </figcaption>
</figure>

Over time, the increments are further developed, and an optimal solution is approached. The advantage lies in the fact that each increment is immediately available to all users as a release. This allows for feedback to be incorporated into each subsequent iteration, particularly to ensure user-friendliness.

<figure markdown>
  ![Image title](../img/dev-process/ongoing-developement-iterations-2023-10-24-1338.png){ width="800" }
  <figcaption>
    Ongoing development is carried out through several iterations with the aim of regularly publishing a new software version. This ensures that the development status and the publicly available software version are not too far apart.
  </figcaption>
</figure>

Going through the phases and the associated effort beyond writing code and releasing software has various advantages. In the short term, it ensures that work is done properly and in line with the agreed-upon requirements for craftsmanship and product. In the long term, it aims to keep the software continuously maintainable and enable further development and reusability. For research, this is a particular focus that contributes to sharing software as research results in a traceable manner and finding synergies.

Below we show all phases in detail. The detailed information is relevant to facilitate teamwork. The goal is to enable a transparent and predictable way of working. Even if the work is not done directly in a team, it is still important to follow the steps to document development decisions in a traceable manner. Working with GitHub as a development platform should be kept in mind. Many additional pieces of information can be documented there, and communication with others is greatly simplified. Communication in development teams and even at a higher level within the entire community or with individuals involved in development should ideally always be up to date. This way, the overall structure of the software architecture should always be known.

### Development phases

In a nutshell, the collaborative software development process defines the approach from the vague idea through getting involved & start planning, testing & implementation to release and finally installation and operation. The aspect of collaborative cooperation is particularly emphasized here, as our software products are freely usable open source software. In the long term, we strive for community-driven implementation during development. In doing so, we are following the idea that the OpenEnergyFamily can be used as a framework for various research projects and thus expanded. The vision is to work together on the implementation of optimal solutions. The community benefits from the freely usable results & infrastructure, the available expertise and the opportunity to contribute its own ideas and thus actively participate in shaping them. We want to follow the Open Science principles.

#### Phase 1: Start, Requirements & Planning

<figure markdown>
  ![Image title](../img/dev-process/phase-1.png){ width="300" }
</figure>

__Summary__

Which goals should be achieved in the 1st phase:

Requirements are created as informal textual descriptions. Information about purpose, users, use cases, functions, priority, and open questions is specified. It is clearly described what criteria must be met for the requirement to be fulfilled.
For each requirement or related requirements, an issue is created on GitHub and filled out according to the guidelines from an issue template.
The development project is created as a project on GitHub, and relevant issues are added.
The development team is assigned to the relevant issues.

__Step 1 - Change Request:__

Initially, a change request is submitted or created, akin to gathering requirements as a foundation for specifying software development requirements in the final step of this phase.

Communication of a change request typically occurs through GitHub using the ticket system (Issues) or the discussion area. For more complex issues, discussion in a developer meeting is also possible. A change request doesn't need to be qualitatively extensive; the focus is on documenting a need, with specification happening later.

Predefined requirements from research projects and specific user needs (user requirements) are the primary sources for requirements included in most change requests. Other potential sources include simple ideas from the community, considered as user requirements. The difference is that there's no immediate idea about what and how to implement, rather a vague idea that needs more specification.

___Errors & Bugfixes___

Additionally, addressing software development errors is among the possible change requests. Errors are a special case, as it's not necessary to go through all the steps of the first phase since what needs to be developed is already clear. Generally, errors not caught by automated tests are discovered in user testing (Phase 4) or during software use (Phase 5: Operation). It's crucial to determine whether an error requires new development, as the functionality cannot otherwise be used. In such cases, it may be necessary to complete all phases. However, most errors are of minor scope and can be resolved quickly. Hence, the subsequent steps of the first and second phases can be skipped, and implementation (error correction) in Phase 3 can start directly. This is referred to as a "BugFix."

Once a change request is submitted, especially if it involves a new feature, implementation cannot start immediately. Changes or requirements may also be interconnected. To maintain an overview of all changes during development, prioritization of change requests is done, and the current development project is planned.

Involved developer roles:

- oep-community-manager

__Step 2 - Prioritization & Planning:__

Prioritizing change requests and requirements, planning the current development project, and integrating it into the overarching development roadmap are tasks in that are included in the step. This is crucial for breaking down the long-term development into smaller work-packages, working towards an overarching goal. The roadmap outlines the long-term development plan roughly, providing developers with an idea of the major development goals. Various projects are currently available on GitHub, and future milestones will be created for them.

To prepare for prioritization, all change requests and requirements logged on GitHub as Issues are automated into a backlog. The backlog, a list on GitHub, collects all available requirements (Issues). Subsequently, prioritization is conducted to determine if a change, for example, should be implemented in the Open Energy Platform. If a change request is deemed relevant after prioritization, its placement in the current development workflow is decided. This is necessary when other developments must be completed first or priorities lie in different task areas. If a change request aligns with the ongoing project and can be implemented immediately after prioritization. In this case it is scheduled for an upcoming development project, providing a rough timeframe for development. Occasionally, specific, binding deadlines are set, impacting prioritization – for instance, if a new function is crucial for a research project's work package and must be presented in a meeting.

Requirements can change during development, and new ones may emerge. Therefore, allocating requirements to a specific release is not always fixed. Unimplemented requirements at a release's launch are scheduled for the subsequent release. Planning requirements for a release announces the start of implementation, signaling that the following steps and phases of the development process will be undertaken. The number of iterations for requirement completion is not predefined.

Core developers play a significant role in prioritization, given their need to oversee current and upcoming development steps. The development principle "Release early, release often" is generally followed to promptly showcase users with ongoing developments.

Once it's decided that a change request should be implemented, the next steps can be taken.

Involved developer roles:

- oep-product-owner
- oep-expert
- oep-software-developer

__Step 3 - Development Team:__

Establishing a development team is essential to clearly distribute responsibilities and foster transparency within the community. While individual efforts can implement development projects, it is generally advisable to form a team. This facilitates practices such as the 4-eye principle from Extreme Programming, where implementation is carried out collaboratively, ensuring a constructive distribution of responsibilities. Common team divisions include Frontend and Backend developers or Developers and Domain Experts. A development team takes on various responsibilities, including executing the subsequent steps of the development process, addressing content-related development queries, documenting and communicating the current development status. It is also assumed that a developer or team adheres to the guidelines established for participation in the development. For instance, various documents are provided in each GitHub repository, with special attention to the CONTRIBUTING.md document.

Involved developer roles:

- oep-domain-expert-energy-modelling
- oep-ui-ux-developer
- oep-software-engineer
- oep-junior-developer
- oep-expert

__Step 4 - Create and Specify Requirements:__

This step focuses on specifying the change request from the initial phase. The goal is to develop a coordinated system specification, serving as the basis for the detailed technical implementation. Since the desired changes are broadly known, the next step is to specify what the change request includes in terms of concrete requirements (functional solution).

When a new functionality (feature) is requested with the change request, it is recommended to first establish a consistent naming convention for the feature. This is crucial for referencing the new functionality in communication. For example, in the development of a new feature for the Open Energy Platform, the functionality was named the "Open Annotation Tool."

Assume a specific but broadly formulated change request for the OpenEnergyPlatform: "I need a button to initiate an Open Peer Review." This generates numerous detailed requirements such as "Where is the button visible?" and "Who can activate the button?" Additionally, the process of the Open Peer Review is not clear. Therefore, it is necessary to design the process and adapt it for implementation in a web application. These various detailed or extensive requirements are typically identified in an analysis phase, often involving a brainstorming session with as many stakeholders as possible. The result is the specification of the software system, which is then aligned with the change request to validate that the software system can fulfill the needs of users. Since various stakeholders are involved in this process, and the specification is systematically developed, a coordinated system specification is established.

Involved developer roles:

- oep-product-owner
- oep-domain-expert-energy-modelling
- oep-ui-ux-developer
- oep-software-engineer
- oep-junior-developer
- oep-expert

#### Phase 2: Specification & Design (User interface & Software functionality)

<figure markdown>
  ![Image title](../img/dev-process/phase-2.png){ width="300" }
</figure>

#### Phase 3: Implementation

<figure markdown>
  ![Image title](../img/dev-process/phase-3.png){ width="400" }
</figure>

#### Phase 4: Acceptance test & release

<figure markdown>
  ![Image title](../img/dev-process/phase-4.png){ width="300" }
</figure>

#### Phase 5: Delivery, Installation & Operation

<figure markdown>
  ![Image title](../img/dev-process/phase-5.png){ width="400" }
</figure>

## GitHub Teams

We have specific _Softwaredeveloper Roles_ which are implemented as [_GitHub Teams_](https://github.com/orgs/OpenEnergyPlatform/teams/oef-software-developer/teams)
to coordinate the development.<br>
They can only be seen by members of the community.

Below, we present a comprehensive overview of all teams dedicated to the developement of software and provide clarification on the identified responsibilities for each role.

In addition to clarifying the responsibilities, we leverage teams to enhance communication. This is particularly effective on GitHub, where users can mention teams in issues, discussions, or pull requests to reach a group of individuals and increase the likelihood of receiving prompt responses. To contact a specific team, use "@" followed by the team name.

To apply for contribution, please get in touch. Take a look at our [contact information](contact.md).

| Team                      | Responsibilities                                                                                                          | [GitHub Rights](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/repository-roles-for-an-organization#permissions-for-each-role) |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------|---------------|
| oep-domain-expert-energy-modelling | - Answers domain-specific questions<br>- Ensures that functionalities solve or support domain-specific problems           | Read          |
| oep-community-manager     | - Moderates issues and discussions<br>- Enforces the "Code of Conduct" and "Contributing" guidelines<br>- Maintains the guidelines       | Triage        |
| oep-product-releaser      | - Enforces release guidelines<br>- Publishes GitHub release<br>- Ensures a release is delivered<br>- Maintains the documentation of changes and the release procedure | Maintainer    |
| oep-product-owner         | - Knows the vision and mission of the overall project<br>- Knows the product<br>- Accepts or rejects changes              | Admin         |
| oep-ui-ux-developer       | - Ensures usability and user experience aspects are implemented<br>- Assists in creating mockups or general design tasks such as graphics, logos, icons, etc. | Write         |
| oep-software-engineer     | - Can independently carry out development according to guidelines<br>- Participates in the planning of ongoing development<br>- Mentors junior developers and provides general technical support<br>- Knows the architecture of at least one software product in the Open Energy Family<br>- Conducts code reviews | Write         |
| oep-junior-developer      | - Has little or no experience in software development and the Open Energy Family<br>- Wishes to contribute to development in the short or long term<br>- Has basic programming knowledge | Write         |
| oep-expert                | - Knows the entire system: all products, especially the software products of the Open Energy Family, including the current architecture and usage, as well as planned developments<br>- Understands dependencies and can assess the impact of changes<br>- Has the final say in development decisions, such as which technology to use, which standards to follow, which pattern to implement | Maintainer    |
| oep-infrastructure-manager | - Implements and operates the CI/CD pipeline and assists in troubleshooting and log analysis<br>- Installs new software versions on a server (after a GitHub release)<br>- Installs new test software version on a server (before a GitHub release)<br>- Manages the installation and operation of all other software tools such as documentation tools | Admin         |
| oep-tester                | - Tests the software, for example, once a test release is published<br>- Continuously checks the functionality of the software products<br>- Continuously checks the content, such as texts in training courses or texts on websites, etc. | Read          |
