# Reclaiming the Scar: Reinforcement Learning – Optimised Miyawaki Corridors for Defragmenting Logged Landscapes

**William Murray**
*10 August 2026*
*Version 0.4*

---

> **Author’s Note**  
> This whitepaper is written from a simple but easily overlooked observation: the strategic geometry of landscape fragmentation maps directly onto the strategic geometry of Go. Roads cut territory; planted corridors cut territory. Both create and erase liberties, both partition and reconnect continuous space, and both determine long‑arc survivability through the shape of connection. The optimisation framework presented here treats ecological restoration as a board‑state problem on a damaged manifold, where Miyawaki micro‑forests function as connection operators and reinforcement learning evaluates policy trajectories over reconnection geometry. Readers familiar with Go will recognise the mapping immediately; readers who do not will still find the ecological argument intact.

---

## Abstract

Logging roads constitute one of the most pervasive drivers of forest fragmentation across tropical and temperate biomes. Their ecological impact extends far beyond the physical removal of vegetation, producing edge effects, movement barriers, invasion pathways, and hydrological disruption. This whitepaper proposes a unified optimisation framework that integrates Miyawaki micro‑forest corridor planting with reinforcement learning techniques modelled on the strategic architecture of AlphaGo. The objective is to maximise **Equivalent Connected Area (ECA)**, a graph‑theoretic measure of landscape permeability, while minimising edge proliferation and economic cost.

---

## 1. The Problem: Logging Roads as Ecological Fragmenters

### 1.1 Mechanisms of Fragmentation

Logging roads impose a series of biophysical disruptions that extend well beyond the cleared corridor.
*   **Edge effects:** Alter temperature, humidity, and wind penetration up to 50–200 metres into intact forest, thereby degrading interior microhabitats.
*   **Movement barriers:** Prevent amphibians, small mammals, and understory birds from crossing exposed ground, fragmenting populations and restricting gene flow.
*   **Invasion corridors:** Allow weeds, feral predators, and human disturbance to penetrate previously inaccessible areas.
*   **Hydrological disruption:** Roadbed compaction disrupts hydrological processes, increasing erosion and drying adjacent soils.

These processes collectively produce a mosaic of isolated habitat patches separated by biologically hostile linear scars. The ecological consequences are not limited to reduced forest cover; rather, they reflect a fundamental loss of connectivity.

### 1.2 Why Connectivity Determines Ecological Function

Connectivity is the principal determinant of ecological resilience in fragmented landscapes.
*   **Genetic erosion:** Isolated patches experience reduced allelic diversity, increasing extinction risk.
*   **Local extinction debt:** Populations fall below viable thresholds, leading to delayed collapse.
*   **Reduced resilience:** Disconnected patches cannot be recolonised following disturbance events.

Restoration strategies that focus solely on increasing tree cover fail to address these structural issues. Effective restoration must therefore prioritise the re‑establishment of **continuous habitat pathways** that support movement, gene flow, and microclimatic stability.

---

## 2. The Solution: Miyawaki Corridors as Topological Repair

### 2.1 The Miyawaki Method

The Miyawaki method accelerates ecological succession through high‑density planting of 30–50 native species across multiple vertical strata.
*   **Rapid growth:** Planting densities of 3–5 saplings per square metre induce competitive vertical growth, resulting in canopy closure within two to three years.
*   **Microclimate formation:** Temperature reductions of up to 10–15 degrees Celsius and substantial increases in soil moisture and carbon accumulation follow shortly thereafter.

These characteristics make Miyawaki micro‑forests uniquely suited to rapid restoration of degraded substrates such as compacted roadbeds. The method’s accelerated growth trajectory aligns well with reinforcement learning feedback loops, which require measurable ecological change within short temporal windows.

### 2.2 Why Corridors, Not Patches

Miyawaki plantings achieve their greatest ecological impact when deployed as **corridors** rather than isolated patches.
*   **Topology alteration:** Corridors bridge gaps between habitat fragments, restoring movement pathways and gene flow.
*   **Edge suppression:** They reduce perimeter‑to‑area ratios, suppressing edge effects and increasing interior habitat.
*   **Root system benefits:** Root systems decompact roadbeds and facilitate mycorrhizal colonisation, further accelerating ecological recovery.

