# Beyond the Linguistic Cortex
**A Modular, Brain-Aligned Architecture for Artificial General Intelligence**

William Murray  
2 April 2026

---

## Table of Contents  
1. Introduction  
2. The Limits of Monolithic Language Models  
    2.1 The Stochastic Parrot Problem  
    2.2 The Grounding Problem  
    2.3 The Memory and Planning Deficit  
    2.4 The Scaling Hypothesis and Its Limits  
3. Biological Precedents for Modular Cognition  
    3.1 The Brain as a System of Systems  
    3.2 The Linguistic Cortex in Biological Context 
    3.3 World Models and Predictive Processing  
    3.4 Memory, Reward, and Planning in the Biological Brain  
4. The Proposed Architecture: A Modular AGI Framework  
    4.1 Overview  
    4.2 The Language Module  
    4.3 The World Model Module  
    4.4 The Memory Module  
    4.5 The Planning and Reward Modules  
    4.6 Perception and Action Modules  
5. The Digital Corpus Callosum: Integration and Coherence  
    5.1 The Biological Precedent  
    5.2 The Digital Corpus Callosum as Integration Fabric  
    5.3 Architectural Implementation  
6. The Minimal Viable AGI: Implementation Pathway  
    6.1 Defining the Minimal Configuration  
    6.2 Justification for the Minimal Set  
    6.3 Scaling Beyond the MVAGI  
7. Meta-Cognition, Homeostasis, and Developmental Engines  
    7.1 Meta-Cognition: Thinking About Thinking  
    7.2 Homeostatic Regulation: Stability Through Self-Regulation  
    7.3 Developmental Engines: Growing Intelligence Over Time  
8. Implications, Limitations, and Future Directions  
    8.1 Implications for AGI Research  
    8.2 Comparison with Existing Proposals  
    8.3 Limitations and Open Questions  
    8.4 Future Directions  
9. Conclusion  

---

## Abstract  
Large Language Models (LLMs) represent a remarkable advance in artificial intelligence, yet they remain fundamentally constrained as candidates for Artificial General Intelligence (AGI). This essay argues that LLMs function as analogues of the brain's linguistic cortex – a powerful interface for symbolic compression and communication – rather than as complete cognitive systems. Drawing on evidence from neuroscience, cognitive science, and contemporary machine learning research, the essay proposes a modular AGI architecture that mirrors the structural, functional, and developmental organisation of biological intelligence. The architecture comprises specialised modules for world-modelling, memory, planning, reward, perception, action, meta-cognition, homeostasis, and developmental scaffolding. Central to the proposal is the Digital Corpus Callosum: a high-bandwidth, bidirectional integration fabric that aligns symbolic and sub-symbolic representations, synchronises module states, resolves conflicts, and enforces global coherence. The essay introduces the concept of a Minimal Viable AGI – an implementation pathway that prioritises the smallest subset of modules sufficient to demonstrate integrated general intelligence – and situates this proposal within the broader landscape of AGI research.

---

## 1. Introduction  
The rapid scaling of Large Language Models over the past half-decade has generated extraordinary excitement – and extraordinary confusion – regarding the proximity of Artificial General Intelligence. [1] Systems such as GPT-4, PaLM, and their successors demonstrate fluency in natural language, competence in code generation, and surprisingly strong performance on standardised reasoning benchmarks. [2] These achievements have led some commentators to speculate that scaling transformer architectures further may be sufficient to produce general intelligence. [3]

Such speculation, however, conflates linguistic competence with cognition itself. Biological intelligence offers a compelling counterexample to the monolithic approach. The human brain does not consist of a single, undifferentiated network; it comprises dozens of specialised subsystems – for perception, memory, planning, reward evaluation, motor control, and language – integrated through dense white-matter tracts and neuromodulatory circuits. [4]

Language, far from constituting the entirety of thought, occupies a circumscribed set of cortical regions (Broca's area, Wernicke's area, the angular gyrus) and functions primarily as an interface for symbolic compression and interpersonal communication. [5] Patients with severe aphasia – the loss of language capacity – nonetheless retain the ability to reason, navigate, plan, and solve novel problems. [6] Language is an interface layered atop cognition, not its substrate.

This essay contends that constructing AGI requires moving beyond monolithic language models toward a modular, brain-aligned architecture in which specialised components collaborate through a unifying integration fabric. Given the current state of incomplete understanding of intelligence itself, the most principled approach draws on the only known example of general intelligence – the biological brain – as an architectural template. This does not entail slavish biomimicry; rather, it involves identifying the functional principles that make biological cognition general, adaptive, and robust, and instantiating those principles in computational form.

The essay proceeds as follows:
*   Section 2 examines the structural and functional limitations of monolithic LLMs as AGI candidates;
*   Section 3 surveys the neuroscientific evidence for modular cognition in biological systems;
*   Section 4 introduces the proposed modular AGI framework and maps its components to biological subsystems;
*   Section 5 elaborates the Digital Corpus Callosum as the critical integration mechanism;
*   Section 6 presents the Minimal Viable AGI concept as a practical implementation pathway;
*   Section 7 addresses the roles of meta-cognition, homeostasis, and developmental engines within the architecture;
*   Section 8 discusses implications, limitations, and directions for future research; and
*   Section 9 concludes with a synthesis of the central argument.

## 2. The Limits of Monolithic Language Models  

### 2.1 The Stochastic Parrot Problem  
  
Bender, Gebru, McMillan-Major, and Shmitchell characterise large language models as “stochastic parrots” – systems that produce statistically plausible sequences of tokens without genuine understanding of the concepts those tokens represent. [1] This critique, while sometimes overstated, identifies a genuine architectural constraint. LLMs acquire distributional patterns from text corpora; they do not construct causal models of the world, form persistent memories of past interactions, or pursue goals through deliberate planning. The appearance of understanding emerges from interpolation over vast training distributions rather than from structured reasoning processes. [7]

