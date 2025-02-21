# Knowledge gained from Domain Driven Design by Eric Evans

This is a really worth reading book which introduces and tells the importance of having the domain understanding for a developer to avoid gaps between expected vs actual design and working.

## Chapter 1 - Putting Domain model to Work
### Crunching Knowledge
In this chapter, the author empasizes on the importance of domain knowledge for the developer. With the vast information, the activities and the complexity each domain holds. It is often difficult to produce the same functionalities with the software until and unless it is simplified and organized in such a way that the domain experts is connected to the purpose of what software does.
The establishment of such understanding is very important for a software to represent the model.

The domain model is not a particular diagram but the intent to convey and communicate what is written in code. It is also the link between the implementation and interpreting the code,
It is the language that everyone would speak be it a technical person or domain expertise. This way they would get together and have effective collaboration to ensure and have constant refinement of the model to get the final output.

The author then takes into a good story where we understand the importance of model that establishes communication between developers and the PCB design experts and get to the common language to get the final output.
The pictorial representation of what they talk and how the data flows is crucial to get the feedback and refine the product or the software.
He also states that the success of the software was with binding model and implementation as soon as possible to reach the milestones and the prototype that was created helped experts in understanding what software can do.
Knowledge Crunching is language combined with sketches and brainstoriming attitude. This is usually led by developers and domain experts. then prototypes are created and seek feedback from experts.

In parallel with model changes, the developers refactor the implementation to express the model and giving the application use of that knowledge.
The author then explained the importance or how fruitful it would be if the developer understand and modularize the domain knowledge in applying to the application code.

### Communication and the Use of language
In the agile world, the communication mostly happens with the code and tests  of the code. Major gap between the developers and domain experts would be the language barrier where they use lot of jargons that developers might not aware of and domain experts may bot understand technical terms.
Translation is not always accurate and hides disconnects in understanding between the domain experts and developers.

The model based language should provide the primary language among developers to describe artifacts in the system and also to describe tasks and functionality. With this commitment, as the developers and domain experts speak in this language and constantly find the gaps and update the model terms with the new terminologies. The better would be the understanding between them and will develop the final product. If something is not working out, the alternative model can be found. then refactor the code, rename the classes, methods and models.

The LANGUAGE is the primary carrier of the aspects of design that don't appear in code - large-scale structures that organize the whole system and BOUNDED CONTEXTS that define relationships of different systems and models.

Too much language also causes ambiguity and miscommunication. For the model to speak out visually which brings the attention of both the parties and concentrate on the exct functionality each one is speaking with the terms that each one are aware of.
Play with the model as you talk about the system. Describe scenarios out loud using the elements and interactions of the model, combining concepts in ways allowed by the model.

The domain experts can use the language of the model in writing use cases and can work even more directly with the model by specifying acceptance tests.
With UBIQUITOUS LANGUAGE, conversations among the developers. among the domain experts and expressson in the code itself are all based on the same language derived from a shared domain model.

#### Documents and Diagrams
Informal UML diagrams in a discussion could be a great start as we talk through the discussion. a digram can be changed as people try different thought experiments and sketch takes on some of the fluidity of sopken words.
The author also explains the importance of UML diagram which represent the model and not the code.

> The model is not diagram but the diagram help communicate and explain the model.

The design document should explain the concepts of the model with sketches and the UBIQUITOUS LANGUAGE. If the document does not have the terms that is used in the project it is not meant for the purpose. By keeping up to date and allows other documents like requirement specification to be more precise.. this can be used to describe such a scenario in terms that directly connect to the MODEL-DRIVEN DESIGN.
#### Explanatory Models
Explanatory models provide the freedom to create much more communicative styles tailored to a particular topic. 

### Binding Model and Implementation
The author explains with an example how the model with lot of associations could not solve the purpose of the developers creating objects if they do not know the language.
Analysis model is the product of analyzing the business domain to organize its concepts without any consideration of the part it will play in software system. But here the design is not based on model so knowledge crunching happens. An analyziz must capture fundamental concepts from the domain in a comprehensible expressive way. 