A corridor functions as a biological artery rather than a linear plantation. Its continuity and structural complexity enable it to sustain microclimatic conditions and ecological processes that isolated patches cannot replicate.

### 2.3 Corridor Design Elements

Effective corridor design requires attention to:
*   **Species stratification:** Multi‑strata species selection ensures structural complexity and ecological resilience.
*   **Planting density:** High‑density planting induces rapid vertical growth.
*   **Soil preparation:** Deep decompaction and organic amendment are essential for establishing root networks in compacted substrates.
*   **Continuity design:** Gaps should not exceed 20–30 metres, with wider nodes placed at regular intervals to enhance microclimatic stability.

These design principles provide the ecological foundation for the reinforcement learning optimisation framework.

---

## 3. Reinforcement Learning Framework for Topological Restoration

This section outlines the computational architecture that underpins the optimisation of Miyawaki corridor placement.

### 3.1 The Go Analogy as a Structural Framework

The analogy between ecological restoration and the game of Go provides a structural scaffold for understanding how reinforcement learning can optimise spatial decisions. Both domains require agents to evaluate millions of possible futures and optimise spatial configurations under uncertainty.

**Table 1: Conceptual mapping between Go and ecological restoration**

| Aspect | Game of Go | Ecological Restoration |
| :--- | :--- | :--- |
| **Goal** | Territorial control | Maximising Equivalent Connected Area (ECA) |
| **Action** | Placing stones on a grid | Selecting corridor placement/planting actions |
| **State** | Current board configuration | Multi-channel landscape tensor ($S_t$) |
| **Outcome** | Long-term strategic landscape | Ecological resilience and connectivity |
| **Evaluation** | Anticipating long-term strategic consequences | Evaluating $\Delta ECA$, Isoperimetric Ratio |

The analogy clarifies why AlphaGo‑style reinforcement learning is well suited to restoration planning.

### 3.2 State Space: Multi‑Channel Landscape Tensor

The reinforcement learning environment represents the landscape as a multi‑channel tensor:

$$S_t \in \mathbb{R}^{(H \times W \times C)}$$

Each channel encodes a distinct ecological, climatic, or socio‑political variable:

*   **Channel 0:** Canopy density (0–1)
*   **Channel 1:** Soil health index (0–1)
*   **Channel 2:** Road scar mask (binary)
*   **Channel 3:** Microclimate humidity (0–1)
*   **Channel 4:** Habitat classification (categorical)
*   **Channel 5:** Slope (degrees)
*   **Channel 6:** Hydrology (soil moisture)
*   **Channel 7:** Feasibility mask (land tenure, access constraints)
*   **Channel 8:** Climate indicator (rainfall, drought index)
*   **Channel 9:** Disturbance risk (fire, flood probability)

This explicit tensor structure ensures reproducibility and allows the agent to reason about ecological processes, climatic variability, and governance constraints simultaneously.

### 3.3 Action Space: Formal Definition

The agent selects one of three actions for each cell during each seasonal decision step:

*   **$A_0$ — Passive succession:** No intervention; natural regeneration proceeds.
*   **$A_1$ — Soil preparation:** Mechanical decompaction, organic amendment, and mycorrhizal inoculation.
*   **$A_2$ — Miyawaki planting:** High‑density, multi‑strata native species installation.

**Action masking** prohibits interventions in intact forest, steep slopes, culturally protected areas, private land without access, and riparian zones requiring special permits.

### 3.4 Reward Function: Mathematical and Ecological Integration

The reward function integrates connectivity, geometry, ecological maturity, and cost:

$$R_t = w_1 \cdot (\frac{\Delta ECA}{ECA_{max}}) - w_2 \cdot \Delta(\frac{P^2}{4\pi A}) + w_3 \cdot \Delta(\alpha C + \beta S + \gamma H) - \sum_i c_i(1 + \delta \cdot \text{Slope} + \eta \cdot \text{Distance})$$

This formulation ensures that the agent prioritises topological reconnection, ecological development, and cost‑effective placement.

