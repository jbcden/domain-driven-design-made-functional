# Introducing Domain Driven Design

## Main goal

In typical developmemt approaches, developers translate a domain experts expectations into code. This can result in mismatches between the actual ask and the result. When communication between developers and domain experts is cut, the result can be that the code drifts from the actual intention over time.

DDD proposes making the model of the domain expert, the developers and the source code *the same*. This eliminates the need to "translate" the domain expert's expectations and can help provide alignment.

## The how

DDD has guidelines for how to approach design:

- Focus on business events and workflows rather than data structures.- Partition the problem domain into smaller sub-domains.- Create a model of each sub-domain in the solution.- Develop a common language (called the “Ubiquitous Language”) that isshared between everyone involved in the project, and is used everywhere in the code.

### Events

Events can help us to understand how and why data is manipulated and for what purpose. The exact events can be determined through exercises like [event storming]. Gathering a list of domain events and how they interact will give us a skeleton for our application.

### Partitioning into subdomains

As with all software, dividing up our code into smaller chunks helps with organization and readability. In this case, subdomains represent parts of larger domain that have their own specialized knowledge, this can also mean that subdomains have their own subdefinitions within the [ubiquitous language].

### Bounded contexts

Bounded contexts can be thought of as subsystems of in our problem domain. Each of these have specialized knowledge of the domain.

### Ubiquitous language

It is important to have standardized terminology for discussing the domain. If people begin using different words interchangeably, the meanings of the words become blurred over time until no one knows *exactly* what a particular term means anymore. Subdomains can have their own "dialects" but this is to provide clarity within the subdomain, not to be used generally throughout the larger domain.

# Chapter 2 Understanding the Domain

When looking to understand a domain resist the urge to think about the underlying design (i.e. databases). Instead try to focus the workflow, events, and the inputs and outputs of each step.

Make sure to consider what makes data valid and consider that the fact that each step in a workflow is transforming the data flowing through it.



[event storming]: ../../glossary.md#event_storming