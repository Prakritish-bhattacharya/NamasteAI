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

Let's go one step deeper into the language of LLMs. Here is where things get really interesting.

**Imagine I say:**  `I went to the bank to deposit money.`

**Now I say:** `I sat near the bank and watched the river.`

The word `bank` is exactly the same in both sentences. But its meaning is completely different. In the first sentence, ***bank = financial institution*** and in second sentence, ***bank = side of a river***. 
<p align="center">
  <a href="./images/bank-story.png">
    <img 
      src="./images/bank-story.png" 
      width="600"
      alt="Architecture diagram"
    />
  </a>
  <p align="center">
    <em>Visual</em>
  </p>
</p>

**So here is the mystery:**

How does an AI model figure out that the same word means different things depending on the sentence?
This is one of the key problems NLP and modern language models are designed to solve. We already learned about tokenization and token IDs. Suppose the tokenizer gives us uniques IDs **Dog** represented with `8123`, **Grapes** with `8521` and **Elephant** with `17234`. The numerical distance between these IDs tells us nothing about their meaning. 
**Remember this: Token ID = identity, not meaning.** And this is an extremely important distinction.

__So Where Does Meaning Come From?__ 

Now comes the interesting part.The model doesn't try to understand the meaning of `8123`. Instead, that token ID is used to look up a learned numerical representation. 👇
<p align="center">
  <a href="./images/embedding.png">
    <img 
      src="./images/embedding.png" 
      height="300" width="400"
      alt="Architecture diagram"
    />
  </a>
  <p align="center">
    <em>Embedding Visual</em>
  </p>
</p>

That final vector is where the interesting information begins to appear.But even that isn't the whole story. Because now we have another mystery.

### Let's return to our bank example.

```text
Sentence 1:
"I deposited money in the bank."

Sentence 2:
"I sat beside the river bank."
```
The tokenizer might produce a token for `bank` in both sentences. So we could have `bank--> same token ID`. Yet the meaning is different. How can the model distinguish them?
> The answer is:
>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Context**
>

The model doesn't look at the word bank in isolation. It looks at the words surrounding it.

```text
"I deposited money in the bank."

                    bank
                     ↑
           ┌─────────┼─────────┐
           │         │         │
       deposited    money      the
```
The surrounding words strongly suggest:
```text
bank + deposited + money
              ↓
       financial institution
```
Here, **"bank"** means a place where we deposit or manage money.

Now look at:
```text
"I sat beside the river bank."

                    bank
                     ↑
           ┌─────────┼─────────┐
           │         │         │
          river     beside      the
```

The surrounding words suggest:

```text
bank + river + beside
              ↓
         river bank
```
Here, **"bank"** means the **side of a river**.

The word **"bank"** itself has not changed.

What changes is the **context around the word**.

```text
Same Token
    │
    ▼
  "bank"
    │
    ├── deposited + money
    │         ↓
    │   Financial Institution
    │
    └── river + beside
              ↓
          River Bank
```

> **The token gives the model the identity of the word, but the surrounding context helps determine its meaning.**

So the model isn't asking **"What does the token ID `4217` mean?"** Instead, it is effectively learning **"What does this token mean given everything around it?"** That's a much more powerful question.

And this is where **Embeddings** become important. Remember our earlier discussion about vectors. A token can be represented using a vector:
```text
bank
 ↓
[0.21, -0.43, 0.71, 0.18, ...]
```
But when the model processes an entire sentence, it uses the surrounding context to build a richer representation.

**Conceptually:**

```text
"I deposited money in the bank."
              ↓
        [financial context]
              ↓
        bank representation
```

<p align="center">versus</p>

```text
"I sat beside the river bank."
              ↓
          [river context]
              ↓
        bank representation
```

So:
```text
bank + financial context
          !=
bank + river context
```

This is the foundation of contextual representations. And this leads us directly to one of the most important ideas in modern NLP:
>**A word does not have to carry its complete meaning by itself. Its surrounding context helps determine what it means.**

That's exactly why the journey from Token IDs → Embeddings → Contextual Embeddings is so important. And now we are ready to go one level deeper: how does the model actually combine all those surrounding tokens to construct that contextual meaning?