Distributed Datasets
---

Basically, we want to keep a clear separation between the data and the applications . The question is: How we accomplish this?

We want simple solutions, and we think that people can adopt something they already now, such as the filesystem metaphor. Each user might have a virtual file system that shows all their data about their own products in folders. They define data about their crops and prices in spreadsheet-like apps. 
 
Your Data
---
 
We want to allow variety, not another centralized repo. This means each node must be in control of their own data so no central control is required or enforced. Each node have the choice to provide or not the data. They have the freedom to take their data away if they want. 
 
This means that authentication is also decentralized, you will need to authenticate with the data sources, not the applications. Each agent has the full control of their data access policies, this means that each farmer can decide which data is public and which is not.  
  
Multicultural
---
 
We don't want to dig deeply into vocabulary variants in the first phase. But this is a huge subject in the food domain. Organic market products are named and organized differently in the different communities, for example in Peru there are more than 200 varieties of potatoes which cannot be mapped to the varieties existent in Europe. In this case  schemas need to be in constant evolution and maintained and mapped by the communities of users. This is a characteristic of gitHub, where code is in constant evolution, just like language is. A pull request and a merge is an implicit agreement process.

Github
---

So GitHub in this sense can act as a desentralized file system, where operations on this data can be described through hydra-like vocabularies just to be used by smart apps. People then can branch the data and operations, promoting reusability.

Probably we will need a tool to explore their data such as data-tank (http://thedatatank.com/). The applications themselves can be cloned so people can provide their own customizations of such applications (for example to build a new food store, with customized look and feel). To maintain interoperability, each github space might be a branch of a specific seed branch that contains the essential vocabularies (upper ontologies) to describe the basic information about agent and products.

Given that the farmers store their data in their own repositories, we have to choose the approach to access the data, either is cached in smart clients or is pulled into elastic search indexes or RDF triple stores. The data could be pulled when changes in the repository are detected (for example triggered by a commit). Both approaches have pros and cons and the one we choose will depend on the applications we'll build on top. (see: http://www.hydra-cg.com/spec/latest/triple-pattern-fragments/)

Complexity
---

Suppose an specialized application to visualize distribution chains. Since the repositories are distributed, we need indexes to track the information of the participants. Specialized directories, which constitute organizations themselves. how we keep this complexity low?


 
 
