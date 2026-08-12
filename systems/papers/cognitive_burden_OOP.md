# The Cognitive Burden of Object-Oriented Programming: A Critical Analysis of Encapsulation, Abstraction, and the Failure of Modular Coherence

**William Murray**
**29 August 2025**

---

## 1. Introduction

The dominance of Object-Oriented Programming (OOP) in contemporary software development represents one of the most significant cognitive burdens imposed upon the programming profession in the past three decades. Despite widespread adoption and institutional endorsement, OOP fundamentally violates principles of cognitive minimalism and epistemic restraint that should guide effective programming practice. This paper argues that OOP constitutes poor practice not merely due to performance considerations or aesthetic preferences, but because it systematically increases cognitive load whilst failing to deliver genuine benefits in terms of modularity, maintainability, or comprehensibility.

The theoretical framework for this critique draws upon Cognitive Load Theory (CLT), which distinguishes between intrinsic load (inherent problem complexity), extraneous load (imposed by poor design), and germane load (productive cognitive effort devoted to schema formation) [1]. When evaluated against these criteria, OOP consistently increases extraneous cognitive load through verbose syntax, convoluted abstractions, and semantically opaque constructs, whilst simultaneously hindering germane load by fragmenting coherent functionality across multiple classes and files.

The significance of this analysis extends beyond academic discourse to encompass practical concerns about developer productivity, code maintainability, and the accessibility of programming to diverse practitioners. As the software industry grapples with increasing complexity and the need for more inclusive development practices, the cognitive burden imposed by OOP becomes a critical barrier to effective software development.

This paper acknowledges that the original creators of object-oriented concepts, particularly those focused on polymorphism as a mechanism for code reuse and abstraction, had legitimate intentions. The concept of polymorphism – allowing different types to be treated uniformly through common interfaces – represents a valuable abstraction mechanism. However, the implementation and evolution of OOP has devolved far from these original intentions, creating a paradigm that obscures rather than clarifies program logic.

## 2. Theoretical Framework: Cognitive Load Theory and Programming Paradigms

The application of Cognitive Load Theory to programming paradigm evaluation provides a rigorous framework for understanding why certain approaches to software development succeed or fail in supporting human cognition. CLT's tripartite model offers precise tools for evaluating the cognitive efficiency of programming languages and methodologies [2].

**Intrinsic cognitive load** in programming stems from the fundamental complexity of computational problems – understanding algorithms, managing state, and reasoning about system behaviour. This load cannot be eliminated without sacrificing computational expressiveness, but it can be presented in forms that align with human cognitive patterns. Effective programming paradigms should minimise the cognitive translation required between human intent and computational expression.

**Extraneous cognitive load** manifests through design decisions that impose unnecessary cognitive overhead without contributing to problem-solving capability. In programming contexts, this includes verbose boilerplate code, inconsistent naming conventions, scattered functionality, and semantically opaque constructs that force developers to maintain irrelevant details in working memory [3]. The principle of epistemic restraint, derived from Occam's Razor, suggests that programming paradigms should avoid multiplying cognitive, semantic, or modular entities beyond what is necessary for emergent coherence.

**Germane cognitive load** represents productive cognitive effort devoted to building mental models, recognising patterns, and developing expertise. Programming paradigms that support germane load exhibit consistent patterns, clear semantic mappings, and progressive disclosure of complexity. They enable developers to construct accurate mental models of system behaviour through direct examination of code structure and logic flow.

The synthesis of these principles suggests that optimal programming paradigms should prioritise **cognitive minimalism** – not through superficial syntactic simplicity, but through deeper attention to conceptual coherence and semantic clarity. This framework provides the theoretical foundation for evaluating OOP's cognitive efficiency and identifying its fundamental shortcomings.

## 3. The Fundamental Flaw: Fine-Grained Encapsulation and Cognitive Fragmentation

The central critique of Object-Oriented Programming centres on its prescription for fine-grained encapsulation – the division of program state into numerous small, encapsulated units that interact through message-passing interfaces. This approach, whilst theoretically appealing, systematically violates principles of cognitive minimalism and creates what can only be described as **cognitive fragmentation**.

