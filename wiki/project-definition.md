This page outlines the evolving definition of the work being done by the team. For original project charter, [visit this page](https://code-for-canada.github.io/team-babel/wiki/project-charter).

See background information about the project here (add link)

## Approach

### Gathering Evidence
We have analyzed the project charter and began the process of refining it down to a more concrete deliverable.

This analysis consists of ongoing interviews with potential stakeholders and allies, as well as ongoing research into the problem space. We have been looking for relevant prior work both internal and external to ESDC related to the various modules outlined in the original charter. Insights gained from the interviews and research have driven the refinement of the charter.

In the early stages we have focused heavily on aspects of the rules module and client module, and have made progress on identifying a set of concrete deliverables.

### Rules as Code
A key aspect of the problem space is the area of written legislation, regulations, and policy, which we will gather here under the term "written rules". These rules are written in natural human language, and in large part were not written with the purpose of being machine-consumable. Progress on many aspects of the Policy Difference Engine may require these rules to be in a machine-consumable form, though there may be some notable exceptions. This machine-consumable form is sometimes known as 'Rules as Code' or RaC (often closely related to the idea of computational law). If a written rule can be reliably converted to RaC, then we can take advantage of many automated processes. 

### Users
The process of identifying key users and stakeholders is ongoing, but one important target user of the PDE will be those involved in the creation of rules. This may include, but is not limited to, economists involved in research as well as people at the program management level who write more specific rules based on results of research. While we continue to refine these users, we will group them under the label of "Rule Writers".

A potential (simplified) use case for the PDE could be as follows:  A rule writer would like to measure the impact of making changes to a policy regarding eligibility of an  allowance for a parents of children with a disability. Suppose one requirement is that the child must be under the age of 17 for the parent to qualify. The rule writer would like to investigate the impact of changing the age threshold to 18. We've identified two concrete aspects from the PDE that would align with points of friction involved in a use case such as this: The Rule search engine and the Simulation engine

## Rule Search Engine
An initial point of friction is to determine whether or not making this change might impact other rules. They may collaborate with policy experts and do some independent research. There may be an opening here for a tool that facilitates this process. This could take many forms. One potential concrete solution for example may be a web-based search engine that inspects a targeted rule and searches a database for related rules that may also be impacted by the change.

The benefit to this is that the rule writer would be able to spend less time manually analyzing documents and rules that may be unrelated to the change and could instead focus on the rules that are determined to be relevant.

### NLP
Without stepping too far into a concrete solution, a project like this may involve machine learning, and more specifically Natural Language Processing (NLP). This is a subfield of AI that involves analyzing and producing human language. For the purposes of this tool, there may be a use case where it could parse through existing rules and identify which are relevant to the targeted rule. This technical aspect will require more investigaton and research, but this is a potential starting point. 

### Considerations, Next Steps, Discussion Points
- Any solution must be scalable and adapt to a changing reality. We must be careful about introducing any new "source of truth" for rules. It would be preferrable to integrate into an existing system (or multiple systems)
- This component does not necessarily require any involved rules to be encoded into a RaC format, although some basic structuring will be needed. 
- The project charter discusses first steps of the PDE as focusing on a single program. While we may be able to narrow the scope to a subset of programs, the goal of a search engine like this would be to search through a wider array of rules. 
- Much of this hinges on extensive user research. We will want to get in touch with a large sample of these rule writers and learn the current processes involved in handling the problem of finding related rules.


## Simulation Engine

A second point of friction in implementing a rule change is that rule writers would want to know how the change might impact the public, mainly those that the rule targets. If we have a rule that has been converted to RaC, then we can build sample households and run simulations of the change against these households, to see how it affects certain parameters, such as overall income.
** Need a more concrete example here...

### LexImpact and OpenFisca
An example of this simulation is the [LexImpact project](https://leximpact.an.fr/ir) from France. This application focuses on income tax rates. The rule writer can create a number of sample households with different configurations of people having different relevant characteristics (65+, veteran, has a disability, etc), and specify their monthly income. The application allows the rule writer to toggle the various tax rates, and then the application calculates the amount that the model household would owe in income tax.

This project is built using OpenFisca, which is an open-source engine that allows you to work with RaC. 

For the fellowship, we may want to consider a similar approach. The exact service that we target will likely be different, but the concept would be similar:
- Translate the written rule to RaC and encode it in a system such as OpenFisca
- Build a series of sample personas or households that would be affected by the rule change
- Toggle the values in the rule to assess the impact on the personas

## Next Steps

### Service and Cost Modules
This current definition primarily addresses components of the Rules module and the Client module. While concrete projects are beginning to develop for these modules, we want to do further exploration on the Service and Cost modules. Again, this will be driven by interviews with relevant stakeholders as well as research on prior work.

Having a more concrete plan for each module will make steps towards a more complete roadmap for the full PDE as defined by the project charter.

### Choosing a Program
Depending on the module that we address for the fellowship and further research we do into the problem space, we may be focusing on a very narrow service ...


### Interview Rule Writers

...