MODEL-DRIVEN DESIGN discards the contrast between design driven vs the model. The ideal design should retain as many conecpts of the model as possible, as literally as possible. But this requires hard thinking and multiple iterations to achieve this.

> Design a portion of the software system to reflect the domain model in a very literal way, so that mapping is obvious.  Revisit the model and modify it to be implemented more naturally in software. Demand a single model that serves both purposes well. Have one model and tie the implementation slavishly to it. To do this usually requires software development tools and languages that support a modeling paradigm, such as object-oriented programming.

Development becomes an iterative process of refining the model, design and code as a single activity 

#### Modeling Paradigms and Tool Support
To support the MODEL DRVEN DESIGN, the tool should represent the concepts in the paradigm. Object- Oriented programming is powerful because it is based on modeling paradigm and provides implementations of the model constructs. 

Procedural languages often support complex data types that begin to correspond to more natural conceptions of the domain, but these complex types are only organized data, and don’t capture the active aspects of the domain.

The author then explained/ built the model based PCB design and worked through the approach of building with the language that is used in PCB design. They created classes and the objects that represent model driven design and included the constraints on combining rules and other enhancements. The other design he proposed was for testing where the components are broken into well - defined interfaces that can be unit tested.

I like this point where the author with an example shares the importance of model representing the design. When a design is based on the model that reflects the basic concerns of the user to a greater extent than with other design approaches. Revealing the model gives the user more access to the potential of the software and yields consistent, predictable behavior.

The Author also gives example of the development with out the knowledge of model could give the result that is not expected. So this shows the importance of the developer being involved in model development  and use the models to adopt it to the implementation. The implementation changes should reflect in the model and model changes should reflect in implementation. So this emphasizes the programmers are modelers.

> Procedural languages often support complex data types that begin to correspond to more natural conceptions of the domain, but these complex types are only organized data, and don’t capture the active aspects of the domain.

## Chapter 2 - Building Blocks of a Model - Driven Design
### Isolating the domain
Decoupling of the domain models from the other functions of the system is important. 
In the layered architecture where we have UI layer to be interacted with the clients. Suppose there is some business logic in the behavior of UI widgets and database scripts. As the code increases, increases the complexity and changing business rules might require tracing the UI code and database code. 

Creating programs that can handle very complex task calls for separation of concerns allowing concentration on different parts of the design in isloation.

* User Interface  - Responsible for showing the info to the user and interpreting the user commands.
* Application layer - Defines the jobs that software is supposed to do and directs the expressive domain objects to work out problems.
* Domain Layer - Responsible for representing the concepts of the business, information about the business situation and business rules.
* Infrastructure Layer - Technical capabilities to support higher layers

The author explains the seperation of concerns at each layer and dividing the responsibilities are important. Here it clearly emphasizes on the boundaries of each layer. For instance, sending an email. The domain layer is only concerned about initiating the request with content to be sent via mail but it is not worried about how it is sent. It is up to the infrastructure layer to send the mail to the concerned parties.

With the current frameworks make the solution such that the domain models should not be buried under the framework related objects which will hinder the performance of the application. The business objects should be readable and expressive of the purpose 

#### Domain Layer is where model lives
The domain layer is the manifestation of that model and all directly related design elements. The design and implementation of the business logic constitutes the domain layer. In model driven design, the software constructs of domain layer mirror the model concepts.

the author calls Smart UI Anti Pattern where layered architecture is not applicable to a simpler project which has simple flow and need not be separated into layers. In this case, the model driven approach may not be the right way to do as it imposes complexity

#### A model expressed in software
In model driven approach, the main aim is to map the model with the implementation which means the associations to be exactly represented.  the author expresses 3 patterns of model elements that express the model 
* Entities
* Value Objects
* Services

