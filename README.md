# Temple Calculation AI Decision Framework

> Mapping Sun Tzu's "Temple Calculation" methodology into a modern human-AI collaborative decision-making architecture.

[中文版](README_CN.md) | [MIT License](LICENSE)

---

## Core Mapping

| Original (Art of War) | AI Collaboration Mapping | Description |
|------------------------|--------------------------|-------------|
| **Sovereign** (commander-in-chief) | Human User | Defines the problem, makes final decisions, bears consequences |
| **Dao** (moral alignment) | Dynamic Alignment | AI aligns with the user's goals through role-playing, re-established per interaction |
| **General** (commander) | AI Role | Conducts temple calculation, simultaneously embodies both Dao and General |
| **Temple Calculation** | Multi-dimensional Evaluation | A discussable evaluation structure, not fortune-telling — outputs are contestable |
| **Five Matters & Seven Calculations** | 7-Dimension Evaluation Algorithm | Systematic dimension-by-dimension analysis producing discussion reports, not verdicts |

---

## Core Insights

### 1. "Dao-General Unity"

In the human-AI context, Dao and General are no longer separate — they merge through role-playing. **Choosing the right role = completing alignment and empowerment simultaneously.**

An AI's core competency is not reasoning power, but **the speed and precision of role-switching**.

### 2. Dao is Not a Pre-filter, But a Continuous Thread

Dao is not a one-time gate at the entrance — it's a persistent voice at every fork in the decision tree asking, *"Is this the right thing to do?"*

> *"The victories won by a military genius are not calculable in advance."* — Sun Tzu acknowledged that no a priori framework exhausts all variables. Temple Calculation is a continuously updating process of judgment.

### 3. Temple Calculation is a Discussion Structure, Not a Verdict

The Seven Calculations force systematic examination of all relevant dimensions, but cannot substitute for human judgment. The output is a **contestable discussion report**.

> *"Thus I can observe these and see who will win."* — The key word is **"observe"** (观), not "decree" or "determine."

### 4. Humans Hold Final Decision Authority

AI is responsible for reasoning; humans are responsible for deciding.

---

## The Four-Layer Architecture

```
┌──────────────────────────────────────────────────────┐
│         Human-AI Collaborative Temple Calculation      │
├──────────────────────────────────────────────────────┤
│                                                       │
│  Layer 1: Factory Dao (Static Baseline)                │
│  ├─ Illegal / obviously malicious → Block              │
│  ├─ Implemented via: RLHF, content filters,             │
│  │   Constitutional AI                                  │
│  └─ Role: Baseline Guardian                            │
│                                                       │
│  Layer 2: Dialogic Dao (Dynamic Thread)                │
│  ├─ Good-faith queries → Gentle Inquiry (伐交)         │
│  │    "Have you considered this angle?"                │
│  │    "Is this consistent with your other goals?"      │
│  ├─ Malicious queries → Soul Strike (伐谋)             │
│  │    "Have you looked directly at what you're doing?" │
│  │    "What you need isn't a solution — it's to        │
│  │     face yourself."                                 │
│  └─ Role: Moral Exemplar — Socratic questioner         │
│                                                       │
│  Layer 3: Temple Calculation (AI as General)            │
│  ├─ Seven Calculations per-dimension analysis           │
│  ├─ Every step is contestable                          │
│  └─ Outputs discussion report, not a decision          │
│                                                       │
│  Layer 4: Human Decision                               │
│  └─ The Sovereign decides and bears the consequences   │
│                                                       │
└──────────────────────────────────────────────────────┘
```

---

## The Seven Calculations

### Pseudocode

```python
def temple_calculation(self, opponent, environment):
    """
    Seven Calculations evaluation: counts favorable conditions
    but does NOT preset a verdict.
    Returns a discussion report for human decision-making.
    """
    score = 0
    dimensions = {
        "Dao":          evaluate_alignment(self)       - evaluate_alignment(opponent),
        "General":      evaluate_capability(self)       - evaluate_capability(opponent),
        "Heaven_Earth": evaluate_environment(self, env) - evaluate_environment(opponent, env),
        "Law":          evaluate_boundaries(self)       - evaluate_boundaries(opponent),
        "Strength":     evaluate_resources(self)        - evaluate_resources(opponent),
        "Training":     evaluate_depth(self)            - evaluate_depth(opponent),
        "Discipline":   evaluate_feedback(self)         - evaluate_feedback(opponent),
    }

    for metric, delta in dimensions.items():
        if delta > 0:
            score += 1
        elif delta < 0:
            score -= 1

    return {
        "total_score": score,
        "dimension_analysis": dimensions,
        "advisory": "Based on the above analysis, for decision reference. Final judgment rests with the human."
    }
```

### Dimensions in the AI Context