#### 3.4.1 Equivalent Connected Area (ECA)
ECA is defined as:
$$\text{ECA} = \sum_{i=1}^{N} \sum_{j=1}^{N} a_i \cdot a_j \cdot p_{ij}^*$$
where $a_i$ and $a_j$ denote patch areas; $p_{ij}^*$ denotes the maximum product movement probability; and $N$ denotes the number of patches.

#### 3.4.2 Movement Probability
Movement probability is defined as:
$$p_{ij}^* = \max_{\pi \in \Pi_{ij}} \prod_{k \in \pi} (1 - r_k)$$
where $\Pi_{ij}$ is the set of all paths between patches $i$ and $j$; and $r_k$ is the resistance of cell $k$.

#### 3.4.3 Isoperimetric Ratio
The isoperimetric ratio is defined as:
$$C = \frac{P^2}{4\pi A}$$
where $P$ denotes perimeter and $A$ denotes area. This compactness metric penalises elongated geometries.

#### 3.4.4 Ecological Maturity
Ecological maturity is represented as:
$$M = \alpha C + \beta S + \gamma H$$
where canopy density ($C$), soil health ($S$), and humidity ($H$) contribute to ecological development.

#### 3.4.5 Contextual Cost
The cost term incorporates slope and distance:
$$\text{Cost}(a_i) = c_i \cdot (1 + \delta \cdot \text{Slope} + \eta \cdot \text{Distance})$$

### 3.5 Monte Carlo Tree Search and Neural Networks

The reinforcement learning agent employs a policy network to propose promising actions and a value network to estimate long‑term ecological outcomes. **Monte Carlo Tree Search (MCTS)** evaluates thousands of simulated futures, enabling the agent to anticipate long‑term consequences of planting decisions.

### 3.6 Expanded Transition Model

The transition model simulates ecological change between time steps, integrating various ecological dynamics:

*   **Canopy Growth:**
    $$C_{t+1} = C_t + r_{Miyawaki} \cdot (1 - C_t)^\beta$$
    Lateral spillover is defined as:
    $$C_{t+1}^{adj} = C_t^{adj} + \lambda_C \cdot C_t$$

*   **Soil Recovery:**
    $$M_{t+1} = M_t + D_M \cdot \nabla^2 M_t + \gamma H_t$$

*   **Microclimate Propagation:**
    $$\text{H}_{t+1} = H_t + \lambda_H \cdot C_t + D_H \cdot \nabla^2 H_t$$
    $$\text{T}_{t+1} = T_t - \kappa C_t$$

*   **Species Interactions:**
    $$P_{succ} = \sigma(C_t, S_t, H_t)$$

*   **Climate and Disturbance:**
    $$\text{X}_{t+1} \sim \mathcal{N}(\mu_X, \sigma_X)$$
    $$\text{S}_{t+1} = S_t \cdot (1 - s_e)$$

### 3.7 Emergent Strategy Discovery

The agent learns strategies such as:
*   Creating humidity anchors to accelerate corridor formation.
*   Prioritising soil preparation in drought‑prone zones.
*   Avoiding fire‑prone ridgelines.
*   Bridging large patches before small ones.
*   Using microclimate spillover to reduce overall planting costs.

---

## 4. The Topology of Fragmentation

Fragmentation is not merely a reduction in forest cover; it is a geometric and topological deformation of the habitat network.

### 4.1 Fragmentation as a Topological Deformation

The **Euler characteristic**, denoted by $\chi$, provides a topological invariant that captures the relationship between connected components and holes:
$$\chi = \text{Components} - \text{Holes}$$

Logging roads increase the number of holes while simultaneously reducing the number of connected components. This dual effect lowers $\chi$ and thereby diminishes the structural coherence of the landscape.

### 4.2 Corridors as Topological Repair

Miyawaki corridors reverse fragmentation by closing holes, merging components, and reducing perimeter. When a corridor bridges two isolated patches, it increases the number of connected components and reduces the number of holes, thereby increasing $\chi$.

The isoperimetric ratio provides a quantitative measure of geometric efficiency. Corridors that reduce this ratio create more compact, interior‑rich shapes that support ecological processes more effectively than elongated or fragmented geometries.