The original conception of object-oriented message-passing envisioned objects as autonomous entities communicating through discrete messages containing copies of relevant state. In practice, however, OOP implementations rely heavily on object references, creating implicit shared state that undermines the theoretical benefits of encapsulation [4]. When objects receive messages from multiple sources, they become effectively coupled, and the promised encapsulation "flies out the window." The resulting system exhibits all the complexity of shared state whilst adding layers of indirection that obscure rather than clarify program logic.

For genuine encapsulation to function effectively, programs would require strict hierarchical organisation with a single "God object" responsible for coordinating all interactions down the chain. Cross-cutting concerns would necessitate convoluted "bucket brigade" communication patterns up and down the hierarchy – an approach so impractical that no competent programmer would implement it. The alternative – allowing direct object interaction – nullifies the theoretical benefits of encapsulation whilst retaining its cognitive overhead.

This fundamental contradiction creates a cognitive burden that manifests in two primary forms: over-engineered abstraction towers and inconsistently architected object tangles. The former represents attempts to maintain encapsulation principles through elaborate hierarchies of abstract classes and interfaces, creating what amounts to a **"giant Tower of abstractions"** that obscures simple functionality behind layers of indirection. The latter emerges when developers, frustrated by the constraints of strict encapsulation, allow objects to interact directly, creating **"an inconsistently architected pile of objects that are all probably Tangled together like Christmas lights."**

The cognitive impact of this fragmentation extends beyond mere complexity to encompass what might be termed **"surface area explosion."** OOP design systematically fragments coherent functionality, taking "relatively self-contained code and splitting it up into many separate methods across many separate classes," often distributed across multiple files [4]. This fragmentation increases the cognitive surface area that developers must navigate to understand program behaviour, creating a sensation analogous to taking "a neatly sorted deck of cards and throwing them into the air."

The debugging implications of this fragmentation are particularly severe. Modern debugging tools, designed to support object-oriented code, often fail to provide crucial information about program state due to the complex indirection inherent in OOP designs. Developers frequently find themselves unable to determine "where the fuck I am" in the call stack, as demonstrated in practical analyses of even well-written object-oriented code [4]. The promised benefits of encapsulation – clear interfaces and predictable behaviour – are undermined by the cognitive overhead required to navigate the resulting complexity.

## 4. The Kingdom of Nouns: Forced Abstraction and Semantic Incoherence

Object-Oriented Programming's ideological commitment to associating all behaviours with data types creates what can aptly be described as a **"Kingdom of Nouns"** – a programming environment populated by artificial entities that exist primarily as containers for behaviour rather than representations of meaningful data [4]. This forced association between functions and data types violates principles of semantic clarity and imposes unnecessary cognitive burden through the creation of "unobvious, unnatural data types."

The manifestation of this problem appears most clearly in the proliferation of "service classes," "manager classes," and other "doer classes" that serve no purpose beyond satisfying OOP's ideological requirements. These entities represent pure cognitive overhead – they contribute nothing to problem-solving capability whilst requiring developers to maintain awareness of their existence, interfaces, and interactions. The resulting code becomes populated with nebulous abstractions like "UserServiceManager" or "DataProcessorFactory" that obscure rather than clarify program intent.

This forced abstraction creates what might be termed **"analysis paralysis"** – developers must engage in elaborate "matchmaking games" between functions and data types, leading to "obnoxious philosophical dilemmas" about where particular functionality should reside [4]. The promised "real-world modelling" becomes a "Fool's game" as developers struggle to map computational operations onto artificial object hierarchies that bear no meaningful relationship to problem domains.

The cognitive burden of this approach extends beyond initial development to encompass long-term maintenance and comprehension. Class names often mislead, as functionality is rarely self-contained within a single class. Tracking down user-visible functionality requires navigating scattered logic across multiple classes, each contributing fragments of the overall behaviour. This fragmentation violates the principle of locality of reference – both in terms of memory access patterns and cognitive processing – making programs significantly more difficult to understand and modify.