Marcus and Davis extend this critique by documenting systematic failures of LLMs on tasks requiring compositional generalisation, physical reasoning, and logical consistency. [8] When presented with novel combinations of familiar concepts – a hallmark of human cognitive flexibility – LLMs frequently produce confident but erroneous outputs. These failures are not merely performance gaps addressable through additional training data; they reflect the absence of architectural mechanisms for grounding, abstraction, and systematic recombination. The monolithic transformer, for all its power, lacks the structural prerequisites for robust general reasoning.

### 2.2 The Grounding Problem  

A particularly consequential limitation concerns perceptual grounding. Human cognition develops through embodied interaction with the physical world; concepts such as “weight,” “distance,” and “fragility” derive their meaning from sensorimotor experience rather than from co-occurrence statistics in text. [9] LLMs, trained exclusively on linguistic data, acquire only the statistical shadow of these concepts – what Harnad terms “parasitic” semantics, inherited from the grounded experiences of the humans who produced the training text. [10]

This absence of grounding manifests in characteristic failure modes: physically implausible spatial reasoning, inability to simulate dynamic processes, and susceptibility to adversarial prompts that exploit the gap between linguistic plausibility and physical reality.

### 2.3 The Memory and Planning Deficit  

Monolithic LLMs operate within a fixed context window – a transient buffer that is erased between interactions and constrained in capacity. [11] They possess no mechanism for persistent episodic memory (the capacity to recall specific past events), no structured semantic knowledge base that updates incrementally, and no procedural memory for acquired skills. Planning presents an equally fundamental challenge. While LLMs can generate text that describes plans, they lack the capacity to evaluate those plans against a world model, simulate their consequences, revise them in response to feedback, or maintain goal states across extended time horizons. [12] These are not peripheral features of intelligence; they are constitutive of it.

### 2.4 The Scaling Hypothesis and Its Limits  

Proponents of the scaling hypothesis argue that continued increases in model size, training data, and compute will eventually produce emergent general intelligence. [3] While scaling has indeed yielded impressive capability gains, the evidence suggests diminishing returns on benchmarks that probe genuine reasoning rather than pattern matching. [13]

Chollet's Abstraction and Reasoning Corpus (ARC) – designed to test fluid intelligence through novel, low-data tasks – remains largely unsolved by scaled LLMs, highlighting a fundamental gap between memorisation-driven performance and true adaptive reasoning. [14] The ARC benchmark is particularly instructive because it requires the kind of on-the-fly abstraction and rule induction that characterises human fluid intelligence; success demands identifying novel visual patterns from minimal examples and applying them to unseen configurations. LLMs, which excel at tasks that resemble their training distribution, struggle precisely because ARC tasks are explicitly designed to fall outside any plausible training distribution.

Furthermore, recent analyses of so-called “emergent abilities” in large language models suggest that many apparent capability jumps may be artefacts of evaluation methodology rather than genuine phase transitions in cognitive capacity. [13] When evaluation metrics are adjusted to use continuous rather than discrete scoring, the sharp transitions dissolve into smooth, predictable scaling curves. This finding undermines the strongest version of the scaling hypothesis – the claim that qualitatively new cognitive capabilities spontaneously emerge at sufficient scale. Scaling a linguistic cortex, however large, does not produce a complete mind; it produces a larger linguistic cortex. The path to AGI requires architectural innovation, not merely parametric expansion.

## 3. Biological Precedents for Modular Cognition  

### 3.1 The Brain as a System of Systems  

Neuroscience has long recognised that the brain comprises functionally specialised subsystems rather than a homogeneous processing substrate. [4] Fodor's influential modularity thesis proposed that input systems – perception and language – operate as informationally encapsulated, domain-specific modules with dedicated neural hardware. [15] While subsequent research has demonstrated greater interaction between modules than Fodor's strict encapsulation allows, the fundamental principle of functional specialisation remains robust. Visual processing, auditory processing, spatial navigation, language production, motor planning, and reward evaluation each depend on distinct neural circuits with characteristic computational properties. Dehaene and colleagues elaborate this principle through Global Workspace Theory, which posits that specialised processors operate in parallel and compete for access to a shared “global workspace” – a distributed neural network (centred on prefrontal and parietal cortices) that broadcasts selected information to all modules simultaneously. [17] This architecture enables flexible, context-dependent integration of specialised computations without requiring each module to communicate directly with every other. The global workspace serves as an integration and arbitration layer, not as the locus of cognition itself. This distinction – between the integration fabric and the specialised processors it connects – provides a crucial insight for AGI architecture design.

### 3.2 The Linguistic Cortex in Biological Context

The language system of the human brain occupies a relatively circumscribed set of cortical regions. Broca's area (in the left inferior frontal gyrus) supports speech production and syntactic processing; Wernicke's area (in the left posterior superior temporal gyrus) supports speech comprehension and semantic retrieval; and the angular gyrus mediates cross-modal integration relevant to reading and abstract semantic processing. [5] Critically, lesion studies demonstrate that damage to these regions impairs language but leaves other cognitive capacities – spatial reasoning, problem-solving, social cognition, motor planning – substantially intact. [6] Conversely, patients with intact language faculties but damage to prefrontal, parietal, or hippocampal regions may lose the capacity for planning, spatial navigation, or episodic memory while retaining fluent speech. These dissociations establish that language constitutes one specialised subsystem among many, rather than the computational engine of general intelligence. Extending this principle to artificial systems suggests that an LLM – however sophisticated – corresponds to the linguistic cortex of a potential AGI system. Treating it as a complete mind represents a category error analogous to treating Broca's area as the seat of all cognition.

### 3.3 World Models and Predictive Processing

The posterior cortex – spanning temporal, parietal, and occipital regions – constructs a continuously updated multimodal model of the environment. [18] This “world model” integrates visual, auditory, tactile, and proprioceptive information into a coherent representation of the current state of the world, and generates predictions about how that state will evolve over time. The hippocampus contributes spatial and episodic structure, enabling both navigation and the re-experiencing of past events; the cerebellum refines predictive models through error-driven learning. [19] This predictive processing framework – articulated theoretically by Clark and computationally by Friston – posits that the brain fundamentally operates as a prediction machine, minimising the discrepancy between expected and observed sensory input. [20]