The actions or operations can be clearly called as Services. But there is confusion between Entities vs Value Objects. there are modules that improves low coupling and high cohesion. 
#### Associations
The interactions between modeling and implementaion is tricky with the associations between objects. Suppose a model shows association between customer and sales representative. We abstract them as real people and think as 2 java objects or encapsulation of database lookup or some comparable implementation.
##### 3 ways of associations make tractable
* Imposition of the traversal direction -> Bi directional are tricky to implement as both objects can only be understood together.
* Addition of a qualifier, effectively reducing multiplicity -> Looking deeper we can get some qualities which reduces associations one-to - one and embeds important rule into model.
* Elimination of non essential associations -> constraining associations make them simpler to implement

##### Entity
  Entity is the object defined primarily by its identity. I really like this point by the author where the Class definitions, responsibilties, attributes and associations should revolve around who they are, rather than the particular attributes tey carry which might change but the identity of who they are would not change. For example, a customer information has name and phone which cannot be treated as entity. Customer ID which is unique would be the ENTITY.

  Each entity must have an operational way of establishing its identiy with another object. But in case of distributed system where the same instance is transferred over network or other datbaase the identity is lost. Sometimes the combinations of attributes can be guaranteed to be unique within the system and it provides unique key for the ENTITY. Once the symbol which is unique is attached to the instance it is immutable and will never be changed.

##### Value Objects
An object that represents a descriptive aspect of the domain that has no conceptual identity is called a VALUE OBJECT. It represents what they are instead of who they are. One good example that I liked helped me understand is the route from LA to SFO via Pacific Coast HighWay. LA, SFO and Highway are Entities where as the route object is the VALUE OBJECT which points to the entities. It can also be assemblage of other VALUE OBJECTS. They are often passed as parameters in messages between objects. A person may be modeled as ENTITY but the person name is VALUE. 

These attributes should be treated as immutable. This allows the software to allow sharing the same refreence and passing safe and do not disturb the original state of the attributes. On the other hand, there might be cases where it should be mutable. For Instance, object creation or deletion is expensive or replacement rather than modification will distrub clustering. As long as VALUE OBJECT is immutable, change management is simple.

##### Services
A SERVICE is an operation offered as an interface that stands alone in the model without encapsulating state as ENTITIES and VALUE OBJECTS do. They are common patterns in technical framwworks but they can also apply in the domain layer.
The service emphasizes the relationship with other objects. The characteristics of good service is 
* relates to a domain concept that is not part of entity or value object
* Interface is defined in terms of other elements of the domain model
* The operation is stateless -> any instance can use it and does not affect behavior

The fine grained domain objects can contribute to knowledge leaks from the domain into application layer . Medium grained stateless services can be easier to reuse in large systems because they encapsulate significant functionality behind simple interface.
##### Modules
The modules in the domain layer should emerge as a meaningful part of the model telling the story of the domain on a larger scale. there should be low copuling and high cohesion within them.

Whenever two model elements are separated into different modules, the relationships between thembecome less direct and increases the overhead of understanding their place in the design. Low coupling between MODULES minimizes this cost, and makes it possible to analyze the contents of one MODULE with a minimum of reference to others that interact.
I like the way the author describes modules as a way of communication mechanism which drives the meaning. If the classes are together inside a module. Think of it as together they are working on a purpose.

The Module should reflect insight into the domain. Modules will also evolve with the model and the code. 

The author presented an interesting scenario where we have been using the frameworks that we seperate the layers to talk to database and business logic and the functional logic to supply to the presentation layer. But according to domain driven design the data should bind with the logic that uses them, In this case, it is not possible and the division or the packages are based on the layers and not the functionalities. In this case, dividing into modules and each module having the layers will make it more complex.

In the above case, the code will not reveal the model and the domain developers wil lose the ability to chunk the model into meaningful pieces. so there should be some tradeoffs in this case. The author suggests to Choose a minimum of technical partitioning rules that are essential to the technical environment or actually aid development.

> Unless there is a real intention to distribute code on different servers, keep all the code that implements a single conceptual object in the same MODULE, if not the same object.

