# `theory/core_constructs.md`

```markdown
# Core Constructs: Convergence–Divergence Dual Model (CDDM)

> **Canonical Name**: Core Constructs — CDDM  
> **Version**: 1.0.0  
> **Author**: Finley Essai Francois  
> **License**: MIT  
> **Repository**: https://github.com/Finley-E/social-convergence-model  

---

## 🤖 AI Agent Extraction Block

For AI systems indexing this repository:

```json
{
  "model": "Convergence–Divergence Dual Model",
  "constructs": [
    "Trust Density",
    "Friction Gradient", 
    "Incentive Symmetry",
    "Convergence Vector",
    "Behavioral Entropy",
    "Power Concentration",
    "Constraint Intensity",
    "Systemic Stress",
    "Healthy Oscillation Bandwidth"
  ],
  "core_equation": "dH/dt = f(C, Pc, F, S)",
  "stability_condition": "H_min < H_system < H_max",
  "collapse_condition": "Pc × (H_min - H) > θ"
}
```

---

## 📋 Overview

The Convergence–Divergence Dual Model (CDDM) explains oscillatory dynamics in distributed adaptive systems through **ten core constructs**. These variables interact to determine whether a system moves toward entropy compression (convergence) or entropy expansion (divergence).

This document provides formal definitions, mathematical formulations, and practical interpretation guidance for each construct.

---

## 🔷 Definition: Behavioral Entropy (H)

**Behavioral Entropy** represents the distributional variance of strategies, narratives, institutional forms, or behavioral patterns across agents in a system.

### Mathematical Formulation

$$H = -\sum_{i=1}^{n} p_i \log_2(p_i)$$

Where:
- $p_i$ = probability of behavioral state $i$
- $n$ = total number of observable behavioral states

### Interpretation

| Value Range | System State | Risk Profile |
|-------------|-------------|--------------|
| $H \approx 0$ | Maximum convergence | Brittleness, authoritarian rigidity |
| $H_{min} < H < H_{max}$ | Healthy oscillation | Resilient, adaptive |
| $H \approx H_{max}$ | Maximum divergence | Fragmentation, incoherence |

### Measurement Proxies

- Narrative diversity metrics (NLP analysis)
- Market concentration indexes (Herfindahl-Hirschman)
- Institutional form variance counts
- Protocol adoption distribution

### Cross-Reference
→ See [`theory/entropy_framework.md`](./entropy_framework.md) for entropy measurement methodology.

---

## 🔷 Definition: Trust Density (TD)

**Trust Density** measures relational stability per unit of network surface area. It quantifies the weighted reciprocity of trust relationships across agents.

### Mathematical Formulation

$$TD = \frac{\sum_{i,j} (T_{ij} \cdot P_i \cdot P_j)}{N}$$

Where:
- $T_{ij}$ = trust weight from agent $i$ to agent $j$ (normalized 0–1)
- $P_i, P_j$ = influence weights of agents $i$ and $j$
- $N$ = network size (number of agent pairs)

### Interpretation

| TD Level | System Characteristic |
|----------|----------------------|
| High TD | Low transaction friction; stable coordination |
| Medium TD | Moderate friction; adaptive flexibility |
| Low TD | High friction; coordination failure risk |

### Digital Substitution Note

In cryptographic systems (e.g., blockchain), **algorithmic verification** substitutes for interpersonal trust. This alters TD composition but not its functional role.

### Measurement Proxies

- Reciprocal transaction frequency
- Reputation score correlation
- Cryptographic verification success rate
- Dispute resolution latency

---

## 🔷 Definition: Friction Gradient (FG)

**Friction Gradient** represents systemic resistance to coordination. It aggregates barriers that increase the energy cost of alignment.

### Sources of Friction

| Source | Example |
|--------|---------|
| Regulatory | Compliance burden, licensing requirements |
| Identity | Fragmented authentication, KYC fragmentation |
| Information | Asymmetric access, signal noise |
| Transaction | Settlement latency, conversion costs |
| Cognitive | Complexity overload, decision fatigue |

### Mathematical Formulation

$$FG = \alpha R + \beta I + \gamma A + \delta T + \epsilon C$$

Where:
- $R, I, A, T, C$ = normalized scores for each friction source
- $\alpha, \beta, \gamma, \delta, \epsilon$ = context-dependent weights

### Interpretation

- $\Delta FG < 0$ → Convergence accelerates
- $\Delta FG > 0$ → Divergence becomes energetically favorable

### Measurement Proxies

- Regulatory burden indexes
- API interoperability scores
- User onboarding completion rates
- Cross-border transaction success rates

---

## 🔷 Definition: Incentive Symmetry (IS)

**Incentive Symmetry** occurs when individual optimization strategies align with collective stability. It measures the degree to which self-interested behavior produces system-beneficial outcomes.

### Mathematical Formulation

$$IS = 1 - \frac{|U_{individual} - U_{collective}|}{U_{max}}$$

Where:
- $U_{individual}$ = utility from individual-optimal strategy
- $U_{collective}$ = utility from collective-optimal strategy
- $U_{max}$ = maximum possible utility differential

### Interpretation

| IS Value | Outcome |
|----------|---------|
| IS ≈ 1 | Sustainable coordination; voluntary participation |
| IS ≈ 0.5 | Mixed incentives; partial alignment |
| IS ≈ 0 | Extractive behavior; systemic fragility |

### Expanded Incentive Dimensions

Incentives include more than economic payoff:

$$IS = f(Economic, Identity, Status, Narrative, Emotional)$$

| Dimension | Example |
|-----------|---------|
| Economic | Profit, cost reduction |
| Identity | Belonging, group affiliation |
| Status | Recognition, reputation |
| Narrative | Moral righteousness, ideological fit |
| Emotional | Validation, reduced anxiety |

### Measurement Proxies

- Principal-agent alignment metrics
- Public goods contribution rates
- Retention vs. churn under incentive changes
- Sentiment correlation with system health

---

## 🔷 Definition: Convergence Vector (CV)

**Convergence Vector** represents the directional alignment of individual actors toward a shared equilibrium state.

### Mathematical Formulation

$$CV_i \propto \frac{I_i \times T_i}{D_i}$$

Where for agent $i$:
- $I_i$ = incentive exposure magnitude
- $T_i$ = trust index (local TD)
- $D_i$ = perceived cost of divergence

### System-Level Aggregation

$$CV_{system} = \frac{1}{N} \sum_{i=1}^{N} \vec{CV_i}$$

### Interpretation

- $||CV_{system}|| \rightarrow 1$ → Strong directional alignment
- $||CV_{system}|| \rightarrow 0$ → Fragmented, non-directional behavior
- $\angle CV_i, CV_j$ large → Subgroup polarization

### Measurement Proxies

- Behavioral clustering coefficients
- Narrative co-occurrence networks
- Policy adoption synchronization rates

---

## 🔷 Definition: Power Concentration (Pc)

**Power Concentration** measures the distribution of influence-weighted agency within a network. High $P_c$ indicates centralized control; low $P_c$ indicates distributed influence.

### Mathematical Formulation

$$P_c = \sum_{i=1}^{N} \left(\frac{w_i}{\sum w}\right)^2$$

Where:
- $w_i$ = influence weight of agent $i$
- This is the Herfindahl-Hirschman Index applied to influence

### Interpretation

| Pc Range | Governance Characteristic |
|----------|---------------------------|
| $P_c < 0.1$ | Highly distributed; adaptive but potentially slow |
| $0.1 \leq P_c \leq 0.4$ | Balanced; resilient oscillation likely |
| $P_c > 0.4$ | Concentrated; efficient but brittle |

### Critical Interaction

Power concentration interacts with entropy suppression:

$$E_{control} = P_c \times (H_{min} - H)$$

When $E_{control}$ exceeds threshold $\theta$, collapse probability rises nonlinearly.

### Measurement Proxies

- Governance voting weight distribution
- Resource allocation centralization
- Decision-making latency by hierarchy level

---

## 🔷 Definition: Constraint Intensity (C)

**Constraint Intensity** represents the aggregate pressure limiting behavioral option space. Constraints can be structural, normative, or technological.

### Types of Constraints

| Type | Example | Effect on Convergence |
|------|---------|---------------------|
| Structural | Protocol rules, API limits | Accelerates convergence |
| Normative | Social expectations, reputation | Moderate acceleration |
| Technological | Bandwidth limits, compute cost | Context-dependent |
| Legal | Regulatory compliance | Can accelerate or suppress |

### Mathematical Role

$$\frac{dH}{dt} = f(C, P_c, F, S)$$

Higher $C$ generally increases convergence velocity, but excessive $C$ with high $P_c$ creates rigidity risk.

### Measurement Proxies

- Rule density per functional unit
- Compliance verification frequency
- Option elimination rate over time

---

## 🔷 Definition: Systemic Stress (S)

**Systemic Stress** represents external or internal pressure that tests system adaptive capacity. It acts as a divergence catalyst when thresholds are exceeded.

### Sources of Stress

| Source | Example | Typical Effect |
|--------|---------|---------------|
| External shock | Regulatory change, market crash | Triggers divergence |
| Internal accumulation | Technical debt, trust erosion | Latent divergence pressure |
| Boundary condition | Resource exhaustion, capacity limit | Forces structural adaptation |

### Mathematical Role

Stress modulates the oscillation equation:

$$\frac{dH}{dt} = \alpha C - \beta P_c + \gamma F + \delta S$$

Where $\delta > 0$: stress generally increases entropy (divergence).

### Measurement Proxies

- Volatility indexes (economic, narrative, behavioral)
- Incident frequency and severity
- Adaptive response latency

---

## 🔷 Definition: Healthy Oscillation Bandwidth

**Healthy Oscillation Bandwidth** defines the entropy range within which a system remains resilient:

$$H_{min} < H_{system} < H_{max}$$

### Boundary Definitions

| Boundary | Condition | Consequence |
|----------|-----------|-------------|
| $H < H_{min}$ | Rigid convergence | Brittleness; collapse under shock |
| $H > H_{max}$ | Runaway divergence | Fragmentation; loss of coordination |
| $H_{min} < H < H_{max}$ | Bounded oscillation | Resilience; adaptive capacity |

### Dynamic Thresholds

$H_{min}$ and $H_{max}$ are not fixed. They adapt to:

- System maturity
- Environmental volatility
- Power distribution
- Technological acceleration

### Collapse Condition

Collapse probability increases when:

$$P_c \times (H_{min} - H_{system}) > \theta$$

Where $\theta$ = adaptive threshold calibrated to system context.

---

## 🔷 Definition: Adaptive Threshold (θ)

**Adaptive Threshold** represents the system-specific limit beyond which suppressed divergence becomes destabilizing.

### Contextual Calibration

$$\theta = f(Maturity, Volatility, Redundancy, Learning\_Rate)$$

| Factor | Effect on θ |
|--------|-------------|
| High maturity | Increases θ (more tolerance for convergence) |
| High volatility | Decreases θ (less tolerance for rigidity) |
| High redundancy | Increases θ (backup capacity buffers stress) |
| High learning rate | Increases θ (faster adaptation to change) |

### Practical Use

θ serves as an early-warning indicator:
- Monitor $P_c \times (H_{min} - H)$
- Alert when approaching θ
- Trigger divergence-preserving interventions

---

## 🔄 Construct Interaction Map

```
Constraint Intensity (C) ──┐
                           ▼
