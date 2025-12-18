# Architectural Modularity

https://developertoarchitect.com/lessons/lesson211.html

- Modularity is about a single system into smaller independently deployable units of software
- Granularity is about the size of those pieces
- `Embrace modularity, but beware of granularity`

<br>

- Common right now in industry to take monolith and break into something like service based, microservices, event driven, etc
- Why is achitectural modularity important?
    - `Maintainability` - ease of which to locate and apply changes in our system
        - Difficult in a monolith sometimes
    - `Testability` - ease of testing and completeness of testing
        - In a large monolith, hard to know if anything else is broken in the system
        - With modularity, change in scope is much smaller and testing surface is much smaller
    - `Deployability`
        - Frequenecy, risk of deployment, process of deployment
            - With monolith, process can be long and complicated
            - With modularity, deployment unit it smaller, process of deployment is easier, frequency is faster, risk is lower
    - `Scalability`
        - With monolith, have to scale everything even though additional scale may only be for one small function
    - `Fault Tolerance`
        - Entire monolith can be brought down and all functionality is lost
        - With modularity, only one service will go down

- Architectural modularity is great until you get some spaghetti beteween services 

![](./images/21.png)

- When this happens, you lose maintainability, testability, deployability, scalability, fault tolerance