### 4.3 Why Reinforcement Learning Discovers Efficient Geometries

Reinforcement learning agents trained on ECA maximisation learn to prioritise actions that produce topological repair. They identify narrow gaps between patches as high‑value targets, bridge large patches before small ones, and avoid creating long, thin geometries that increase perimeter without improving connectivity.

---

## 5. Research Agenda

The research agenda is divided into four phases:

### 5.1 Phase 1 — Environment Construction (Months 1–6)
*   **Data Acquisition:** Acquiring high-resolution satellite imagery and LiDAR data to map existing vegetation canopy and topography.
*   **Tensor Generation:** Generating multi‑channel landscape tensors ($S_t$) containing hydrological, climatic, and ecological variables.
*   **Feasibility Mapping:** Implementing action masks that encode land tenure, access constraints, and legal zoning prohibitions.
*   **Model Calibration:** Calibrating baseline growth and microclimate parameters to ensure ecological realism.

### 5.2 Phase 2 — Reward Calibration (Months 4–9)
*   **Baseline Calculations:** Computing initial ECA baseline values across the target landscape.
*   **Resistance Validation:** Validating movement resistance parameters ($r_k$) using empirical species movement studies.
*   **Project Validation:** Benchmarking the reward function against existing, empirical Miyawaki corridor deployments.
*   **Weight Optimisation:** Calibrating weight factors ($w_1, w_2, w_3$) and cost penalties ($c_i$) to balance ecological efficacy with financial feasibility.

### 5.3 Phase 3 — Reinforcement Learning Training (Months 7–18)
*   **Multi-Scenario Training:** Training policy and value networks under diverse climate trajectories, including drought-heavy, fire-prone, and extreme rainfall events.
*   **Baseline Benchmarking:** Comparing agent output against heuristic baselines, such as expert-designed corridor networks and least-cost path models.
*   **Strategy Analysis:** Evaluating emergent structural patterns to identify novel spatial strategies that inform broader ecological theory.

### 5.4 Phase 4 — Pilot Deployment (Months 15–24)
*   **Site Selection:** Selecting pilot sites in road‑scarred areas featuring heterogeneous patch sizes, mixed land tenure, and diverse microclimates.
*   **Long-Term Monitoring:** Executing a 3–5 year empirical monitoring framework tracking canopy closure rates, soil recovery, fauna transit, and net ECA change.
*   **Feedback Integration:** Incorporating field observations into the transition model to refine the environment tensor for future deployment rounds.

---

## 6. Expected System Outputs

The framework generates a comprehensive suite of tools for planning and implementation:

*   **Corridor Placement Maps:** Spatially explicit maps identifying optimal corridor locations, integrating ecological, climatic, and socio‑political constraints.
*   **Species Mix Recommendations:** Species mixes tailored to local ecological conditions, drawing on the Miyawaki method’s emphasis on multi‑strata planting.
*   **Planting Density Maps:** Maps specifying spatial distribution of planting intensities to accelerate canopy closure and manage cost.
*   **Canopy Closure Projections:** Temporal projections of canopy closure based on the transition model, supporting monitoring and evaluation.
*   **Connectivity Dashboards:** Visual summaries presenting ECA values, movement probabilities, and compactness metrics for adaptive management.

---

## 7. Limitations and Open Questions

*   **Regional Calibration Requirements:** The transition model and reward function require region‑specific calibration due to significant variation in soil properties, growth rates, and climate.
*   **Sensitivity of ECA to Parameter Variation:** ECA is highly sensitive to movement resistance values and patch definitions, necessitating rigorous validation of movement resistance models.
*   **Socio‑Political Constraints:** The agent cannot resolve socio‑political conflicts or negotiate access rights; integration of socio‑political modelling is required.
*   **Climate Uncertainty:** Extreme climate events may exceed modelled ranges, requiring continuous model updating.
*   **Computational Cost:** Landscape‑scale reinforcement learning requires substantial computational resources, limiting accessibility.
*   **Ecological Risk:** Interventions may inadvertently facilitate invasive species movement or alter hydrological processes.

---

## 8. Conclusion

