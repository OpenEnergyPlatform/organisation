---
title: "OEFamily-SC Governance Update"
status: draft            # draft | discussion | accepted | rejected | postponed
body: OEFamily-SC        # responsible committee: OEFamily-SC or OEO-SC
authors:
  - "Ludwig, RLI>"
created: 2026-07-13
discussion: "<link to the GitHub Discussion thread>"
decided: ""              # date, filled after the decision
---

# Open Energy Enhancement Proposal (OEEP)

## Summary

This proposal establishes a documented governance structure for the Open Energy Family. 
It adopts `governance.md` as the authoritative reference and puts its
roles, bodies, and procedures into use.

## Motivation

The OEFamily has grown without a written governance. Roles and decisions exist
in practice, and the OEFamily-SC has taken decisions, but they are neither
documented nor transparent to people outside the immediate circle. An
undocumented structure is easy to run while the same few people are involved and
fragile once they change: there is no agreed way to reach a decision, to record
what was decided, or to change the rules themselves.
As the family and its funding context grow, this needs a stable and transparent
footing. The aim of this proposal is to provide one, without adding more
process than the work needs.

## Proposal

Adopt the governance documented in `governance.md` and put it into effect.

**Current state** 
- The structure is informal
- The OEFamily-SC decides in practice
- the OEO-SC has acted in an advisory role
- development happens in developer groups (OEP-DEV, OEO-DEV, open-mastr-dev).
- There is no defined quorum or majority, no record of decisions, no escalation rule between the
groups and the committees, and no procedure for changing the rules. 
- A veto for the Community Manager was proposed earlier but was rejected.

**Proposed state** 
- `governance.md` defines: membership and voting
- roles of the Community Manager, maintainer, and contributor
- decision-making committee (OEFamily-SC), advisory committee (OEO-SC), and
autonomous development groups (OEP-DEV, OEO-DEV, open-mastr-dev)
- decision procedures (consensus and lazy consensus in the groups, voting in the OEFamily-SC,
recommendations from the OEO-SC, and a request for reconsideration by the
Community Manager)
- criteria for escalating a question from a group to a committee
- the OEEP process for larger decisions
- and a procedure for amending the governance
- Minutes and decisions are published in the Compendium

**Difference** 
- The change moves the family from an undocumented arrangement to a written one: defined quorum and majority instead of ad hoc counting
- written and archived minutes instead of the etherpad
- explicit escalation criteria instead of intuition
- an amendment rule for detailed discussions

**Bootstrap** 
This proposal establishes the OEEP process and therefore cannot follow it. 
It is adopted directly by the OEFamily-SC, which already exists and
already takes decisions. From adoption, all further decisions follow the process
set out here.

## Impact

Immediate steps after adoption:

- Elect a Community Manager at the next OEFamily-SC meeting, for the one-year
  term defined in `governance.md`, Section 3.1.
- Put the OEEP process into use for decisions from adoption onward; this
  proposal is the first entry in `proposals/`.
- Begin keeping and archiving minutes for all bodies in `minutes/`, and extend
  the existing notes into the template format.

Repository and structure:

- Add `governance.md`, to the Compendium, with `proposals/` and `minutes/` and their templates.
- Add the issue labels `oeep`, and `governance`, and admin entry
  requiring OEFamily-SC review for `governance.md` and `proposals/`.

The proposal changes process, not code or data. It does not affect published
interfaces, ontology identifiers, or existing data models.

## Open questions

- Who is nominated as the first Community Manager.


## Final comment period

Opened on: YYYY-MM-DD. Summary by <name>:
- main points
- compromises reached
- open objections, if any

## Decision

- Body and date:
- Vote (for / against / abstain):
- Outcome: accepted | rejected | postponed | returned to discussion
- Request for reconsideration by the CM: none | raised (reason, result)
