---
layout: default
title: "Sample Answer — Module 03: Neural Network Explainer"
permalink: /assessments/sample-answers/module-03/
---

# Sample Answer — Module 03
## Assignment: Neural Network Explainer

**Brief:** Create a one-page visual explainer showing how a Transformer model processes a sentence.

<span class="marks-badge">10 marks</span>

---

<div class="sample-answer">
<h4>📄 Model Answer — How a Transformer Processes "The cat sat on the mat"</h4>

A Transformer model processes text in four main stages: tokenisation, embedding, attention, and output generation. Here is how the sentence **"The cat sat on the mat"** flows through the model.

</div>

---

## Stage 1 — Tokenisation

The sentence is split into **tokens** — the basic units the model processes. Each token is roughly 3–4 characters or one short word.

```mermaid
graph LR
    S["The cat sat on the mat"] --> T1["The"]
    S --> T2["cat"]
    S --> T3["sat"]
    S --> T4["on"]
    S --> T5["the"]
    S --> T6["mat"]

    T1 --> ID1["Token ID: 464"]
    T2 --> ID2["Token ID: 3797"]
    T3 --> ID3["Token ID: 3332"]
    T4 --> ID4["Token ID: 319"]
    T5 --> ID5["Token ID: 262"]
    T6 --> ID6["Token ID: 2603"]

    style S fill:#ddf4ff,stroke:#0969da
```
<p class="diagram-caption">Each word becomes a numeric token ID that the model can process mathematically</p>

---

## Stage 2 — Embeddings

Each token ID is converted into a **vector** — a list of hundreds of numbers that captures its meaning. Similar words have similar vectors.

```mermaid
graph TD
    T["Token: cat\nID: 3797"] --> E["Embedding Vector\n[0.23, -0.41, 0.87, 0.12, ...]"]
    E --> P["+ Position Encoding\n(adds word order information)"]
    P --> V["Final Input Vector\n[0.31, -0.38, 0.91, 0.19, ...]"]

    style T fill:#f6f8fa,stroke:#d0d7de
    style E fill:#dafbe1,stroke:#2da44e
    style P fill:#fff8c5,stroke:#d4a72c
    style V fill:#ddf4ff,stroke:#0969da
```
<p class="diagram-caption">Without position encoding, the model would treat "cat sat" and "sat cat" identically</p>

---

## Stage 3 — Attention Mechanism

The **attention mechanism** is the key innovation of Transformers. Every token looks at every other token and decides how much to "pay attention" to it when building its representation.

```mermaid
graph TD
    subgraph Attention["Self-Attention: what does 'sat' focus on?"]
        SAT["sat"] -->|"high attention 0.7"| CAT["cat\n(who sat?)"]
        SAT -->|"high attention 0.6"| MAT["mat\n(sat where?)"]
        SAT -->|"low attention 0.1"| THE1["the"]
        SAT -->|"low attention 0.1"| ON["on"]
    end

    style Attention fill:#f6f8fa,stroke:#d0d7de
    style SAT fill:#ddf4ff,stroke:#0969da
    style CAT fill:#dafbe1,stroke:#2da44e
    style MAT fill:#dafbe1,stroke:#2da44e
```
<p class="diagram-caption">Attention scores show which words are most relevant to understanding each token in context</p>

---

## Stage 4 — Output Generation

After attention, the model predicts the most likely next token one at a time.

```mermaid
sequenceDiagram
    participant P as Prompt
    participant M as Transformer Model
    participant O as Output

    P->>M: "The cat sat on the"
    M->>O: Predicts → "mat" (probability: 0.87)
    O->>M: "The cat sat on the mat"
    M->>O: Predicts → "." (probability: 0.72)
    O->>M: "The cat sat on the mat."
    M->>O: Predicts → [END] token
```
<p class="diagram-caption">Token-by-token generation — each prediction feeds back as input for the next</p>

---

## Full Pipeline Summary

```mermaid
flowchart LR
    A["📝 Input Text"] --> B["🔢 Tokenise"]
    B --> C["📐 Embed + Position"]
    C --> D["👁️ Self-Attention\n(multiple layers)"]
    D --> E["🧮 Feed-Forward\nNetwork"]
    E --> F["🎯 Output\n(next token)"]
    F -->|"Feed back in"| D

    style A fill:#f6f8fa,stroke:#d0d7de
    style D fill:#ddf4ff,stroke:#0969da
    style F fill:#dafbe1,stroke:#2da44e
```
<p class="diagram-caption">The Transformer processes all tokens in parallel (unlike RNNs) — making it dramatically faster to train</p>

---

## How This Answer Scores

| Criteria | Marks | What this answer does |
|----------|-------|-----------------------|
| Diagram accurate and labelled | 4 | 5 diagrams covering all 4 stages |
| Explanation in student's own words | 3 | Plain language throughout |
| Attention mechanism correct | 2 | Shows which tokens attend to which |
| Presentation clear | 1 | Structured with captions |
| **Total** | **10** | |

---

<div class="tip-box">
<strong>💡 Examiner Tip:</strong> Many students draw a generic "input → hidden layers → output" neural network diagram and call it a Transformer. That scores 2/4 for the diagram at best. The Transformer is distinguished by the <em>attention mechanism</em> — your explainer must show how tokens relate to each other, not just how data flows through layers.
</div>