The abstraction problem is compounded by the semantic confusion between programmers' technical definition of "abstract" (simplified interface over complex implementation) and its general usage (difficult to understand, bearing no resemblance to common experience). Most program components are abstract in the latter sense, making them cognitively challenging to conceptualise them as neatly self-contained modules with real-world analogues. The pollution of code with generic entities like "managers," "factories," and "services" adds excess layers of abstraction that increase rather than decrease cognitive burden.

This semantic incoherence represents a fundamental violation of cognitive minimalism principles. Rather than reducing the conceptual entities that developers must maintain in working memory, OOP systematically multiplies them through artificial abstractions that serve ideological rather than practical purposes. The resulting cognitive overhead manifests as increased development time, higher error rates, and reduced accessibility for developers who process information systematically.

## 5. Cognitive Load Analysis: OOP versus Procedural Approaches

A systematic comparison of Object-Oriented and procedural programming approaches through the lens of Cognitive Load Theory reveals significant differences in cognitive efficiency and developer experience. This analysis demonstrates that procedural approaches consistently reduce extraneous cognitive load whilst supporting more effective germane load through clearer semantic mappings and more direct expression of program logic.

Procedural programming's fundamental advantage lies in its cognitive simplicity: **"there is just the call graph"** [4]. This unified mental model eliminates the multiple, overlapping conceptual frameworks that OOP requires developers to maintain simultaneously – inheritance hierarchies, composition relationships, data flow patterns, and call graphs. The cognitive burden of maintaining these multiple, often conflicting mental models represents pure extraneous load that contributes nothing to problem-solving capability.

The principle of **explicit parameterisation** in procedural programming directly addresses the shared state problems that OOP attempts to solve through encapsulation. By passing data explicitly as function parameters, procedural code ensures that data access flows clearly through the call graph, making dependencies visible and traceable. This approach eliminates the hidden coupling that emerges in object-oriented systems when objects share references to mutable state.

The cognitive benefits of procedural approaches become particularly evident in debugging and program comprehension scenarios. Procedural code maintains clear execution flow that can be followed linearly through function calls, whilst object-oriented code often requires developers to navigate complex webs of method invocations across multiple classes. The debugging experience described in practical analyses of OOP code – where developers repeatedly lose track of execution context and struggle to understand program state – rarely occurs in well-structured procedural code [4].

The handling of long functions in procedural programming illustrates another cognitive advantage. Contrary to object-oriented orthodoxy that mandates small methods, procedural programming recognises that long functions have legitimate uses for **"long laundry lists"** of sequential operations [4]. Such functions provide clear logical flow, reduce cognitive clutter by limiting the number of entities developers must browse, and avoid the difficulty of naming numerous small functions that serve no purpose beyond satisfying arbitrary size constraints.

The cognitive efficiency of procedural approaches extends to error handling and program modification. **Pure functions** – a natural fit within procedural paradigms – are "truly self-contained," making them easier to understand, test, and modify. The absence of side effects means that function behaviour can be understood through examination of parameters and return values, without requiring knowledge of complex object lifecycles or global state dependencies.

**Coarse-grained encapsulation** at the module or namespace level provides the organisational benefits that OOP promises without the cognitive overhead of fine-grained object interactions. This approach works because modules are larger and less numerous than typical OOP classes, making cross-cutting concerns "reasonably manageable" even when ideal hierarchical organisation is violated [4].

## 6. The Historical Accident: Java's Influence and Industry Adoption

The dominance of Object-Oriented Programming in contemporary software development represents what can best be described as a historical accident rather than a rational evaluation of programming paradigm effectiveness. The widespread adoption of OOP correlates strongly with Java's introduction in the mid-1990s, which offered numerous practical advantages that were largely independent of its object-oriented features [4].

Java's appeal stemmed from several factors that addressed genuine pain points in 1990s software development: cross-platform compatibility through virtual machine bytecode, garbage collection that eliminated manual memory management, proper namespaces without header files, and accessible naming conventions that contrasted favourably with cryptic Win32 APIs. The language provided a "welcome reprieve" from the complexity of C++ development environments whilst offering the familiar curly-brace syntax that gave it the feel of "real programming."

