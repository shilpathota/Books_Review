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

