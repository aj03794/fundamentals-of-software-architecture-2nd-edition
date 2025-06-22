# fundamentals-of-software-architecture-2nd-edition

## Chapter 1 - Introduction

### Defining Software Architecture

- 4 dimensions
- Software architecture of a system consists of an `architecture style` as the starting point, combined with the `architecture characteristics` it must support, the `logical components` to implement its behavior, and finally the `architecture decisions` to justify it

![](./images/2.png)

- `Architecture characteristics` define the `capabilities` of a system (aka the `-ilities`) and the criteria for success
    - Describes how the system should *behave* 
    - Availability, reliability, testability, scalability, security, agility, fault tolerance, elasticity, recoverability, performance, deployability, learnability...
- `Logical components` define its *behavior*
    - Defining these is one of the key structural activities for architects

![](./images/3.png)

- One required architectural characteristics are identified and the logical components needed, you can use this as a starting point to choose an appropriate `architecture style` for implementing the solution

![](./images/4.png)

- The fourth dimension is `architectural decisions`, which define the rules for how a system should be constructed

### Laws of Software Architecture

- Law 1: Everything in software architecture is a trade-off
    - If you think you've identified something that isn't a trade-off, you haven't identified the trade-off yet
    - Trade-off analysis is an ongoing activity
        - There is no one size fits all solution for all systems
        - Every situation requires us to re-evaluate those trade-offs
- Law 2: Why is more important than how
    - Architecture is broader than just a combinatin of structure elements
- Law 3: Software architecture decisions aren't binary but rather exist on a spectrum between extremes
    - Why an architect made an particular decision includes the trade-offs they considered
    - Seeing an architecture you may be able to understand *how* it works, but might struggle with *why* the previous architect or team made certain decisions

### Expectations of a an Architect
- Make architecture decisions
- Continually analyze the architecture
- Keep current with latest trends
- Ensure compliance with decisions
- Understand diverse technologies, frameworks, platforms, and environments
- Lead a team and possess interpersonal skills
- Understand and navigate organizational politics
    - Almost every decisions an architect makes will be challenged
        - Must justify those decisions

## Chapter 2 - Architectural Thinking

- Image helping decide if something is architectural or design
    - These things are usually on a spectrum

![](./images/1.png)

- Technical breadth becomes more important than technical depth
    - Some areas you will specialize in either out of need or out of interest

## Chapter 4 - Architectural Characteristics Defined

- `Structual design` is one of the key activites for software architects 
    - Two sub-activities (performed in any other or in parallel):
        - Architectural characteristics analysis
        - Logical component design
- `Problem domain` aka `domain` is the list of requirements required to solve some problem
- Software solution consists of both domain requirements and architectural characteristics

### Architectural Characteristics and System Design

- To be considered an architectural characteristic, a requirement must meet 3 criteria
    - Specify a nondomain design consideration
    - Influence some structural aspect of the design
    - Be critical or important to the application's succes
- *Nondomain design consideration*
    - Structural design in software architecture consists of two activities by an architect
        - Understanding the problem domain and uncovering what kinds of "-ilities" the system needs to support to be successful
        - Domain design considerations cover behavior of the system and architectural characteristics define the "-ilities" (aka capabilities)
    - Design requirements specify WHAT the applixation should do
    - Architectural characteristics specify HOW to implement the requirements and WHY certain choices were made