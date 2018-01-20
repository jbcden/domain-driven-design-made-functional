# Introducing Domain Driven Design

## Main goal

In typical developmemt approaches, developers translate a domain experts expectations into code. This can result in mismatches between the actual ask and the result. When communication between developers and domain experts is cut, the result can be that the code drifts from the actual intention over time.

DDD proposes making the model of the domain expert, the developers and the source code *the same*. This eliminates the need to "translate" the domain expert's expectations and can help provide alignment.

## The how

DDD has guidelines for how to approach design:

- Focus on business events and workflows rather than data structures.- Partition the problem domain into smaller sub-domains.- Create a model of each sub-domain in the solution.- Develop a common language (called the “Ubiquitous Language”) that isshared between everyone involved in the project, and is used everywhere in the code.