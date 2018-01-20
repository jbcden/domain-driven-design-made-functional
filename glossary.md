# Glossary

## Bounded Contexts

A kind of subsystem in the implementation. Each context represents some specialized knowledge in the solution.

## Business Process

Describes a goal that the business (rather than an individual user) wants to achieve. It’s similar to a [scenario], but with a business-centric focus rather than a user-centric focus.

## Command

a request for some process to happen, triggered by a person or another event. If the process succeeds, the state of the system changes and one or more Domain Events are recorded.

## Context Map

Shows the relationships between bounded contexts at a high level.

## Core Domain

Domains that provide a business advantage

## Domain

Is that which a domain expert is an expert in. These can often manifest as separate parts of a business.

## Domain Events

The starting point of all business processes. These can be thought of as triggers (i.e. you receive an email or a phone call). Since these events are triggers, meaning they have already happened, they should generally be discussed in the past tense.

## Domain Model

A set of simplifications that represent those aspects of a domain that are relevant to a particular problem. The domain model is part of the solution space, while the domain that it represents is part of the problem space.

## [Event storming]

A technique to discover the events in a domain. It generally works by gathering “Anyone who has questions, and anyone who has answers” into a room and having them post events and the workflows triggered by these events. These can then be further organized into timelines that are discussed etc.

<a name="scenario"></a>
## Scenario

Describes a goal that a customer (or other user) wants to achieve, such as placing an order. It is similar to a "story" in Agile development.

## Ubiquitous Language

The set of concepts and vocabulary that is shared between everyone on the team. This includes requirements documents, designs and source code. Bounded contexts can have their own dialects of the ubiquitous language, as certain terms may have slightly different meanings in different contexts.

## Use Case

Is a more detailed version of a scenario, which describes in general terms the user interactions and other steps that the user needs to take to accomplish a goal. 

## Workflow

A detailed description of part of a business process. That is, it lists the exact steps that an employee (or software component) needs to do to accomplish a business goal or sub-goal. We’ll limit a "workflow" to what a single person or team can do, so that when a business process is spread over multiple teams (as the ordering process is), we’ll divide the overall business process into a series of smaller workflows, which are then coordinated in some way.


[Event storming]: https://eventstorming.com
[scenario]: #scenario