Use packaging to separate the domain layer from other code. Modularity becomes more crutial as the design gets bigger and more complex

The ENTITIES, VALUE OBJECTS and their associations, along with a few domain SERVICES and the organizing MODULES are point of direct corresspondence between the implementation and the model.


### Modeling Paradigms
Object oriented programming helped the developers in achieving the model based approach for the applications. But the object creation should be used wisely. While object models address a large number of practical software problems,  A knowledge-rich domain model contains explicit rules, yet the object paradigm lacks specific semantics
for stating rules and their interactions.

This is something that got my atttention of what the author is saying that Suppose there is a rules engine for which we may not use object paradigm but mixed up the declarative way of programming. On adding up more rules and whcih is not in sync with the model definitely looses the synchronization with object system. When the domain model is bridging two paradigms, it is crucial to keep it cohesive, showing the relationships between, in this example, the rules and the objects. It is important to continue to think in terms of models while working with rules. Otherwise, the data and the rules become unconnected. 

### Lifecycle of the Doman Object
Most of the objects created are transient and they gets garbage collected after the life cycle of the object is ended.
There are 3 patterns to address problems with the maintenance of object
* AGGREGATES tighten up the model itself by defining clear ownership and boundaries
* FACTORIES to create and reconstitute complex objects
* REPOSITORIES address the middle and end of the lifecycle, providing the means of finding and retrieving persistent objects while encapsulating the immense infrastructure involved

> Modeling AGGREGATES and adding FACTORIES and REPOSITORIES to the design gives us the ability to manipulate the model objects systematically and in meaningful units throughout their lifecycle.

#### AGGREGATES
- It is difficult to guarantee the consistency of changes to objects in a model with complex associations.
- To address the issues that occurs with maintaining the complex associations and also adhering to the model which represents domain knowledge, we need an abstraction for encapsulating references within the model.
- An AGGREGATE is a cluster of associated objects that we treat as a unit for the purpose of data changes.
- Each AGGREGATE has a root and a boundary. The boundary defines what is inside the AGGREGATE.
- The root is a single specific ENTITY contained in the AGGREGATE.
- The root is the only member of the AGGREGATE that outside objects are allowed to hold references to, although objects within the boundary may hold references to each other.
- ENTITIES other than the root have local identity, but it only needs to be unique within the aggregate, since no outside object can ever see it out of the context of the root ENTITY.

  For Example, the car is ROOT which is identified by the VIN number which is unique and each tyre internally has some representation to find which tyre rotation is captured. That is internal to the car and the outside world refers car with VIN. But Tyre has unique identity within the aggregate.

> Cluster the ENTITIES and VALUE OBJECTS into “AGGREGATES” and define boundaries around each. Choose one ENTITY to be the “root” of each AGGREGATE, and control all access to the objects inside the boundary through the root.
> Only allow references to the root to be held by external objects.
> Transient references to internal members can be passed out for use within a single operation only. Because the root controls access it cannot be blind-sided by changes to the internals. This makes it practical to enforce all invariants for objects in the AGGREGATE and for the AGGREGATE as a whole in any state-change.

#### FACTORIES
This concept has come into the field due to separation of reponsibilities between the object creation and responsibility of the objects. A program element whose responsibility is the creation of other objects is called a FACTORY.


 Just as the interface of an object should encapsulate its implementation, allowing a client to use its behavior without knowing how it works, a FACTORY encapsulates the knowledge needed to create a complex object or AGGREGATE. It provides an interface that reflects the goals of the client and an abstract view of the created object.

 > Shift the responsibility for creating instances of complex objects and AGGREGATES to a separate object, which may itself have no responsibility in the domain model, but is still part of the domain design. Provide an interface that encapsulates all complex assembly and that does not require the client to reference the concrete classes of the objects being instantiated. Create entire AGGREGATES as a piece, enforcing their invariants.

There are some creational patterns like FACTORY METHOD, ABSTRACT FACTORY and BUILDER. these patterns helps the model driven design on track