Crucially, Java could have achieved virtually all of these benefits as a procedural language whilst retaining portability, garbage collection, and exception handling. Languages like Python demonstrate that it is possible to support both object-oriented and procedural approaches without forcing all functionality into classes. The decision to mandate object-oriented organisation was ideological rather than technical, yet it became conflated with Java's genuine technical advantages.

The GUI programming context of the 1990s provided a particularly compelling use case for object-oriented approaches, as the mapping of GUI components to classes seemed "very natural" and offered tangible examples of "real world modeling." This specific domain success was then generalised inappropriately to all programming contexts, despite the fact that most software development involves computational rather than interface concerns.

The industry's subsequent investment in object-oriented methodologies – design patterns, SOLID principles, dependency injection, test-driven development – represents what might be termed **"compensatory complexity."** These practices emerged as "Band-Aids" to address the fundamental problems created by OOP's flawed foundation rather than as natural extensions of a successful paradigm [4]. The proliferation of these compensatory practices serves as evidence that **"the original vision of object-oriented programming has never panned out."**

The educational impact of this historical accident cannot be overstated. An entire generation of programmers has been trained to think in object-oriented terms, creating institutional momentum that persists despite mounting evidence of the paradigm's cognitive inefficiency. The result is an industry-wide case of what might be termed **"paradigm lock-in,"** where the costs of transition appear to outweigh the benefits of change, even when the current approach is demonstrably suboptimal.

## 7. Practical Implications: Code Comprehension and Maintenance

The practical implications of Object-Oriented Programming's cognitive burden manifest most clearly in code comprehension and maintenance scenarios, where developers must navigate complex object hierarchies to understand and modify program behaviour. Real-world analyses of object-oriented code, even when written by highly skilled practitioners, consistently demonstrate the paradigm's failure to support effective program comprehension [4].

The **loss of execution flow control** represents perhaps the most significant practical problem with object-oriented code. Developers frequently find themselves unable to follow program execution due to complex templated classes, multiple levels of inheritance, and abstract interfaces that obscure the actual code being executed. This problem is compounded by debugging tools that fail to provide crucial information about program state, such as the actual types of templated classes or the specific variables being initialised in complex constructors.

The **fragmentation of functionality across multiple classes** creates what might be termed **"cognitive scatter"** – developers must maintain awareness of numerous small pieces of functionality distributed across different files and classes to understand any single program behaviour. This fragmentation violates principles of locality of reference and makes it significantly more difficult to build coherent mental models of program operation.

Object creation patterns in OOP often exhibit what can be described as **"premature instantiation"** – objects are created and then later populated with data, without clear justification for their existence at the point of creation. This pattern forces developers to maintain awareness of object lifecycles and state transitions that contribute nothing to problem-solving capability whilst increasing cognitive burden.

The principle of **"hiding implementation details,"** often cited as a benefit of OOP, frequently becomes a detriment in practice by creating so many levels of indirection that it becomes impossible to understand program behaviour. The promised benefits of abstraction are undermined when the abstraction layers themselves become more complex than the underlying implementation they purport to simplify.

Maintenance scenarios reveal additional problems with object-oriented approaches. The **tight coupling** between classes, despite theoretical encapsulation, means that modifications to one class often require changes to multiple related classes. The resulting **"ripple effects"** make it difficult to predict the full impact of changes, leading to increased testing burden and higher error rates.

The **naming problem** in object-oriented code represents another significant maintenance challenge. Class and method names often fail to accurately reflect their functionality, as behaviour is distributed across multiple classes rather than being self-contained. This naming confusion increases the cognitive burden of code navigation and makes it more difficult for new developers to understand existing codebases.

## 8. Cognitive Accessibility and Neurodivergent Considerations

The cognitive burden imposed by Object-Oriented Programming has particularly significant implications for neurodivergent developers and those who process information systematically. The paradigm's reliance on implicit relationships, scattered functionality, and context-dependent behaviour creates barriers that disproportionately affect individuals who benefit from clear, predictable patterns and explicit information flow [3].

The principle of **minimal surprisal** becomes crucial when considering neurodivergent-inclusive programming paradigms. OOP's context-dependent semantics and hidden coupling violate this principle by creating situations where identical code can behave differently depending on complex interaction patterns that are not immediately visible. This unpredictability can impose significant cognitive burden on individuals who process information systematically and rely on consistent, predictable behaviour patterns.

