This page describes the Project Charter as outlined at the beginning of the Code for Canada fellowship. We acknowledge that some of the goals will be refined, altered, pushed back, and removed as the project is explored. For an up-to-date definition of the project, see the [Project Definition](https://code-for-canada.github.io/team-babel/wiki/project-definition)

## Background

The ESDC delivers programs to many clients (old age security, CPP, EI, student loans, RESPs, etc). These programs are subject to laws and policy, some of which date back decades. To ensure compliance, the ESDC has operational guidelines and directives on how to handle applications and claims. In many cases, this guidance is unclear, conflicting, and outdated. Making changes in one place can have unintended consequences elsewhere, and it is hard to predict how a change to a program will affect people.

The ESDC has begun a transformation project to change how it delivers benefits. The goal of the Benefits Delivery Modernization project (BDM) is a multi-year long initiative to modernize tools and processes that deliver important social benefits to the public. This project fits in with the initiative.

It is also important to note that the department is experiencing significant changes due to the Covid-19 pandemic, so there is an ongoing need to support efficient legislation and policy development.


## High-Level Goals

### Long-Term Vision
Incrementally develop a solution that will allow us to detect changes to rules and predict impact on clients/society/operations, which will help identify policy gaps and priorities for policy changes, as well as potential improvements and automation. This general tool can be referred to as a 'Policy Difference Engine' (PDE).


### Product Delivery
We will be facilitating progress on this project in order to accelerate digital transformation in government by showing what's possible. There is a focus on delivering a concrete product that addresses an urgent need that can be used and tested by staff. While the delivery of the product as outline in the charter is not fixed, fellows will work on a roadmap, refine the design, and prioritize components of the project. A deadline for deliverables is August 21, 2021. 

The purpose of this project is to improve policy and service agility. There are no hard and fast target dates, instead, the plan is to test and use the tools together as they are developed to provide supporting analysis to other transformation initiatives.

### Building Digital Capacity
The fellowship will build digital capacity in government by helping to familiarize public servants with modern digital methods and tools through delivery and training. This involves creating a smooth transition and hand-off to the ESDC at the end of the fellowship.

The fellowship team will work as a dedicated, self-empowered team following agile principles. Fellows will use modern design and development and processes throughout their residency. They will conduct user research and develop iteratively, and will make their work as open and transparent as possible.

By showing what is possible through prototyping, the work done by the fellows will serve as a use case for future work at ESDC. The goal is to create processed that can be replicated once the fellows leave. In order to enable product sustainability, fellows will make choices that will enable their product to be maintained by the government after they complete their fellowship. This means taking cost, government capacity, and training needs into account when making a selection.


## Policy Difference Engine

### First Iteration
At the start of the fellowship, the project is still in the very high-level stages, and the specific architecture is not yet known. This may be mitigated by having the project run somewhat independently.

The first iteration of the PDE is to develop or customize a tool that can read the various documents, generate a set of rules, and check for consistency and interdependencies between. This would focus on a single program. Ideally this would link to other tools (such as OpenFisca) to simulate the policy's impact on clients.

### Definitions of Done
- Succeeded (-): Primary research has been done to inform a potential solution. High-level roadmap to create the engine.
- Succeeded: Low-fidelity mockup created to test and validate assumptions with end-users. Compares differences between wording and generated rules in various docs, tracks associations, finds contradictions, and looks for places where clarification is needed.
- Succeeded (+): The tool uses OpenFisca or similar tools to simulate the impact of changes to the policy’s basic parameters on clients. The tool Contains a way to associate cost with processing specific rules.
- Epic: Tool can generate rules by reading legs, regs, policies.
- Output: A basic policy difference engine for one or more programs.


## Impact

### Rules Module
When changing a rule, determine how that rule may be connected to other rules. This is largely a manual process, which makes it challenging to keep up to date. Define a process for:
- Identifying & reading legislation, regulations, policies to generate rules (or build on the rules used for systems)
- Analyzing the rules for contradictions and linkages
- Determining how strict the the process around changing a given rule is

Notes:
- Ensure that any solution is scalable and can keep up with continuously changing rules.
- Some of this may be automated using machine learning techniques, although prior work in this area appears to be mainly academic.

### Cost Module
Calculate the cost of changing rules (how much staff time needed, payments triggered, volume of requests generated). If we can estimate the cost involved with rule changes, it can help prioritize certain operations for optimization. There are some existing tools used for this, but they are not in a reusable form. This module could be built in a variety of tools, but the output would have to be combined with that of the client impact analysis to gain a fuller picture of costs benefit. 

### Client Module
Forecast effects of a policy change on clients in terms of socio-economic indicators and impact on specific types of clients defined by the Journey Mapping program.
- Which rules impact client eligibility and benefits the most
- Identify policy gaps - who needs a benefit but is not being served
- Benefit cost/savings from adding/removing a rule
- Client compliance costs associated with the rule
- Policy outcome impact for clients based on performance indicators

Every program has a series of policy indicators that show the intended effect. These are available on [GC Info base](...) or by in program information files maintained by te department.

There are existing models used to measure client impact, but many are created as one-offs and then discarded. Furthermore, they aren't built to measure how policies impact specific clients. This tool would consolidate/integrate them with a model of how specific clients and personas used in the Life Journey Mapping team, are affected by the policy.

Similar work has been done by some jurisdictions using OpenFisca, and other tools.

### Service Impact Module:
Integrate insights and data from Service Analytics Evidence Base to show how rule changes will affect the ability to meet service targets. Associate various indicators with specific policies. Examples of indicators:
- Integrity issues of non-compliance
- Common errors
- Ineligible applications
- Missing info
- Business expertise/Functional guidance interventions

Based on these associations, provide evidence needed to recommend priorities for policy changes, channel improvements, and communications to address the most common issues.

Expansions:
- Could be expanded to allow a trade-off between service standards and costs to be calculated.
- Could look at broader set of indicators to identify which rules are hardest for clients and agents to follow
- As the Service Analytics Evidence Base grows, it can be used to calibrate the simulation and check the results against real experience.


## Limitations and Risks

### Architecture
Since BDM has just begun its initial developments, it will not be possible to build project components that fit explicitly in the BDM architecture because the architecture is not yet known. 

To mitigate this, the project may run independently of the major product roadmap. While it is broad in scope, the intention is to build one or two of the modules, sufficient to demonstrate a real-world application for the tool’s analytical ability, that policy analysts can use to support them in their work if it is just another support and not a complete calculator. 

Scoping will need to be done by the fellows and the team once the project starts to determine feasibility and which tools are required. 

### Data Access
As long as the data being used is public, there will be no issue with hosting in a cloud environment, however, ESDC would need the discretion to determine public access rights to which information. This project has been scoped to specifically focus on publically available data, so it can be hosted in a cloud environment. 

If part of the policy impact simulation were to be made public, it could be used by public policy researchers across Canada to model better proposals, and they could help expand the model. However, certain info about costs and metrics may be considered sensitive, and could mislead Canadians about the department's capacity if not accurately simulated.

### Timeframe
Depending on how long the project activities last, there is a risk there is insufficient coverage and absorption time for ESDC resources to internalize their skills. Many ESDC resources have multiple priorities surrounding the BDM project and other related program mandates. Context shift may make it impossible for all resources to absorb new digital principles and skills.

