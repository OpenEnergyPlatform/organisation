# Governance of the Open Energy Family

This document defines the roles, bodies, and decision-making procedures of the
Open Energy Family (OEFamily). It is the authoritative reference. Operational
details such as meeting dates, mailing lists, and contacts are kept on the
[Contact page](../contact/).


## 1. Scope and principles

Four principles underlie the structure.

1. Contribution grounds participation. Within a development group, a say in
   decisions follows from the work done, not from institutional affiliation or
   title.
2. Consensus is the default. A formal vote is the fallback when consensus
   cannot be reached, not the normal case.
3. Decisions, minutes, and votes are documented publicly in the Compendium.
   Only matters that protect individuals, such as Code of Conduct cases, are
   kept private.
4. This document changes only through the procedure in Section 7.

## 2. Membership and voting

An institution joins the OEFamily by contributing to an OEFamily project and
stating this to the OEFamily-SC. Each member institution names a representative
and a deputy for votes.

Voting rights follow active contribution. In practice the institutions
currently doing the work hold the vote; standing is not affected by an
occasional absence. An institution leaves either by its own statement or after
about a year without any contribution. Departures are recorded in the minutes.

## 3. Roles

### 3.1 Community Manager (CM)

The Community Manager connects the community and the development groups. 
The role coordinates and moderates. 
The CM collects and bundles feedback from the community and carries it to the bodies, keeps an
overview of ongoing and planned development and passes on knowledge through
onboarding, documentation, and references, organises and moderates meetings and
community formats, and points out duplicated effort between groups.

The CM has the right to speak and to submit motions in the development groups
and in both committees. Before an adopted decision takes effect, the CM may ask
the responsible committee to reconsider it once (Section 5.5). This is a
suspensive request, not a power to block.

The OEFamily-SC appoints the CM for a term of one year, with reappointment
possible, and may remove the CM by a two-thirds majority. If the position is
vacant, the OEFamily-SC names an interim replacement.

### 3.2 Maintainer

A maintainer carries operational responsibility for a project or component,
including repository rights, releases, and review. Maintainers vote in the
development group of their project.

### 3.3 Contributor

A contributor works actively on a project through code, ontology terms, data,
documentation, or review. Contributors vote in the development group of their
project.

## 4. Bodies

The OEFamily has one decision-making committee, one advisory committee, and development groups.

### 4.1 OEFamily Steering Committee (OEFamily-SC)

The OEFamily-SC is the decision-making body for the framework as a whole. It
sets strategic direction and takes the binding decisions that concern the family
across projects.

1. Keep an overview of the OEFamily: its functions, components,
   responsibilities, and timelines, and related work in the field.
2. Support development: advise on priorities and keep the work sustainable
   through continued feedback and testing.
3. Mediate and decide: enforce the Code of Conduct in interpersonal conflict
   and decide content disputes escalated from the development groups.
4. Represent the OEFamily externally at conferences and in public, maintain
   networks, and communicate with funding bodies and ministries.
5. Develop the longer-term direction: pursue strategies to extend the
   functionality and identify future fields of application.

### 4.2 OEO Steering Committee (OEO-SC)

The OEO-SC guides the development of the Open Energy Ontology (OEO) and its use
across projects. Its role is advisory: it gives recommendations, guides basic
design decisions, maintains contact with external ontology teams and the OEO
user community, and serves as the first point for arbitration in OEO questions.
Binding decisions that reach beyond the OEO-DEV group are referred to the
OEFamily-SC (Section 5.4).

### 4.3 Development groups: OEP-DEV and OEO-DEV

Development takes place in specific groups: 
Currently, there are 3 active developer teams:
OEP-DEV for the Open Energy Platform, 
OEO-DEV for the Open Energy Ontology, and
open-mastr-dev for open-mastr. 
Each sets its own pace and organises itself. 
The groups work autonomously: they settle the technical and content
questions within their scope and involve the committees only when a question
exceeds that scope (Section 5.6) or when they seek advice or arbitration.

The members of a group are the people who work on it actively. 
The groups exchange progress and coordinate next steps, plan and distribute tasks, 
and reach decisions by consensus within their scope. 
A member who also sits on the relevant committee carries information both
ways and brings forward proposals or decisions that the committee needs to take.

## 5. Decision-making

### 5.1 Responsibility