Version 0.4 presents a comprehensive and mathematically rigorous framework for optimising Miyawaki corridor placement using reinforcement learning. The integration of ecological theory, topological analysis, and computational optimisation provides a robust foundation for addressing the structural challenges posed by logging road fragmentation.

The restoration of connectivity is not merely a matter of planting trees; it is a **topological repair process** that requires strategic placement, ecological insight, and long‑term planning. Reinforcement learning offers a powerful tool for discovering geometrically efficient and ecologically resilient strategies. The research agenda provides a clear pathway for developing and deploying this framework in real landscapes.

---

## GLOSSARY

**Equivalent Connected Area (ECA)**
A graph‑theoretic measure of effective connected habitat area. ECA weights patch areas by the probability of movement between them, thereby capturing both the size and the permeability of the habitat network. Higher ECA values indicate greater ecological connectivity.

**Isoperimetric Ratio**
A compactness metric defined as $P^2 / 4\pi A$, where $P$ denotes perimeter and $A$ denotes area. Lower values indicate more compact, interior‑rich geometries.

**Miyawaki Method**
A high‑density, multi‑species planting technique that accelerates forest succession.

**Monte Carlo Tree Search (MCTS)**
A search algorithm that evaluates future states through stochastic simulation, used in reinforcement learning to explore possible action sequences.

**Movement Resistance**
A value representing the difficulty of species movement across a landscape cell, ranging from 0 (free movement) to 1 (complete barrier).

**Successional Stage**
A phase in ecological development, typically progressing from pioneer to early, mid, late, and climax stages.

**Transition Model**
The ecological simulator that updates landscape state between time steps, incorporating canopy growth, soil recovery, microclimate propagation, and disturbance regimes.

**Patch Adjacency Graph**
A graph representation of habitat patches and their connectivity, providing the structural basis for calculating ECA.

**Microclimate Spillover**
The propagation of humidity, shade, and temperature reduction from forest nodes into adjacent cells.

**Disturbance Regime**
A set of stochastic events (e.g., fire, flood, pest outbreaks) that affect ecological processes.

**Feasibility Mask**
A spatial layer encoding land tenure, access constraints, cultural protections, and legal restrictions, ensuring that RL strategies remain implementable.

**Hydrological Recovery**
The restoration of soil moisture, infiltration capacity, and water retention following disturbance or compaction.

**Connectivity Dashboard**
A visual summary of connectivity metrics, including ECA, movement probabilities, and compactness values, supporting adaptive management.

---

## Appendix A — Mathematical Formulations

### A.1 Equivalent Connected Area (ECA)
$$\text{ECA} = \sum_{i=1}^{N} \sum_{j=1}^{N} a_i \cdot a_j \cdot p_{ij}^*$$
This formulation captures both the size and the permeability of the habitat network.

### A.1.1 Movement Probability
$$p_{ij}^* = \max_{\pi \in \Pi_{ij}} \prod_{k \in \pi} (1 - r_k)$$
This formulation reflects the ecological reality that species movement is constrained by substrate conditions.

### A.2 Isoperimetric Ratio
$$C = \frac{P^2}{4\pi A}$$
This metric ensures that the reinforcement learning agent favours interior‑rich geometries.

### A.3 Ecological Maturity Function
$$M = \alpha C + \beta S + \gamma H$$
This function ensures that the agent rewards ecological development alongside connectivity gains.

### A.4 Reward Function
$$R_t = w_1 \cdot (\frac{\Delta ECA}{ECA_{max}}) - w_2 \cdot \Delta(\frac{P^2}{4\pi A}) + w_3 \cdot \Delta(\alpha C + \beta S + \gamma H) - \sum_i c_i(1 + \delta \cdot \text{Slope} + \eta \cdot \text{Distance})$$
This formulation ensures that the agent prioritises topological repair, ecological development, and cost‑effective placement.

### A.5 Canopy Growth Dynamics
$$C_{t+1} = C_t + r_{Miyawaki} \cdot (1 - C_t)^\beta$$
Lateral canopy spillover is represented as:
$$C_{t+1}^{adj} = C_t^{adj} + \lambda_C \cdot C_t$$