The **fragmentation of functionality** across multiple classes and files creates particular challenges for developers who benefit from being able to examine complete logical sequences in a single location. The need to navigate between multiple files and classes to understand a single program behaviour increases cognitive load and can be particularly challenging for individuals with attention-related differences who may struggle to maintain context across multiple locations.

The **"Kingdom of Nouns"** problem has specific implications for neurodivergent developers who may process abstract concepts differently. The proliferation of artificial entities like "service classes" and "manager classes" creates additional cognitive entities that must be maintained in working memory without contributing to problem comprehension. This multiplication of abstract entities violates principles of cognitive minimalism and can be particularly burdensome for individuals who prefer concrete, direct representations of program logic.

Procedural programming approaches offer significant advantages for neurodivergent-inclusive development through their emphasis on **explicit parameter passing, clear execution flow, and minimal abstraction overhead.** The ability to understand program behaviour through direct examination of function calls and parameter flow reduces the cognitive burden associated with maintaining complex mental models of object interactions and state dependencies.

The debugging advantages of procedural approaches become particularly important for neurodivergent developers who may rely more heavily on systematic analysis of program behaviour. The clear execution flow and explicit state management in procedural code make it easier to understand program behaviour through debugging tools and systematic analysis, reducing the cognitive burden associated with program comprehension and modification.

## 9. Alternative Approaches: Procedural Programming and Cognitive Efficiency

The alternative to Object-Oriented Programming lies not in exotic functional programming paradigms, but in a return to procedural approaches that prioritise cognitive efficiency and semantic clarity. Procedural programming, properly understood, offers a more cognitively efficient approach to software development that aligns with human cognitive architecture whilst avoiding the artificial constraints imposed by object-oriented ideology [4].

The fundamental advantage of procedural programming lies in its cognitive simplicity: there is no explicit association between data types and functions, eliminating the forced abstractions that characterise object-oriented approaches. This separation allows developers to think about data structures and transformations independently of artificial "responsibilities" or "self-imposed barriers," reducing cognitive load and enabling more direct expression of program logic.

The guidelines for effective procedural programming directly address the problems that OOP attempts to solve through encapsulation whilst avoiding the cognitive overhead of fine-grained object interactions. **Explicit parameterisation** ensures that data dependencies flow clearly through the call graph, making program behaviour predictable and traceable. This approach eliminates the hidden coupling that emerges in object-oriented systems whilst maintaining clear separation of concerns.

The opportunistic use of **pure functions** within procedural paradigms provides the benefits of functional programming without requiring wholesale adoption of functional approaches. Pure functions are "truly self-contained," making them easier to understand, test, and modify. The absence of side effects means that function behaviour can be understood through examination of parameters and return values, without requiring knowledge of complex object lifecycles or global state dependencies.

**Coarse-grained encapsulation** at the module or namespace level provides organisational benefits without the cognitive overhead of fine-grained object interactions. This approach recognises that encapsulation works effectively at larger scales where the number of interacting entities remains manageable and cross-cutting concerns can be handled through well-defined interfaces.

The acceptance of **long functions** in procedural programming represents a significant cognitive advantage over object-oriented approaches that mandate artificial function size limits. Long functions that implement sequential operations provide clear logical flow and reduce cognitive clutter by eliminating the need to navigate between numerous small methods that serve no purpose beyond satisfying arbitrary size constraints.

The proposed **"use" block concept** illustrates how procedural languages could be enhanced to provide the benefits of local encapsulation without the overhead of separate function definitions. Such constructs would allow inline, self-contained code blocks that explicitly manage variable scope whilst maintaining clear execution flow – combining the benefits of functional approaches with the cognitive simplicity of procedural organisation.

## 10. Conclusion

This analysis has demonstrated that Object-Oriented Programming represents a fundamentally flawed paradigm that systematically violates principles of cognitive minimalism and imposes unnecessary cognitive burden on software developers. The core problems – fine-grained encapsulation that creates cognitive fragmentation, forced abstraction that populates code with meaningless entities, and the multiplication of conceptual frameworks that developers must maintain simultaneously – constitute violations of epistemic restraint that make programs more difficult to understand, modify, and maintain.