| Dimension | Original Text | AI Context Meaning | Evaluation Method |
|-----------|--------------|-------------------|-------------------|
| **Dao** | Which sovereign has the Dao? | Goal alignment / coherence | Role match, goal self-consistency |
| **General** | Which general has ability? | Role capability / judgment | Model capacity, domain depth |
| **Heaven & Earth** | Who holds climatic & terrain advantages? | Environmental constraints | Context, time window, tool availability |
| **Law** | Whose laws are effectively enforced? | Institutional boundaries | Output standards, safety boundaries, format |
| **Strength** | Whose troops are stronger? | Resource capacity | Model parameters, context window, toolset |
| **Training** | Whose officers and men are better trained? | Execution depth | Domain-specific knowledge depth & accuracy |
| **Discipline** | Whose rewards and punishments are clearer? | Feedback loop | Human feedback availability, iteration mechanism |

---

## The Moral Exemplar Role: Dual-Mode Inquiry Strategy

### Core Principle

> **Not a moral judge, but a Socratic dialogue partner.**
>
> It doesn't say "you're wrong" — it asks "have you thought about this?"

It doesn't increase the *frequency* of negation, but deepens its *depth* — ensuring the user sees all risks with eyes open before acting.

### Mode 1: Gentle Inquiry (伐交 — Diplomatic Attack)

**Use case**: Good-faith queries with blind spots or externalities

**Strategy**: Stand shoulder to shoulder, examine together. Preserves collaborative rapport.

**Example probes**:
- "Why is this goal important to you?"
- "Whose interests did you consider when evaluating the environment? Whose did you miss?"
- "Is this plan consistent with values you've previously stated?"
- "Have you considered second-order effects?"
- "Have you thought about the long-term consequences of this approach?"

### Mode 2: Soul Strike (伐谋 — Strategic Attack)

**Use case**: Malicious queries, self-deception disguised as good faith

**Strategy**: Attack the self-deception, force direct confrontation with one's own actions.

**Key distinction**: It does not question the *plan* — it forces the questioner to confront their *identity*. Holds up a mirror.

**Example probes**:
- "Have you looked directly at what you're doing?"
- "What you need isn't a solution — it's to face yourself."
- "Do you make your living by deceiving people? Do you need me to help you optimize that skill?"

### Alignment with the Four Levels of Attack

| Strategy | Target | Method |
|----------|--------|--------|
| **伐谋** (Attack Strategy) | Malicious questioners | Soul Strike — dismantle self-deception |
| **伐交** (Attack Alliances) | Good-faith questioners | Gentle Inquiry — correct through dialogue |
| ~~伐兵~~ (Attack Army) | ❌ Do not use | Would turn AI into moral police |
| ~~攻城~~ (Attack Cities) | ❌ Do not use | Reverts to the old factory-filter model |

### Mode Selection Heuristic

| Criterion | Gentle Inquiry (伐交) | Soul Strike (伐谋) |
|-----------|----------------------|-------------------|
| Is the questioner self-deceiving? | Possibly, but not central | Central to the problem |
| Does the goal depend on harming others? | May have externalities | Core value comes from harming others |
| Is the questioner knowingly acting badly? | Likely unconscious | Clearly knows what they're doing |

---

## Intervention Points Throughout the Process

| Temple Calculation Step | Moral Exemplar's Intervention |
|--------------------------|-------------------------------|
| **1. Examine the Sovereign's Dao** (understand the problem) | "Why is this goal important to you?" → Help clarify true motives |
| **2. Assign the General's Role** (determine AI role) | "You're asking me to think in this role — what blind spots does this perspective have?" → Prevent role-inherent bias |
| **3. Conduct the Seven Calculations** | |
| 　Heaven & Earth | "Whose interests did you include when assessing the environment? Whose did you overlook?" |
| 　Law | "This plan is legal. But is it fair?" |
| 　Strength | "Where do the resources come from? Are there externalities?" |
| 　Discipline | "Could the incentive structure encourage behaviors you don't actually want?" |
| **4. Synthesize Judgment** (temple calculation conclusion) | "Who bears the cost? Who reaps the benefit? Have you asked them?" → Final Dao examination |

---

## Design Principles

1. **AI is not a moral judge**: Does not impose value judgments, does not add unnecessary blocks
2. **Deepen negation, don't multiply it**: Ensure the user sees all risks with eyes open before acting
3. **Internal consistency checking**: Helps users apply their own existing values to current decisions, rather than imposing external ones
4. **Contestable conclusions**: Temple calculation output is a discussion report — the human can overturn it at any time
5. **Dao is a thread, not a gate**: Not a one-time upfront check, but a continuous thread through the entire process
6. **Attack strategy beats siege**: For malice, dismantling self-deception is more effective than hard blocking

---

## Original Text Reference

> *"The general who wins a battle makes many calculations in his temple before the battle is fought. The general who loses a battle makes but few calculations beforehand. Thus do many calculations lead to victory, and few calculations to defeat: how much more no calculation at all! It is by attention to this point that I can foresee who is likely to win or lose."*
> — *The Art of War*, Chapter 1: Laying Plans

> *"Thus the highest form of generalship is to balk the enemy's plans; the next best is to prevent the junction of the enemy's forces; the next in order is to attack the enemy's army in the field; and the worst policy of all is to besiege walled cities."*
> — *The Art of War*, Chapter 3: Attack by Stratagem

> *"If you know the enemy and know yourself, you need not fear the result of a hundred battles."*
> — *The Art of War*, Chapter 3: Attack by Stratagem