In the machine learning literature, analogous principles appear in the work of Ha and Schmidhuber on world models [21] and LeCun's Joint Embedding Predictive Architecture (JEPA), which proposes learning representations by predicting latent states rather than pixel-level observations. [22] Hafner and colleagues demonstrate the power of world-model-based reasoning through the Dreamer architecture, which learns to act effectively in simulated environments by planning within a learned latent dynamics model. [23] These efforts confirm that world-modelling – absent from standard LLM architectures – constitutes a tractable and essential component of general intelligence.

### 3.4 Memory, Reward, and Planning in the Biological Brain

Biological memory comprises multiple functionally distinct systems: working memory (maintained by sustained prefrontal activity), episodic memory (dependent on hippocampal encoding and cortical consolidation), semantic memory (distributed across temporal and prefrontal cortices), and procedural memory (supported by basal ganglia and cerebellar circuits). [24] Each system serves different computational purposes and operates on different timescales; their coordination enables the flexible deployment of past experience in novel contexts.

The dopaminergic reward system – centred on the ventral tegmental area and the striatum – provides the teaching signals that shape behaviour through reinforcement learning. [25] Schultz's discovery that dopaminergic neurons encode reward prediction errors established a direct link between biological reward processing and the temporal-difference learning algorithms central to modern reinforcement learning. [26] Planning, meanwhile, depends on prefrontal cortex and its interactions with the basal ganglia, supporting goal maintenance, hierarchical action decomposition, and model-based evaluation of candidate strategies. [27] Sutton and Barto's foundational framework for reinforcement learning formalises these principles computationally, and model-based reinforcement learning – which plans by simulating outcomes within an internal model – offers the most neurally plausible account of deliberate planning. [28] Taken together, memory, reward, and planning represent architectural pillars that any AGI system must instantiate; their absence from monolithic LLMs constitutes a fundamental, not merely incremental, limitation.

## 4. The Proposed Architecture: A Modular AGI Framework

### 4.1 Overview

The proposed architecture comprises a set of specialised modules – each corresponding to a functionally distinct subsystem of the biological brain – integrated through a central communication fabric (the Digital Corpus Callosum) and supervised by meta-cognitive and homeostatic regulatory layers. The core modules include: a Language Module (LLM), a World Model Module, a Memory Module (with working, episodic, semantic, and procedural sub-components), a Planning Module, a Reward and Value Module, Perception and Action Modules, a Meta-Cognitive Module, a Homeostatic Regulation Module, and a Developmental Engine. Each module operates with relative autonomy in its domain of specialisation while exchanging information with other modules through the integration fabric.

This design philosophy draws on the principle that biological intelligence achieves generality not through a single omnipotent processor but through the coordinated activity of many specialised systems. [4] The architecture preserves the strengths of existing AI components – the linguistic fluency of LLMs, the predictive power of world models, the optimisation capacity of reinforcement learning – while addressing the integration deficit that prevents any single component from achieving general intelligence.

### 4.2 The Language Module

The Language Module corresponds to the biological linguistic cortex and is instantiated by a large language model. Its function is symbolic compression and decompression: encoding complex thoughts into natural language and decoding natural language into internal representations. Critically, the Language Module serves as an interface – mediating communication with human users, enabling verbal reasoning and self-narration, and providing access to the vast cultural knowledge embedded in training corpora. [5] It does not serve as the world model, the planner, or the agent. Recognising the Language Module's circumscribed role prevents the architectural overloading that characterises current LLM-centric approaches.

### 4.3 The World Model Module

The World Model Module constructs and maintains a multimodal generative model of the environment – a learned, internal simulation that represents the current state of the world and predicts how it will change in response to actions or external events. [21] Drawing on the JEPA framework, this module learns representations in latent space rather than reconstructing raw observations, enabling efficient prediction and generalisation. [22] The World Model operates in a complementary stream to the Language Module: where the Language Module processes symbolic and cultural information, the World Model processes spatial, temporal, and causal structure. Their integration – achieved through the Digital Corpus Callosum – produces a system that can both reason about the world and communicate its reasoning in natural language.

### 4.4 The Memory Module

The Memory Module implements four biologically inspired sub-systems. Working memory provides a limited-capacity buffer for maintaining and manipulating information relevant to the current task – analogous to the active maintenance function of prefrontal cortex. [24] Episodic memory stores structured records of past experiences, enabling the system to recall specific events, learn from mistakes, and generalise across episodes. Semantic memory maintains a continuously updated knowledge base of facts, concepts, and relationships – distinct from the frozen knowledge embedded in LLM parameters. Procedural memory stores acquired skills and routines as executable policies, supporting the accumulation of expertise over time. This multi-system design addresses the memory deficit of monolithic LLMs by providing persistent, structured, and functionally differentiated storage.

### 4.5 The Planning and Reward Modules

The Planning Module implements model-based reinforcement learning: it uses the World Model to simulate the consequences of candidate actions, evaluates those consequences against objectives provided by the Reward Module, and selects action sequences that maximise expected value. [28] This approach enables deliberate, multi-step planning – the capacity to reason about future states and choose actions strategically – that is entirely absent from autoregressive token prediction. The Reward and Value Module provides both intrinsic objectives (curiosity, coherence, energy conservation) and extrinsic objectives (task-specific goals), and implements credit assignment mechanisms that attribute outcomes to the actions responsible for them. [25] Together, these modules transform the architecture from a reactive system into a goal-directed agent.

### 4.6 Perception and Action Modules

Perception Modules provide hierarchical encoders for processing sensory input – visual, auditory, tactile, and proprioceptive – transforming raw observations into structured representations suitable for the World Model and other modules. [18] Action Modules provide the complementary interface, translating planned actions into executable motor commands or API calls. These modules ground the architecture in the physical or digital environment, addressing the perceptual grounding problem that constrains disembodied language models. The inclusion of perception and action completes the sensorimotor loop that biological cognition requires for learning and adaptation.

