<div align="center">

# How Machines Represent Meaning

</div>

<div style="display: flex; justify-content: space-between;">

<a href="../episode-04/README.md">← Previous Episode</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="../episode-06/README.md">Next Episode →</a>

</div>

---

Machines represent meaning by converting **words, images, and concepts** into long lists of numbers called **vectors**.

Because computers only understand math and logic (ones and zeros), they can't feel or experience the real world the way humans do. Instead, they capture **meaning** using the **Distributional Hypothesis**.

> The `Distributional Hypothesis` is a foundational concept in linguistics and artificial intelligence, summarized by the famous quote by linguist John Rupert Firth:
>
> **"You shall know a word by the company it keeps."**
>
>## How It Works
>
>Machines do not have real-world experiences. They do not know what a **"banana"** tastes or looks like. Instead, they scan billions of sentences to see which words appear next to each other.
>
>### 1. The Setup
>
>Imagine a machine reads these sentences:
>
>- `"I ate a ripe banana."`
>- `"I ate a ripe apple."`
>
>### 2. The Pattern
>
>The machine notices that both **"banana"** and **"apple"** frequently appear next to words like:
>
>- `ate`
>- `ripe`
>- `sweet`
>- `fruit`
>
>### 3. The Conclusion
>
>Because **"banana"** and **"apple"** share a large amount of overlapping context, the machine concludes that they are **related concepts**.
>
>---
>
>## The Mathematical Map
>
>To use this hypothesis, AI systems build a giant **mathematical matrix (grid)**.
>
>### 1. Counting Context
>
>The machine tracks how often words appear near one another.
>
>### 2. Creating Coordinates
>
>These counts are turned into **coordinates (vectors)** on a multi-dimensional map.
>
>### 3. Measuring Closeness
>
>Concepts that are synonyms or belong to the same category naturally **cluster together** on this map because they share the same conversational >**"neighborhood."**
><p align="center">
>  <a href="./images/distributional-hypothesis.png">
>    <img 
>      src="./images/distributional-hypothesis.png" 
>      width="400"
>      alt="Architecture diagram"
>    />
>  </a>
>  <p align="center">
>    <em>Distributional Hypothesis</em>
>  </p>
></p>