The practical evidence supporting this critique is overwhelming. Real-world analyses of object-oriented code, even when written by highly skilled practitioners, consistently demonstrate the paradigm's failure to support effective program comprehension. The loss of execution flow control, the fragmentation of functionality across multiple classes, and the debugging difficulties inherent in object-oriented approaches represent systematic failures that cannot be attributed to poor implementation but rather reflect fundamental problems with the paradigm itself.

The historical analysis reveals that OOP's dominance represents an accident of timing rather than a rational evaluation of programming paradigm effectiveness. Java's success stemmed from practical advantages – cross-platform compatibility, garbage collection, and improved development environments – that were largely independent of its object-oriented features. The subsequent investment in compensatory practices like design patterns and SOLID principles represents evidence that the original vision of object-oriented programming has failed to deliver its promised benefits.

The cognitive accessibility implications of this analysis extend beyond individual developer productivity to encompass broader questions of inclusion and diversity in software development. The cognitive burden imposed by OOP creates barriers that disproportionately affect neurodivergent developers and those who process information systematically, contributing to the exclusion of diverse perspectives from the software development profession.

The alternative lies in procedural programming approaches that prioritise cognitive efficiency through explicit parameter passing, clear execution flow, and minimal abstraction overhead. These approaches align with human cognitive architecture whilst avoiding the artificial constraints imposed by object-oriented ideology. The guidelines for effective procedural programming – explicit parameterisation, opportunistic use of pure functions, coarse-grained encapsulation, and acceptance of long functions where appropriate – provide practical strategies for reducing cognitive burden whilst maintaining expressive power.

Whilst acknowledging that the original creators of object-oriented concepts had legitimate intentions, particularly regarding polymorphism as a mechanism for code reuse, the implementation and evolution of OOP has devolved far from these original goals. The paradigm has become a collection of compensatory practices that obscure rather than clarify program logic, creating cognitive burden without delivering corresponding benefits.

The path forward requires abandoning the "ideals" of OOP in favour of more pragmatic approaches that prioritise human cognitive efficiency over ideological consistency. This represents not a retreat from sophisticated programming techniques, but rather an advancement toward programming paradigms that serve human flourishing rather than imposing additional cognitive burdens. The liberation from object-oriented constraints can enable more direct, comprehensible, and maintainable approaches to software development that better serve both developers and the users of the systems they create.

The implications of this analysis extend beyond individual programming practice to encompass educational approaches, industry standards, and the future direction of programming language development. The recognition that OOP represents poor practice should inform decisions about curriculum design, language selection, and architectural approaches, prioritising cognitive efficiency and semantic clarity over adherence to object-oriented orthodoxy.

As the software industry continues to grapple with increasing complexity and the need for more inclusive development practices, the principles identified in this analysis – cognitive minimalism, epistemic restraint, and alignment with human cognitive architecture – provide essential guidance for creating programming environments that enhance rather than hinder human cognitive capabilities. The future of effective software development lies not in the multiplication of abstract entities and artificial constraints, but in the disciplined application of cognitive science principles to create programming paradigms that serve human flourishing.

---

### References

[1] Sweller, J. (1988). Cognitive load during problem solving: Effects on learning. *Cognitive Science*, 12(2), 257-285.

[2] Murray, W. (2025). *Cognitive Minimalism in Programming: Applying Occam's Razor and Cognitive Load Theory to Software Development Best Practices*. Unpublished manuscript.

[3] Murray, W. (2025). *Cognitive Load and Referencing Styles: Optimising Scholarly Communication*. Unpublished manuscript.

[4] Anonymous. (2025). *Critique of Object-Oriented Programming*. Unpublished manuscript.

[5] Paas, F., Renkl, A., & Sweller, J. (2003). Cognitive load theory and instructional design: Recent developments. *Educational Psychologist*, 38(1), 1-4.

[6] Van Merrienboer, J. J., & Sweller, J. (2005). Cognitive load theory and complex learning: Recent developments and future directions. *Educational Psychology Review*, 17(2), 147-177.