## 5. The Digital Corpus Callosum: Integration and Coherence

### 5.1 The Biological Precedent

The corpus callosum – the largest white-matter tract in the human brain – provides approximately 200 million axonal fibres connecting the left and right cerebral hemispheres. [29] It enables high-bandwidth, bidirectional communication between functionally lateralised regions; supports the synchronisation of activity across hemispheres; and implements both excitatory and inhibitory gating to regulate inter-hemispheric information flow. [30] Gazzaniga's pioneering research on split-brain patients – individuals whose corpus callosum has been surgically severed – demonstrates the consequences of severing this integration fabric: each hemisphere operates with partial information, generating independent and sometimes contradictory perceptions, intentions, and verbal reports. [31]

A particularly instructive phenomenon in split-brain research is confabulation. When the left hemisphere (which controls language) observes behaviour initiated by the right hemisphere (which lacks linguistic access), the left hemisphere fabricates plausible but incorrect explanations for that behaviour. [31] This confabulation – the generation of linguistically coherent but factually unfounded narratives – bears a striking structural resemblance to the hallucination phenomenon in large language models. LLMs, like the disconnected left hemisphere, produce fluent text that lacks grounding in an accurate world model. The analogy suggests that LLM hallucination may be understood not as a bug to be patched but as a predictable consequence of a fundamental architectural deficit: the absence of a callosal integration fabric connecting the linguistic system to a veridical world model.

### 5.2 The Digital Corpus Callosum as Integration Fabric