Technical and content questions inside a project are settled by its development
group. Advice and recommendations on the OEO come from the OEO-SC. Binding,
framework-wide decisions rest with the OEFamily-SC. Where a question touches both
the OEO and the framework, the OEFamily-SC decides after hearing the OEO-SC.

### 5.2 Development groups: consensus and lazy consensus

Everyone present and actively contributing has one vote; the aim is consensus.
Between meetings, lazy consensus applies: a proposal is announced in the open
(issue or discussion) and carried out after 1 week unless a reasoned objection
is raised. Silence counts as assent; a reasoned objection returns the question
to discussion. If no consensus forms, the proposal and the objections go to the
relevant committee, the OEO-SC for OEO questions and otherwise the OEFamily-SC.

### 5.3 OEFamily-SC: voting

Before a decision, members receive enough information in time to decide. Each
member institution present has one vote. The committee can decide when at least
half of the voting institutions are represented. Members vote for, against, or
abstain. A proposal passes when more than half of the votes cast for and against
are in favour; abstentions count towards the quorum but not the result. A tie
counts as rejection; the proposal may be revised and brought again.

### 5.4 OEO-SC: recommendations

The OEO-SC reaches its positions by consensus and, where it needs to state one
clearly, by an indicative vote. Its output is a recommendation to OEO-DEV or to
the OEFamily-SC, not a binding decision. Questions that exceed the OEO-DEV scope,
for example changes to published ontology identifiers or to shared interfaces,
are passed to the OEFamily-SC together with the committee's recommendation.

### 5.5 Request for reconsideration by the Community Manager

Before an adopted decision takes effect, the CM may ask the committee to
reconsider it once. The request is made in writing and gives a reason concerning
consistency, sustainability, or effect on the community. It defers the decision
and reopens discussion. At the next meeting the committee decides again under
Section 5.3, and the earlier decision stands if it is reaffirmed. The request is
a suspensive step, used sparingly, and does not replace argument on the
substance.

### 5.6 Escalation from a development group to a committee

A question leaves the development group when at least one of the following holds:

- it affects more than the group's own project, such as shared interfaces or
  infrastructure, or other OEFamily components;
- it changes public contracts such as APIs, data models, published ontology
  identifiers, or URI and slug conventions;
- it commits the resources of several institutions or touches funding commitments;
- it changes policies, licences, or this governance;
- it remains contested within the group.

Where the group holds a consensus, it forwards the proposal as a strong recommendation.

## 6. Proposal process

Decisions in the sense of Section 5.6 are written up as an Open Energy Enhancement Proposal (OEEP). 
The mechanism follows the established pattern and is at
the same time the technical implementation in the Compendium (Section 8).

1. Draft. The proposal is written as a Markdown document from the template
   (`proposals/YYYY-MM-DD_oeep_topic.md`) and submitted as a pull request.
2. Discussion. Open commenting in the pull request and the linked GitHub
   Discussion, for at least 4 weeks.
3. Final comment period. A named responsible person summarises the state, its
   main points, compromises, and open objections, and starts the final comment
   period. Full consensus is not required; what is required is the
   absence of a strong, reasoned consensus against the proposal.
4. Decision. After the final comment period the responsible committee decides
   under Section 5.3 (OEFamily-SC) or gives its recommendation (OEO-SC).
   Outcomes are accepted, rejected, postponed, or returned to discussion.
5. Record. The outcome, date, and vote are recorded in the proposal and the
   minutes.

## 7. Amending this document

A change to this document is itself an OEEP (Section 6) and needs adoption by the
OEFamily-SC with a two-thirds majority of the votes cast for and against. A
change that concerns only the OEO also requires hearing the OEO-SC. Each adopted
change is versioned and dated in the change log.

## 8. Implementation in GitHub

The governance is kept in the OEP Compendium:

- `governance.md` is this document, the authoritative reference.
- `proposals/` holds OEEPs from the template, with an index listing status
  (draft, discussion, final comment period, accepted, rejected, postponed).
- `proposals/template.md` is the template for new proposals.
- `minutes/` holds the archived minutes of both committees and of the
  development groups where public.
- GitHub Discussions carry the discussion and final comment period, one thread
  per proposal, linked from it.
- Issue labels are used for tracking.
- Admins require review by the OEFamily-SC for changes to `governance.md` and `proposals/`.
