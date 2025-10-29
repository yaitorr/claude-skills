# Strategy Document: Q3 Resource Allocation for Widget Owners
# Executive Summary
This document outlines our revised approach to the NodeJS upgrade initiative for widget owners. Given significant blockers and capacity constraints in Q2, we recommend pausing external communication about readiness until core dependencies are stable and upgrade requirements are clearly defined.
# Problem Statement
Throughout the NodeJS upgrade initiative, we have communicated to widget owners that "some work will be required" to adopt the changes. However, accurately scoping the effort and timeline has proven challenging.

****Related Initiative Tickets:****
* ~[AP-6155](~https://gbujira.oraclecorp.com/browse/AP-6155~)~
* ~[DSM-29919](~https://gbujira.oraclecorp.com/browse/DSM-29919~)~

****Key Blocking Issues:****

1. ****Resource Disruption:**** Original team members with institutional knowledge were affected by RIFs, creating knowledge gaps and onboarding overhead
2. ****Build Instabilities:****
   * The maestro service fails to build in `iad-dev` (~[DSM-31790](~https://gbujira.oraclecorp.com/browse/DSM-31790~)~)
   * Opattern Migration has introduced uncertainty around X-Web-SDK build capacity ([slack reference](~https://opower.slack.com/archives/C6ET4P613/p1761242523967859~))
3. ****Dependency Delays:**** Beta releases of core dependencies (maestro, x-w-g-c-t) remain in Q2 spillover, blocking experimentation with NextWeb artifacts including Widget Libraries and individual widgets
4. ****Knowledge Transfer:**** New team members require time to ramp up on the technical context

****Critical Question:**** Should widget owner teams continue allocating resources to this work, or should we adjust our approach?
# Strategic Principles
## 1. Show, Then Tell
We will complete beta releases of core dependencies and document required migration steps **before** requesting widget owner action. This approach increases trust and improves quarterly planning predictability for downstream teams. We must establish a clear understanding of changes required for Widgets and Widget Libraries—work previously attempted in Q3 (~[DSM-31540](~https://gbujira.oraclecorp.com/browse/DSM-31540~)~) but not yet delivered.
## 2. Dogfood Our Own Work
Our team now works more closely with widget owners than ever before. We will leverage these relationships to accelerate the process of identifying and documenting required code changes, using our own experience as a validation mechanism.

# Recommended Actions
## Primary Decision: Pause Readiness Signaling
****Action:**** Communicate to widget owners that preparation work is not yet complete. We will issue MOPEDs (Method of Procedure) documents only after achieving the following milestones:

1. Beta versions of build tools are published and stable
2. Required code changes are documented with concrete examples and effort estimates

****Concrete Action Items:****
* Draft communication to widget owners explaining the timeline adjustment and rationale
* Establish milestone criteria and success metrics for beta release
* Create MOPED template with required sections for widget migration guidance
* Schedule bi-weekly checkpoint meetings to track progress against milestones

## Address Blockers and Ensure Focus
****Priority:**** Team members dedicated to this initiative must have protected focus time. Further delays would compound technical debt and jeopardize Q4 delivery commitments.

****Resource Allocation:****
1. ****Cristian Lazo**** (Tech Lead): ≥80% dedicated capacity
2. ****Vitaliy Utkin****: Prioritized support to Cristian with escalation path for blockers

****Success Criteria:****
* Beta dependencies released by [specific date]
* Migration documentation completed with ≥3 widget examples validated
* Zero critical build blockers outstanding by end of Q3
