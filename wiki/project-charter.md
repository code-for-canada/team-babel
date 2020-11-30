This page describes the Project Charter as outlined at the beginning of the Code for Canada fellowship. We acknowledge that some of the goals will be refined, altered, pushed back, and removed as the project is explored. For an up-to-date definition of the project, see the [Project Definition](https://code-for-canada.github.io/team-babel/wiki/project-definition)

## Background

The ESDC delivers programs to many clients (old age security, CPP, EI, student loans, RESPs, etc). These programs are subject to laws and policy, some of which dates back decades. To ensure compliance, the ESDC has operational guideline and directives on how to handle applications and claims. In many cases, this guidance is unclear, conflicting, and outdated. Making changes in one place can have unintended consequences elsewhere, and it is hard to predict how a change to a program will affect people.

The ESDC has begun a transformation project to change how it delivers benefits. The goal of the Benefits Delivery Modernization project (BDM) is a multi-year long initiative to modernize tools and processes that deliver important social benefits to the public.


## Goals

### High-Level Product Goal
Incrementally develop a solution that will allow us to detect changes to rules and predict impact on clients/society/operations, which will help identify policy gaps and priorities for policy changes, as well as potential improvements and automation. This general tool can be referred to as a 'Policy Difference Engine' (PDE).

We will be facilitating progress on this project in order to accelerate digital transformation in government by showing what's possible. There is a focus on delivering a concrete product that addresses an urgent need that can be used and tested by staff. A deadline for deliverables is August 21, 2021.

We also want to build digital capacity in government by helping to familiarize public servants with modern digital methods and tools through delivery and training. This involves creating a smooth transition and hand-off to the ESDC at the end of the fellowship.

At the start of the fellowship, the project is still in the very high-level stages, and the architecture is not yet known. 

### Policy Difference Engine
Team is exploring creating a policy difference engine tool that would be incrementally developed to allow us to detect changes to rules, predict the impact that changes to rules might have on clients/society/operations. First iteration is to develop or customize a tool that can read the various documents, generate a set of rules, and check for consistency, and the interdependencies between them focused on a single program. Ideally this would link to other tools (such as OpenFisca) to simulate the policy's impact on clients.


### Definitions of Done
- Level 1: Primary research has been done to inform a potential solution. High-level roadmap to create the engine
- Level 2: Low-fidelity mockup created to test and validate assumptions with end-users. Compares differences between wording and generated rules in various docs, tracks associations, finds contradictions, and looks for places where clarification is needed
- Level 3: Tool uses OpenFisca or other tools to simulate impact of changes to clients. Contains a way to associate cost with processing specific rules
- Level 4: Tool can generate rules by reading legs, regs, policies


### Potential Impact

Rules Module:
- When changing a rule, we need to know how it may be connected to other related rules. This is largely a manual process, which makes it challenging to keep up to date. We may be able to improve this by adding some degree of automation that could assist in various parts of the rule-making process, such as identifying related rules that must be checked for consistency. 

Cost Module:
- If we can estimate the cost involved with rule changes using simulations, then we can prioritize certain operations. There are some existing models used for this, but they are not very reusable.

Client Module:
- Using socioeconomic indicators, we may be able to forecast effects of policy change on the clients. This may include identifying impact of a change on client eligibility, cost savings for the client, time savings, etc. Every program has indicators that define the intended effect.

Service Impact Module:
- Integrate insights and data to show how rule changes will affect the ability to meet service targets, and identify other issues in the system (non-compliance, ineligible applications, missing info, etc)


## Other Considerations

### Security
This project has been scoped to specifically focus on publically available data. If using public data, then we can host the data in a cloud environment. 