### A.6 Soil Moisture Diffusion
$$M_{t+1} = M_t + D_M \cdot \nabla^2 M_t + \gamma H_t$$

### A.7 Microclimate Propagation
$$\text{H}_{t+1} = H_t + \lambda_H \cdot C_t + D_H \cdot \nabla^2 H_t$$
$$\text{T}_{t+1} = T_t - \kappa C_t$$

### A.8 Successional Stage Transition
$$P_{succ} = \sigma(C_t, S_t, H_t)$$

### A.9 Disturbance Probability
$$\text{X}_{t+1} \sim \mathcal{N}(\mu_X, \sigma_X)$$
$$\text{S}_{t+1} = S_t \cdot (1 - s_e)$$

## Appendix B — Implementation Details

*   **B.1 Grid Resolution:** The environment uses a **$10 \text{ m} \times 10 \text{ m}$ grid resolution**.
*   **B.2 Action Masking Rules:** Prohibits interventions in intact forest, steep slopes, culturally protected areas, private land without access, and riparian zones requiring special permits.
*   **B.3 Movement Resistance Layers:** Includes road scars, bare soil, grassland, shrubland, young forest, and mature forest.
*   **B.4 Climate Scenarios:** Training incorporates multiple climate trajectories (baseline, drought-heavy, extreme rainfall, fire-prone).
*   **B.5 Disturbance Events:** Includes fire, flood, pest outbreak, illegal clearing, and windthrow, defined by probability, severity, and spatial footprint.
*   **B.6 Miyawaki Growth Calibration:** Draws on LiDAR canopy height models, soil moisture sensors, and vegetation plots for ecological realism.
*   **B.7 Computational Architecture:** Requires distributed GPU or TPU clusters, parallelised Monte Carlo rollouts, and memory‑efficient tensor compression.

## Appendix C — Terminology Glossary

*   **Equivalent Connected Area (ECA):** A measure of effective connected habitat area weighted by movement probability.
*   **Isoperimetric Ratio:** A compactness metric comparing perimeter to area ($P^2 / 4\pi A$).
*   **Miyawaki Method:** A high‑density, multi‑species planting technique that accelerates forest succession.
*   **Monte Carlo Tree Search (MCTS):** A search algorithm that evaluates future states through stochastic simulation.
*   **Movement Resistance:** A value representing the difficulty of species movement across a cell.
*   **Successional Stage:** Ecological development phases: pioneer, early, mid, late, and climax.
*   **Transition Model:** The ecological simulator that updates landscape state between time steps.
*   **Patch Adjacency Graph:** A graph representation of habitat patches and their connectivity.
*   **Microclimate Spillover:** Propagation of humidity, shade, and temperature reduction from forest nodes.
*   **Disturbance Regime:** Stochastic events such as fire, flood, or pest outbreaks.

## Appendix D — Validation Protocol

*   **D.1 Miyawaki Field Validation:** Assesses the transition model against empirical data (canopy closure rates, soil moisture recovery, microclimate formation).
*   **D.2 Connectivity Validation:** Examines whether predictions of movement probability and ECA align with observed wildlife movement (using camera traps, GPS-tagged species).
*   **D.3 Sensitivity Analysis:** Evaluates how variations in model parameters (reward weights, resistance values, disturbance probabilities) influence agent behaviour.
*   **D.4 Real‑World Pilot Deployment:** Tests recommendations in real landscapes over 3–5 years, using field data to update the transition model.

## Appendix E — Data Requirements

*   **E.1 Remote Sensing:** Required datasets include LiDAR canopy height models, multispectral satellite imagery, soil moisture radar, and road network vector layers.
*   **E.2 Field Data:** Required measurements include soil cores, microclimate sensors, vegetation plots, and wildlife movement data.

## Appendix F — Ethical and Governance Considerations

*   **F.1 Indigenous Land Rights:** Corridor placement must respect Indigenous land rights and involve co‑design with Indigenous communities.
*   **F.2 Community Engagement:** Projects should incorporate local employment and co‑management agreements.
*   **F.3 Ecological Risk:** Practitioners must avoid planting in sensitive riparian zones or creating corridors that facilitate invasive species movement. Adaptive management is essential.
