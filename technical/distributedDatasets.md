Distributed Datasets
---

We want to keep a clear separation between the data and the applications. The question is: How we accomplish this?

We want simple solutions, and we think that people can adopt something they already know, such as the filesystem metaphor. Each user might have a virtual file system that shows all their data about their products in folders. They define data about their crops and prices in spreadsheet-like apps. 
 
Your Data
---
 
We want to allow variety, not another centralized repo. This means each node must be in control of their data, so no central authority is required or enforced. Each node has the choice to provide or not the data. They have the freedom to take their data away if they want. 
 
This means that authentication is also decentralized; you will need to authenticate with the data sources, not the applications. Each agent has the full control of their data access policies; this means that each farmer can decide which data is public and not.  
  
Multicultural
---
 
We don't want to dig deeply into vocabulary variants in the first phase. But this is a huge subject in the food domain. Organic market products are named and organized differently in the different communities; for example, in Peru, there are more than 200 varieties of potatoes that cannot be mapped to the types existent in Europe. In this case, schemas need to be in constant evolution and maintained and mapped by the communities of users. This is a characteristic of gitHub, where code is in continuous evolution, just like language. A pull request and a merge is an implicit agreement process.

Github
---

In this sense, GitHub can act as a decentralized file system, where operations on this data can be described through Hypermedia vocabularies just to be used by smart apps. People then can branch the data and services, promoting reusability.

We will probably need a tool to explore their data. The applications themselves can be cloned so people can provide their customizations of such applications (for example, to build a new food store, with a customized look and feel). To maintain interoperability, each GitHub space might be a branch of a specific seed branch containing essential vocabularies (upper ontologies) to describe the necessary information about agents and products.

Given that the farmers store their data in their repositories, we have to choose the approach to access the data, It is either cached in smart clients or is pulled into elastic search indexes or RDF triple stores. The data could be pulled when the repository changes are detected (for example, triggered by a commit). Both approaches have pros and cons, and the one we choose will depend on the applications we'll build on top. (see: http://www.hydra-cg.com/spec/latest/triple-pattern-fragments/)

Complexity
---

Suppose a specialized application to visualize distribution chains. Since the repositories are distributed, we need indexes to track the information of the participants. Specialized directories, which constitute organizations themselves. How we keep this complexity low?