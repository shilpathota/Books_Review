# Review of Book Domain Driven Design by Eric Evans

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
An object that represents a descriptive aspect of the domain that has no conceptual identity is called a VALUE OBJECT