> FACTORY METHOD encapsulates expansion of an Aggregate


#### REPOSITORIES
The repositories provide controlled access to aggregates and act as a bridge between the domain model and the data persistence.  the purpose of repositories are they abstract the mechanisms of object storage and retrieval. They also provide an in-memory collection like interface to access domain objects. they ensure that domain llogic remains independent of persistent concerns.

##### What is the difference between repositories and Data Access Objects (DAOs)?
- DAO expose database queries and are focused on the persistence mechanism where as repositories, are part of the domain layer and provide access to aggregates while maintaining business rules
- Repositories return fully formed domain objects, not raw data structures.

##### Good repository means--
- Handles aggregates -> Repositories typically manage aggregate roots to ensure consistency
- Provides a collection like interface -> It should behave like an in-memory collection offering methods like add(), remove() and findById()
- Encapsulates Queries -> Clients should not beed to know how objects are persisted and they should just retrieve objects via repository methods
- Maintains a Seperation of Concerns -> Business Logic should not be mixed with persistence logic

##### Implementation Guidelines --
- Define repositories for aggregate roots only
- Keep repository interfaces domain driven  (eg., findOrderByCustomer() instead of a generic SQL like query)
- Allow the domain layer to remain independent of the persistence layer ( Use dependency injection if needed)
- Use repositories as an entry point for retrieving domain objects instead of direct database access

##### Repositories in Large context
* They work closely with factories to handle object creation
* They preserve domain logic by ensuring only valid domain objects are retrieved and stored
* They help decouple the domain layer from the infrastructure layer
  
#### Designing Objects for Relational Databases
This topic focuses on the domain models to relational databases, handling object - relational impedence mismatches, and ensuring that the persistence mechanism does not pollute the domain layer

##### The Challenge of Mapping objects to Relational Databases
Relational Databases store data in tables with normalized structures and Object oriented models represent entities as objects with encapsulated behaviors. this creates challenge when mapping between the two because - 
* Objects have hierarchial relationships while relational databases rely on flat tables with foreign keys
* Objects use inheritance and polymorphism but relational databases do not directly support these features
* Objects are usually referenced through associations while relational databases prefer joins
 To bridge this gap domain driven design must carefully map objects to database tables without compromising the domain model

##### Mapping Aggregates to Tables
Since aggregates group entities and enforce consistency rules, the persistence mechanism should not reflect aggregate boundaries. So recommended approach is
* Each aggregate root should map to a separate table
* Entities inside an aggregate should be stored in the same table or as related tables
* Foriegn keys should only reference aggregate roots not inernal entities

For example, Order is an aggregate root and maps to orders table and the Orderline is part of Order and maps to the order_lines table with a foreign key references to orders.

> Objects within the same aggregate should be saved and retrieved together to maintain consistency

##### Handling Associations in a Relational Database
Object-oriented models rely on associations(references) while relational databases use foreign keys.


**One-to-One Association** - If an Employee entity has an associated Address. It can be stored using a foriegn key in the Employee Table. 


> Best Practice - If the associated object is a Value Object (e.g., Address) consider embedding it in the parent table rather than using a foriegn key.

**One-to-Many Association** - If an Order has multiple OrderLines. the order_lines table will store a foreign key pointing to orders

> Best Practice - Use cascading operations in the ORM to ensure that deleting an order deletes its order lines


**Many-to-Many Association** - For relationships like " A student can enroll in multiple Courses and a course has multiple students" a join table is needed

> Best Practice - When using many-to-many relationships, introduce a domain concept instead of a pure join table (eg., Enrollment)

##### Strategies for Handling Inheritance




## Chapter 3 - Refactoring Toward Deeper Insight
### Making implicit Concepts Explicit
### Supple Design
### Applying Analysis Patterns
### Relating Design Patterns to the Model

## Chapter - 4 - Strategic Design
### Maintaining Model Integrity
### Distillation
### Large-Scale Structure