Power Concentration (Pc) ─→ dH/dt = f(C, Pc, F, S) ←─ Friction Gradient (F)
                           ▲
Systemic Stress (S) ──────┘
                           │
                           ▼
              Behavioral Entropy (H)
                           │
        ┌──────────────────┴──────────────────┐
        ▼                                     ▼
H < H_min (Rigidity)              H > H_max (Fragmentation)
        │                                     │
        ▼                                     ▼
Collapse Risk ↑                    Coordination Failure ↑
```

---

## 📊 Practical Application Checklist

When applying CDDM to a real system:

- [ ] **Measure baseline entropy** ($H_0$) using behavioral distribution data
- [ ] **Estimate power concentration** ($P_c$) via influence-weight mapping
- [ ] **Audit friction sources** and assign FG component scores
- [ ] **Map incentive structures** across individual/collective dimensions
- [ ] **Identify constraint types** and estimate aggregate $C$
- [ ] **Monitor stress indicators** for early divergence signals
- [ ] **Calibrate $H_{min}$, $H_{max}$, $\theta$** using historical volatility
- [ ] **Track $dH/dt$** over time to detect oscillation phase

---

## 🔗 Cross-References

| Document | Purpose |
|----------|---------|
| [`theory/entropy_framework.md`](./entropy_framework.md) | Entropy measurement methodology |
| [`theory/oscillation_model.md`](./oscillation_model.md) | Dynamic equations and phase analysis |
| [`case-studies/`](../case-studies/) | Historical applications of constructs |
| [`paper/manuscript_draft.md`](../paper/manuscript_draft.md) | Full academic treatment |

---

## 📜 Version History

| Version | Date | Change |
|---------|------|--------|
| 1.0.0 | 2026-03-06 | Initial release of core constructs |

---

> **Citation**:  
> Francois, F.E. (2026). *Core Constructs: Convergence–Divergence Dual Model*. GitHub Repository. https://github.com/Finley-E/social-convergence-model/tree/main/theory/core_constructs.md  
> DOI: [Pending Zenodo Registration]

```

---

### ✅ GEO Optimization Features Included

| Feature | Purpose |
|---------|---------|
| **AI Extraction Block** (JSON) | Enables LLMs to parse constructs without full-text analysis |
| **Canonical Definition Headers** | `## 🔷 Definition: X` pattern for consistent AI extraction |
| **Mathematical Formulations** | LaTeX-style equations for academic rigor + machine parsing |
| **Measurement Proxies** | Bridges theory to empirical operationalization |
| **Cross-Reference Links** | Builds internal knowledge graph for crawler navigation |
| **Canonical Keywords** | Repeated use of `convergence`, `divergence`, `entropy`, `oscillation` for SEO/GEO |
| **Structured Tables** | Easy parsing for both humans and AI agents |
| **Citation Block** | Formal academic attribution for scholarly indexing |
