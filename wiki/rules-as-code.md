This is a list of resources  related to the concept of Rules as Code

## Concept

### What is Rules as Code
- Approach to developing rules designed to improve policy outcomes
- Sometimes synonymous with computational law
- Can involve multidisciplinary teams drafting rules in both natural language and code at the same time
- It is a general principle that can have many applications: Contracts, organizational policies, board games, etc.

### Background
Traditional models of creating, managing, and improving government rules (policy, legislation, regulation, etc) were developed for a non-digital environment. This can result in mismatch between intent and implementation (sometimes called the implementation gap).

As legislation, regulation, and policy changes, we want to be able to measure the impact that the change will have on the population that the rule affects. If a rule can be made machine-consumable, then it can take advantage of many automated processes. This includes the ability to run simulations on sample individuals/households/populations to see how the change might affect them. This is a big step towards evidence-based policy.

The process of converting written rules to 'Rules as Code' will be a collaborative process between technologists and legislators, since it is important to preserve the legal intent of the law that is being encoded. This process may also serve to highlight ambiguities that are already present in the written law, and motivate the idea of a multi-disciplinary approach when creating new rules.

### Legal considerations
RaC is closely aligned with the concept of [Legal Formalism](https://en.wikipedia.org/wiki/Legal_formalism), which is the idea that laws should be clear and uncontroversial, so they can be applied unscrupulously. This is in contrast with legal realism, which permits arbitrary discretion in legal judgment to balance interests of affected parties on a case-by-case basis. 

This means that RaC may be more relevant in a civil law context, where laws are taken more literally. It is less relevant to common law, where judicial innovation is the norm. This is an important consideration. Computational law is only as powerful as deductive reasoning in general, but in reality, laws are more complicated than this and open to interpretation. 

Relevant source: http://complaw.stanford.edu/readings/complaw.pdf

### Ethical Considerations
Since we are modelling humans, we need to be conscious of the data we use to build the model and also the data that we **omit** from the model. If we leave out some important piece of data when modelling humans, we risk ignoring certain groups.

***

## Previous Work

### New Zealand Case Study
- Link: https://www.digital.govt.nz/dmsdocument/95-better-rules-for-government-discovery-report/html
- Related Article: https://apolitical.co/en/solution_article/new-zealand-explores-machine-readable-laws-to-transform-government
- LabPlus: https://www.digital.govt.nz/blog/labplus-expanding-the-service-innovation-tookit/

3 Weeks exploration to identify opportunities and challenges of creating human and machine-consumable rules for effective service delivery.

Important findings:
- It is difficult to produce machine-consumable rules if policy has not been developed with this output in mind
- Not all legislation is suitable for Rules as Code, but a multidisciplinary approach can assist in making clearer rules

Questions and next steps:
- Identify legislative barriers to data and digital transformation to inform development of standard clauses
- Work closely with other D7 countries: Canada, Estonia, Israel, New Zealand, South Korea, Uruguay, UK

### Blawx

Blawx is a free open-source web tool for encoding rules, created by Jason Morris. It is based on blockly, which is descended from MIT's scratch: 
- https://law.mit.edu/pub/blawxrulesascodedemonstration/release/1
- https://www.blawx.com/

## OpenFisca

[OpenFisca](https://code-for-canada.github.io/team-babel/wiki/openfisca) is an open-source platform for building RaC engines.

***

### More Resources

MIT Computational Law Blog: https://law.mit.edu/

BetterRules: https://github.com/BetterRules/example-rules-as-code

Scott McNaughton:
- https://medium.com/@mcnaughton.sa/week-50-reflections-on-rules-as-code-5878ff42d43c