The Digital Corpus Callosum is the proposed integration mechanism for the modular AGI architecture. It serves five primary functions. First, it performs cross-modal alignment – translating between the symbolic representations of the Language Module and the sub-symbolic latent representations of the World Model, ensuring that linguistic descriptions remain consistent with the system's internal model of reality. [22] Second, it implements synchronous state sharing – broadcasting relevant state information from each module to all others that require it, analogous to the global workspace's broadcasting function in biological cognition. [17] Third, it provides conflict resolution – detecting inconsistencies between module outputs (for instance, when the Language Module generates a claim that contradicts the World Model's predictions) and arbitrating in favour of the better-grounded representation. Fourth, it implements gating and control – selectively amplifying or attenuating information flow between modules based on current task demands and attentional priorities. Fifth, it embeds safety and verification mechanisms – subjecting proposed actions and assertions to consistency checks before they are executed or communicated.

### 5.3 Architectural Implementation

The Digital Corpus Callosum operates as a learned routing and alignment layer – not a fixed bus but an adaptive network that develops increasingly sophisticated integration strategies through training. Drawing on cross-attention mechanisms and contrastive alignment techniques from multimodal learning, [32] the callosum learns to map between heterogeneous representation spaces, resolve conflicts through evidence weighting, and route information efficiently based on task context. Its training proceeds jointly with the modules it connects, enabling co-adaptation between specialised processors and the integration fabric.

The implementation draws on several existing technical paradigms. Cross-attention mechanisms – widely used in multimodal transformers – provide the foundation for inter-module communication, allowing each module to attend to relevant information from other modules while filtering irrelevant signals. Contrastive learning objectives – as demonstrated in CLIP and related architectures [32] – provide the training signal for aligning representations across heterogeneous spaces; the callosum learns to project symbolic linguistic representations and sub-symbolic world-model representations into a shared embedding space where consistency can be evaluated. Gating mechanisms – inspired by the mixture-of-experts paradigm – enable dynamic routing, ensuring that information flows preferentially to the modules that require it for the current task while reducing unnecessary communication overhead.

This design addresses a critical gap in existing AGI proposals. Many modular architectures enumerate components – world models, planners, memory systems – but fail to specify how those components communicate and cohere. [33] The Digital Corpus Callosum fills this gap by providing an explicit, trainable mechanism for achieving the unified operation that distinguishes a mind from a collection of disconnected tools. Without such a mechanism, a modular system risks degenerating into a loose federation of independent programs – capable in their individual domains but unable to coordinate on tasks requiring integrated cognition.

## 6. The Minimal Viable AGI: Implementation Pathway

### 6.1 Defining the Minimal Configuration

A practical implementation pathway must identify the smallest subset of modules sufficient to demonstrate integrated general intelligence – what may be termed a Minimal Viable AGI (MVAGI). This concept draws on engineering principles of incremental development: rather than attempting to construct the entire architecture simultaneously, the MVAGI provides a testable prototype that can be evaluated, refined, and progressively expanded. [34]

The proposed MVAGI comprises six components:
1. A Language Module (an existing LLM, fine-tuned for integration)
2. A World Model Module (a latent dynamics model trained on multimodal data)
3. A Planning Module (implementing model-based reinforcement learning)
4. An Episodic Memory system (a persistent, queryable store of past experiences)
5. A Digital Corpus Callosum (the integration fabric)
6. A Meta-Cognitive Module (a supervisory layer for error detection and confidence estimation)

This configuration omits – for the initial prototype – full multimodal perception, procedural memory, intrinsic motivation, social cognition, and homeostatic regulation, deferring these to subsequent development phases.

### 6.2 Justification for the Minimal Set

Each component in the MVAGI addresses a distinct and necessary cognitive function. The Language Module provides the symbolic interface for communication and verbal reasoning. The World Model provides grounded, predictive understanding of the environment. The Planning Module transforms understanding into goal-directed action. Episodic Memory provides the capacity to learn from experience over time. The Digital Corpus Callosum integrates these components into a coherent system. The Meta-Cognitive Module provides self-monitoring – the capacity to detect errors, estimate confidence, and know when to defer or seek additional information. [35] Removing any single component would leave a critical cognitive gap: without the World Model, reasoning remains ungrounded; without the Planner, understanding cannot translate into action; without Memory, the system cannot accumulate experience; without the Callosum, modules cannot collaborate; without Meta-Cognition, the system cannot monitor its own reliability.

### 6.3 Scaling Beyond the MVAGI

Subsequent development phases progressively add components to the MVAGI core. The first expansion incorporates multimodal perception (vision, audio) and procedural memory, enabling the system to interact with richer environments and accumulate skills. Procedural memory is particularly important for this expansion phase, as it enables the system to compile frequently used action sequences into efficient routines – reducing the computational burden on the Planning Module and freeing deliberative resources for novel challenges.

The second expansion adds intrinsic motivation (curiosity-driven exploration), social cognition (theory of mind, imitation learning), and homeostatic regulation. Intrinsic motivation provides the system with autonomous drive to explore its environment and seek out learning opportunities even in the absence of externally specified goals – a capacity that distinguishes truly autonomous agents from task-specific tools. Social cognition enables the system to model other agents' beliefs, intentions, and knowledge states, supporting cooperative behaviour, communication, and cultural learning.

The final phase introduces developmental dynamics – the capacity for the system to undergo structured developmental stages analogous to biological maturation. [36] This incremental pathway manages engineering complexity while maintaining a functional, testable system at each stage. Each expansion phase can be independently evaluated against benchmarks that probe the specific capabilities it introduces, ensuring that progress toward full AGI capability is measurable and empirically grounded.

## 7. Meta-Cognition, Homeostasis, and Developmental Engines

### 7.1 Meta-Cognition: Thinking About Thinking

Meta-cognition – the capacity to monitor, evaluate, and regulate one's own cognitive processes – represents a critical and frequently overlooked component of general intelligence. [35] Flavell's foundational work distinguishes between meta-cognitive knowledge (understanding of one's own cognitive strengths and limitations) and meta-cognitive regulation (the ability to plan, monitor, and adjust cognitive strategies during task performance). [37] Nelson and Narens formalise this through a two-level model in which a “meta-level” monitors and controls an “object-level” of cognitive processing. [38]

In the proposed architecture, the Meta-Cognitive Module implements analogous functions. It monitors the outputs of other modules for internal consistency, detects situations in which confidence is low or conflicting signals arise, triggers deliberative re-processing when automatic responses appear unreliable, and maintains long-horizon coherence by tracking whether ongoing activity remains aligned with overarching goals. Biologically, these functions map onto the medial prefrontal cortex and the anterior cingulate cortex – regions that support error detection, conflict monitoring, and self-referential processing. [39] The inclusion of meta-cognition addresses a salient limitation of current AI systems: their inability to recognise the boundaries of their own competence. An LLM that generates a confident but incorrect response demonstrates precisely the failure mode that meta-cognitive monitoring would prevent.

### 7.2 Homeostatic Regulation: Stability Through Self-Regulation

Biological intelligence operates within homeostatic constraints – regulatory mechanisms that maintain internal variables within viable ranges despite external perturbation. [40] The hypothalamus and brainstem neuromodulatory systems regulate arousal, attention, learning rates, and energy allocation, ensuring that the organism neither overreacts to trivial stimuli nor underreacts to significant threats. These systems implement a form of dynamic stability that prevents runaway excitation, catastrophic forgetting, and resource depletion.

The Homeostatic Regulation Module translates these principles into the AGI architecture. It monitors system-level variables – computational resource allocation, learning rate schedules, module activation levels, and error rates – and adjusts them dynamically to maintain stable operation. [40] When the World Model's prediction errors spike (indicating environmental novelty), the homeostatic system increases learning rates and attentional resources allocated to perception; when prediction errors are low (indicating a familiar environment), it reduces resource expenditure and allows consolidation processes to proceed. This regulatory function is analogous to the role of neuromodulators (dopamine, serotonin, norepinephrine, acetylcholine) in biological cognition and addresses the stability-plasticity dilemma – the challenge of maintaining learned knowledge while remaining adaptable to new information. [41]

### 7.3 Developmental Engines: Growing Intelligence Over Time

Human intelligence does not emerge fully formed; it develops through a structured sequence of stages characterised by critical periods, progressive skill acquisition, synaptic pruning, and curriculum-driven learning. [42] Infants first develop basic sensorimotor competences; children progressively acquire language, social cognition, and abstract reasoning; adolescents refine executive function and long-horizon planning. Each stage builds upon the competences acquired in the preceding stage, and the timing of developmental transitions matters – premature exposure to complex tasks impedes rather than accelerates development. [43]

The Developmental Engine implements analogous principles within the AGI architecture. Training proceeds through a curriculum that presents tasks of progressively increasing complexity, with each phase building on representations and competences stabilised in the preceding phase. Early phases focus on world-model learning and basic sensorimotor competences; intermediate phases introduce planning, memory consolidation, and linguistic integration; advanced phases engage meta-cognition, social reasoning, and abstract thought. Consolidation cycles – inspired by the memory-consolidating function of sleep in biological systems [45] – periodically interrupt active learning to stabilise newly acquired knowledge, compress redundant representations, and integrate recent experiences with long-term memory structures. Bengio and colleagues provide computational precedent for curriculum learning, demonstrating that presenting training examples in order of increasing difficulty accelerates convergence and improves generalisation. [44] The Developmental Engine extends this principle from a training heuristic to a core architectural component, arguing that structured developmental trajectories are not merely useful but necessary for the emergence of robust, adaptive intelligence.

## 8. Implications, Limitations, and Future Directions

### 8.1 Implications for AGI Research

The proposed architecture carries several implications for the broader AGI research programme. First, it reframes the role of LLMs: rather than abandoning large language models or treating them as proto-AGI systems, the architecture positions them as essential but circumscribed components – the linguistic cortex of a more comprehensive cognitive system. [5] This reframing preserves the substantial investment in LLM research while redirecting effort toward the missing architectural components. Second, the proposal highlights integration as the central unsolved problem of AGI. Many individual components – world models, planners, memory systems, reinforcement learning agents – exist in mature or near-mature forms; the challenge lies in composing them into a coherent, unified system. [33] The Digital Corpus Callosum addresses this challenge directly.

### 8.2 Comparison with Existing Proposals

The architecture shares important features with LeCun's proposed autonomous machine intelligence framework, which similarly emphasises world models, hierarchical planning, and self-supervised learning. [22] It diverges, however, in several respects: it assigns a more central role to language (as the primary interface for cultural learning, verbal reasoning, and human communication); it includes explicit meta-cognitive and homeostatic layers; and it specifies an integration mechanism (the Digital Corpus Callosum) rather than leaving inter-module communication implicit. LeCun's framework, while architecturally sophisticated, underspecifies the mechanism by which its proposed components – the world model, the actor, the critic, and the configurator – achieve coordinated operation. The present proposal addresses this gap directly through the callosal integration fabric. Goertzel's OpenCog framework pursues a related vision of modular cognitive architecture but employs a different integration strategy based on hypergraph knowledge representation. [33] While OpenCog's emphasis on heterogeneous knowledge representation is well-motivated, its reliance on a single representational substrate (the atomspace) may limit its capacity to accommodate the fundamentally different computational idioms of symbolic and sub-symbolic processing. The present architecture embraces representational heterogeneity and relies on the Digital Corpus Callosum to mediate between distinct representation spaces. Legg and Hutter's formal definition of universal intelligence provides a theoretical benchmark against which such architectures may be evaluated, though the gap between formal definitions and practical implementation remains substantial. [46]

### 8.3 Limitations and Open Questions

Several significant challenges remain unresolved. The latent alignment problem – ensuring that representations in different modules occupy compatible spaces and can be meaningfully compared – lacks a general solution. [32] The identity persistence problem – maintaining a coherent sense of self and continuous autobiographical memory across updates, restarts, and architectural modifications – has no established precedent in artificial systems. The question of whether and how consciousness might emerge from modular integration remains philosophically and empirically open. [47] Ethical considerations – including the safety implications of goal-directed agents with planning and memory capabilities – require careful attention and the embedding of safety constraints within the callosal fabric itself. [48]

### 8.4 Future Directions

Productive avenues for future research include: empirical investigation of cross-modal alignment techniques suitable for the callosal integration layer; the development of benchmarks that evaluate integrated cognition rather than individual capabilities; exploration of neuromorphic hardware architectures that natively support modular, asynchronous processing; and the construction of MVAGI prototypes in simulated environments that permit systematic evaluation of integrated performance. The developmental dimension of the architecture – the structured progression from simple to complex competences – also warrants empirical study, particularly regarding the identification of optimal curricula and the timing of developmental transitions.

## 9. Conclusion

The central argument of this essay is that Artificial General Intelligence requires structural, functional, and developmental analogues to biological intelligence – and that monolithic language models, for all their linguistic sophistication, provide only one of the many necessary components. LLMs function as the linguistic cortex of a potential AGI system: powerful, culturally informed, and indispensable for symbolic communication, yet fundamentally insufficient as standalone cognitive architectures. General intelligence demands grounded world models that predict and simulate physical reality; memory systems that accumulate, organise, and retrieve experience across multiple timescales; planning mechanisms that translate understanding into goal-directed action; reward systems that provide the evaluative signals necessary for learning and adaptation; and meta-cognitive processes that monitor the system's own reliability and coherence.

The Digital Corpus Callosum – the proposed integration fabric – addresses what is perhaps the most critical and least discussed gap in current AGI research: the mechanism by which specialised modules achieve unified, coherent operation. Just as the biological corpus callosum prevents the confabulatory fragmentation observed in split-brain patients, the Digital Corpus Callosum prevents the hallucination, incoherence, and groundlessness that characterise disconnected linguistic systems. Homeostatic regulation ensures dynamic stability; developmental engines ensure that intelligence matures through structured stages rather than emerging fully formed from a single training run.

The Minimal Viable AGI concept offers a pragmatic pathway forward – a testable prototype comprising the smallest set of modules sufficient for integrated general intelligence, expandable through incremental addition of further components. This approach manages engineering complexity while maintaining a functional, evaluable system at each stage of development. The essay does not claim that the proposed architecture will produce consciousness, sentience, or human-equivalent intelligence. It claims, more modestly, that the architecture addresses identified structural deficits in current approaches and provides a principled, biologically grounded blueprint for constructing systems with integrated, adaptive, and general cognitive capabilities. The path to AGI leads not through a larger linguistic cortex but beyond it – toward a complete, modular, and deeply integrated artificial mind.

---

## Endnotes

1. E. Bender, T. Gebru, A. McMillan-Major, and S. Shmitchell, “On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?” *Proceedings of the ACM Conference on Fairness, Accountability, and Transparency (FAccT)*, 2021, pp. 610–623.
2. OpenAI, “GPT-4 Technical Report,” *arXiv preprint arXiv:2303.08774*, 2023.
3. J. Kaplan, S. McCandlish, T. Henighan, et al., “Scaling Laws for Neural Language Models,” *arXiv preprint arXiv:2001.08361*, 2020.
4. M. S. Gazzaniga, R. B. Ivry, and G. R. Mangun, *Cognitive Neuroscience: The Biology of the Mind*, 5th ed. New York: W. W. Norton, 2019.
5. E. Fedorenko, A. Nieto-Castañón, and N. Kanwisher, “Lexical and Syntactic Representations in the Brain: An fMRI Investigation with Multi-Voxel Pattern Analyses,” *Neuropsychologia*, vol. 50, no. 4, 2012, pp. 499–513.
6. A. R. Luria, *Higher Cortical Functions in Man*, 2nd ed. New York: Basic Books, 1980.
7. G. Marcus, “The Next Decade in AI: Four Steps Towards Robust Artificial Intelligence,” *arXiv preprint arXiv:2002.06177*, 2020.
8. G. Marcus and E. Davis, *Rebooting AI: Building Artificial Intelligence We Can Trust*. New York: Pantheon Books, 2019.
9. L. W. Barsalou, “Grounded Cognition,” *Annual Review of Psychology*, vol. 59, 2008, pp. 617–645.
10. S. Harnad, “The Symbol Grounding Problem,” *Physica D: Nonlinear Phenomena*, vol. 42, no. 1–3, 1990, pp. 335–346.
11. A. Vaswani, N. Shazeer, N. Parmar, et al., “Attention Is All You Need,” *Advances in Neural Information Processing Systems (NeurIPS)*, vol. 30, 2017, pp. 5998–6008.
12. K. Valmeekam, M. Marquez, S. Sreedharan, and S. Kambhampati, “On the Planning Abilities of Large Language Models – A Critical Investigation,” *Advances in Neural Information Processing Systems (NeurIPS)*, vol. 36, 2023.
13. R. Schaeffer, B. Miranda, and S. Koyejo, “Are Emergent Abilities of Large Language Models a Mirage?” *Advances in Neural Information Processing Systems (NeurIPS)*, vol. 36, 2023.
14. F. Chollet, “On the Measure of Intelligence,” *arXiv preprint arXiv:1911.01547*, 2019.
15. J. A. Fodor, *The Modularity of Mind: An Essay on Faculty Psychology*. Cambridge, MA: MIT Press, 1983.
16. M. S. C. Thomas and J. L. McClelland, “Connectionist Models of Cognition,” in *The Cambridge Handbook of Computational Psychology*, R. Sun, Ed. Cambridge: Cambridge University Press, 2008, pp. 23–58.
17. S. Dehaene and J.-P. Changeux, “Experimental and Theoretical Approaches to Conscious Processing,” *Neuron*, vol. 70, no. 2, 2011, pp. 200–227.
18. A. Clark, *Surfing Uncertainty: Prediction, Action, and the Embodied Mind*. Oxford: Oxford University Press, 2016.
19. J. O’Keefe and L. Nadel, *The Hippocampus as a Cognitive Map*. Oxford: Clarendon Press, 1978.
20. K. Friston, “The Free-Energy Principle: A Unified Brain Theory?” *Nature Reviews Neuroscience*, vol. 11, no. 2, 2010, pp. 127–138.
21. D. Ha and J. Schmidhuber, “Recurrent World Models Facilitate Policy Evolution,” *Advances in Neural Information Processing Systems (NeurIPS)*, vol. 31, 2018.
22. Y. LeCun, “A Path Towards Autonomous Machine Intelligence,” *OpenReview preprint*, version 0.9.2, 2022.
23. D. Hafner, T. Lillicrap, J. Ba, and M. Norouzi, “Dream to Control: Learning Behaviours by Latent Imagination,” *Proceedings of the International Conference on Learning Representations (ICLR)*, 2020.
24. L. R. Squire and S. M. Zola, “Structure and Function of Declarative and Nondeclarative Memory Systems,” *Proceedings of the National Academy of Sciences*, vol. 93, no. 24, 1996, pp. 13515–13522.
25. W. Schultz, P. Dayan, and P. R. Montague, “A Neural Substrate of Prediction and Reward,” *Science*, vol. 275, no. 5306, 1997, pp. 1593–1599.
26. W. Schultz, “Dopamine Reward Prediction-Error Signalling: A Two-Component Response,” *Nature Reviews Neuroscience*, vol. 17, no. 3, 2016, pp. 183–195.
27. E. K. Miller and J. D. Cohen, “An Integrative Theory of Prefrontal Cortex Function,” *Annual Review of Neuroscience*, vol. 24, 2001, pp. 167–202.
28. R. S. Sutton and A. G. Barto, *Reinforcement Learning: An Introduction*, 2nd ed. Cambridge, MA: MIT Press, 2018.
29. F. Aboitiz, A. B. Scheibel, R. S. Fisher, and E. Zaidel, “Fiber Composition of the Human Corpus Callosum,” *Brain Research*, vol. 598, no. 1–2, 1992, pp. 143–153.
30. M. S. Gazzaniga, “Cerebral Specialization and Interhemispheric Communication: Does the Corpus Callosum Enable the Human Condition?” *Brain*, vol. 123, no. 7, 2000, pp. 1293–1326.
31. M. S. Gazzaniga, *The Bisected Brain*. New York: Appleton-Century-Crofts, 1970.
32. A. Radford, J. W. Kim, C. Hallacy, et al., “Learning Transferable Visual Models from Natural Language Supervision,” *Proceedings of the International Conference on Machine Learning (ICML)*, vol. 139, 2021, pp. 8748–8763.
33. B. Goertzel, “OpenCog: A Software Framework for Integrative Artificial General Intelligence,” *Proceedings of the AGI Conference*, 2009, pp. 63–68.
34. E. Ries, *The Lean Startup: How Today’s Entrepreneurs Use Continuous Innovation to Create Radically Successful Businesses*. New York: Crown Business, 2011.
35. J. H. Flavell, “Metacognition and Cognitive Monitoring: A New Area of Cognitive–Developmental Inquiry,” *American Psychologist*, vol. 34, no. 10, 1979, pp. 906–911.
36. L. Smith and M. Gasser, “The Development of Embodied Cognition: Six Lessons from Babies,” *Artificial Life*, vol. 11, no. 1–2, 2005, pp. 13–29.
37. J. H. Flavell, “Metacognitive Aspects of Problem Solving,” in *The Nature of Intelligence*, L. B. Resnick, Ed. Hillsdale, NJ: Erlbaum, 1976, pp. 231–235.
38. T. O. Nelson and L. Narens, “Metamemory: A Theoretical Framework and New Findings,” in *The Psychology of Learning and Motivation*, vol. 26, G. H. Bower, Ed. New York: Academic Press, 1990, pp. 125–173.
39. D. M. Amodio and C. D. Frith, “Meeting of Minds: The Medial Frontal Cortex and Social Cognition,” *Nature Reviews Neuroscience*, vol. 7, no. 4, 2006, pp. 268–277.
40. P. Sterling, “Allostasis: A Model of Predictive Regulation,” *Physiology and Behaviour*, vol. 106, no. 1, 2012, pp. 5–15.
41. S. Grossberg, “Competitive Learning: From Interactive Activation to Adaptive Resonance,” *Cognitive Science*, vol. 11, no. 1, 1987, pp. 23–63.
42. J. Piaget, *The Construction of Reality in the Child*. New York: Basic Books, 1954.
43. E. L. Newport, “Maturational Constraints on Language Learning,” *Cognitive Science*, vol. 14, no. 1, 1990, pp. 11–28.
44. Y. Bengio, J. Louradour, R. Collobert, and J. Weston, “Curriculum Learning,” *Proceedings of the International Conference on Machine Learning (ICML)*, 2009, pp. 41–48.

---

## Bibliography

### Articles
*   **Aboitiz, F., Scheibel, A. B., Fisher, R. S., and Zaidel, E.** “Fiber Composition of the Human Corpus Callosum.” *Brain Research*, vol. 598, no. 1–2, 1992, pp. 143–153.
*   **Amodio, D. M., and Frith, C. D.** “Meeting of Minds: The Medial Frontal Cortex and Social Cognition.” *Nature Reviews Neuroscience*, vol. 7, no. 4, 2006, pp. 268–277.
*   **Barsalou, L. W.** “Grounded Cognition.” *Annual Review of Psychology*, vol. 59, 2008, pp. 617–645.
*   **Bender, E., Gebru, T., McMillan-Major, A., and Shmitchell, S.** “On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?” *Proceedings of the ACM Conference on Fairness, Accountability, and Transparency (FAccT)*, 2021, pp. 610–623.
*   **Bengio, Y., Louradour, J., Collobert, R., and Weston, J.** “Curriculum Learning.” *Proceedings of the International Conference on Machine Learning (ICML)*, 2009, pp. 41–48.
*   **Dehaene, S., and Changeux, J.-P.** “Experimental and Theoretical Approaches to Conscious Processing.” *Neuron*, vol. 70, no. 2, 2011, pp. 200–227.
*   **Fedorenko, E., Nieto-Castañón, A., and Kanwisher, N.** “Lexical and Syntactic Representations in the Brain: An fMRI Investigation with Multi-Voxel Pattern Analyses.” *Neuropsychologia*, vol. 50, no. 4, 2012, pp. 499–513.
*   **Friston, K.** “The Free-Energy Principle: A Unified Brain Theory?” *Nature Reviews Neuroscience*, vol. 11, no. 2, 2010, pp. 127–138.
*   **Gazzaniga, M. S.** “Cerebral Specialization and Interhemispheric Communication: Does the Corpus Callosum Enable the Human Condition?” *Brain*, vol. 123, no. 7, 2000, pp. 1293–1326.
*   **Ha, D., and Schmidhuber, J.** “Recurrent World Models Facilitate Policy Evolution.” *Advances in Neural Information Processing Systems (NeurIPS)*, vol. 31, 2018.
*   **Hafner, D., Lillicrap, T., Ba, J., and Norouzi, M.** “Dream to Control: Learning Behaviours by Latent Imagination.” *Proceedings of the International Conference on Learning Representations (ICLR)*, 2020.

### Books
*   **Chalmers, D. J.** *The Conscious Mind: In Search of a Fundamental Theory*. Oxford: Oxford University Press, 1996.
*   **Fodor, J. A.** *The Modularity of Mind: An Essay on Faculty Psychology*. Cambridge, MA: MIT Press, 1983.
*   **Gazzaniga, M. S.** *The Bisected Brain*. New York: Appleton-Century-Crofts, 1970.
*   **Gazzaniga, M. S., Ivry, R. B., and Mangun, G. R.** *Cognitive Neuroscience: The Biology of the Mind*, 5th ed. New York: W. W. Norton, 2019.
*   **Luria, A. R.** *Higher Cortical Functions in Man*, 2nd ed. New York: Basic Books, 1980.
*   **Marcus, G., and Davis, E.** *Rebooting AI: Building Artificial Intelligence We Can Trust*. New York: Pantheon Books, 2019.
*   **O’Keefe, J., and Nadel, L.** *The Hippocampus as a Cognitive Map*. Oxford: Clarendon Press, 1978.
*   **Piaget, J.** *The Construction of Reality in the Child*. New York: Basic Books, 1954.
*   **Ries, E.** *The Lean Startup: How Today’s Entrepreneurs Use Continuous Innovation to Create Radically Successful Businesses*. New York: Crown Business, 2011.
*   **Russell, S.** *Human Compatible: Artificial Intelligence and the Problem of Control*. New York: Viking, 2019.
*   **Sutton, R. S., and Barto, A. G.** *Reinforcement Learning: An Introduction*, 2nd ed. Cambridge, MA: MIT Press, 2018.
*   **Walker, M. P.** *Why We Sleep: The New Science of Sleep and Dreams*. London: Allen Lane, 2017.

### Online Resources and Preprints
*   **Chollet, F.** “On the Measure of Intelligence.” *arXiv preprint arXiv:1911.01547*, 2019.
*   **Kaplan, J., McCandlish, S., Henighan, T., et al.** “Scaling Laws for Neural Language Models.” *arXiv preprint arXiv:2001.08361*, 2020.
*   **LeCun, Y.** “A Path Towards Autonomous Machine Intelligence.” *OpenReview preprint*, version 0.9.2, 2022.
*   **Marcus, G.** “The Next Decade in AI: Four Steps Towards Robust Artificial Intelligence.” *arXiv preprint arXiv:2002.06177*, 2020.
*   **OpenAI.** “GPT-4 Technical Report.” *arXiv preprint arXiv:2303.08774*, 2023.

### Book Chapters
*   **Flavell, J. H.** “Metacognitive Aspects of Problem Solving.” In *The Nature of Intelligence*, edited by L. B. Resnick. Hillsdale, NJ: Erlbaum, 1976, pp. 231–235.
*   **Thomas, M. S. C., and McClelland, J. L.** “Connectionist Models of Cognition.” In *The Cambridge Handbook of Computational Psychology*, edited by R. Sun. Cambridge: Cambridge University Press, 2008, pp. 23–58.
