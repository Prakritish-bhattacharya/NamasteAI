<div align="center">

# 🧠 NamasteAI — Deep Technical Learning Repository

### Understanding AI beyond the surface

**Learn → Research → Visualize → Understand → Share**

<br/>

[![Course](https://img.shields.io/badge/Course-Namaste%20AI-blue)](https://namastedev.com/learn/namaste-ai)
[![Focus](https://img.shields.io/badge/Focus-AI%20%26%20LLMs-purple)](#-what-is-this-repository)
[![Documentation](https://img.shields.io/badge/Style-Technical%20Deep%20Dives-green)](#-how-to-read-this-repository)

</div>

---

## 📖 About This Repository

**NamasteAI** is my personal technical documentation and learning repository for the **Namaste AI** course by **[Akshay Saini](https://www.linkedin.com/in/akshaymarch7/)**, launched on the **[NamasteDEV](https://namastedev.com/)** platform.

The goal of this repository is not to simply write down what is taught in each episode.

Instead, I am trying to go **one level deeper**.

For every episode, I identify the important concepts, research how they work behind the scenes, build mental models, create architecture diagrams, explore practical examples, and collect useful resources for further learning.

> **The course teaches the concept.  
> This repository documents my attempt to deeply understand the concept.**

---

# 🎓 Course Credit

This repository is based on the **Namaste AI** course created and taught by:

### **[Akshay Saini](https://www.linkedin.com/in/akshaymarch7/)**

The original course is available through the **[NamasteDEV](https://namastedev.com/)** platform.

All credit for the original course content, teaching, explanations, and episode structure goes to **[Akshay Saini](https://www.linkedin.com/in/akshaymarch7/)** and the **[NamasteDEV](https://namastedev.com/)** platform.

This repository is an independent learning and documentation effort built around my understanding and research of the concepts covered in the course.

---

# 🎯 What Is This Repository?

A course can explain **what something is**.

But while learning AI, I often want to understand:

- Why do we need it?
- What problem does it solve?
- How does it work?
- What happens behind the scenes?
- What does the architecture look like?
- How does it connect with other AI concepts?
- Where is it used in real systems?
- What should I learn next?

That is the purpose of this repository.

### The learning approach

```text
                    Namaste AI Episode
                           │
                           ▼
                  Identify Key Concepts
                           │
                           ▼
                      Research
                           │
                           ▼
                  Understand Internals
                           │
                           ▼
                  Create Mental Models
                           │
                           ▼
                  Draw Architecture
                           │
                           ▼
                  Add Practical Examples
                           │
                           ▼
                  Collect References
                           │
                           ▼
                  Document Everything
                           │
                           ▼
                    Share & Learn
```

---

# 🗂️ Repository Structure

```text
NamasteAI/
│
├── Seasons/
│   │
│   ├── season1/
│   │   ├── episode-01/
│   │   │   ├── README.md
│   │   │   └── images/
│   │   │
│   │   ├── episode-02/
│   │   │   ├── README.md
│   │   │   └── images/
│   │   │
│   │   └── episode-03/
│   │       ├── README.md
│   │       └── images/
│   │
│   └── season2/
│       └── ...
│
|
│
└── README.md
```

> The exact number of episodes, images, and supporting files will grow as the repository grows.

---

# 📁 What Does Each Folder/File Do?

## `README.md`

This is the **home page of the repository**.

It explains:

- What this project is
- Why it exists
- How the repository is organized
- How to read the episodes
- How to contribute
- Course and author information

Think of it as the **map of the entire repository**.

---

## `Seasons/`

This is the main container for all course seasons.

Instead of putting every episode into one huge folder, the content is separated by season.

```text
Seasons/
│
├── season1/
├── season2/
└── ...
```

This keeps the repository scalable as more seasons are documented.

---

## `season1/`

Contains all the deep-dive documentation for **Season 1**.

Each episode gets its own folder so that the explanation, diagrams, and other supporting material remain together.

```text
season1/
│
├── episode-01/
├── episode-02/
├── episode-03/
└── ...
```

---

## `season2/`

Contains the documentation for **Season 2**.

The same organizational pattern will be followed for future seasons:

```text
season2/
│
├── episode-01/
├── episode-02/
├── episode-03/
└── ...
```

---

## `episode-XX/`

Each episode is treated as an **independent technical article**.

For example:

```text
episode-03/
│
├── README.md
└── images/
```

The idea is that a reader should be able to open `README.md` and read the complete episode without jumping between multiple Markdown files.

---

## `episode-XX/README.md`

This is the **main technical blog for that episode**.

A typical episode article can contain:

```text
Episode Overview
      ↓
What You'll Learn
      ↓
Concept 01
      ↓
Concept 02
      ↓
Behind the Scenes
      ↓
Architecture
      ↓
Practical Example
      ↓
Implementation
      ↓
Real-World Applications
      ↓
How Everything Connects
      ↓
Key Takeaways
      ↓
Further Reading
```

The goal is to provide a **continuous reading experience**.

---

## `episode-XX/images/`

Contains diagrams, architecture illustrations, and other visual material used inside the episode article.

For example:

```text
images/
├── architecture.png
├── concept-01.png
├── inference.png
└── transformer.webp
```

Keeping images close to their episode makes relative Markdown links simple and keeps the repository organized.

---


# 🧭 How to Read This Repository

There are two good ways to explore the repository.

## 🚶 Start From the Beginning

If you are learning AI from scratch, follow the seasons and episodes sequentially:

```text
Season 1
   │
   ├── Episode 01
   │
   ├── Episode 02
   │
   ├── Episode 03
   │
   └── ...
         │
         ▼
      Season 2
         │
         └── ...
```

This gives you a more structured learning path.

---

## 🔎 Jump Directly to a Concept

If you already know the basics, you can browse the episode folders and jump directly to a topic that interests you.

For example:

```text
LLM
│
├── Token Prediction
├── Base Model
├── Instruct / Chat Model
├── Inference
├── Hallucination
├── Knowledge Cutoff
└── ...
```

Each article is designed to be understandable on its own as much as possible.

---

# 🧠 How Each Episode Is Documented

The episode documentation follows a common structure.

### 1. 📌 Episode Context

A short introduction explaining the episode and its major ideas.

### 2. 🧠 Core Concepts

Important concepts are identified and explained individually.

### 3. 🔬 Behind the Scenes

The explanation goes deeper into what happens internally.

### 4. 🏗️ Architecture

Diagrams are used whenever a visual representation can make the concept easier to understand.

### 5. 💻 Practical Examples

Simple examples are included to connect theory with real-world behavior.

### 6. 🧩 Connections

Related concepts are connected so the reader can understand the bigger picture.

### 7. 📚 Further Reading

Useful documentation, research papers, tutorials, engineering articles, and implementations are collected for readers who want to go deeper.

### 8. 💡 Key Takeaways

The most important ideas are summarized at the end.

---

# 🎨 Why One README Per Episode?

I intentionally prefer:

```text
episode-03/
└── README.md
```

instead of:

```text
episode-03/
├── concepts.md
├── resources.md
├── diagrams.md
└── README.md
```

The reason is **reader experience**.

A technical article should feel like one continuous journey:

```text
Concept
  ↓
Explanation
  ↓
Diagram
  ↓
Example
  ↓
Deep Dive
  ↓
Reference
```

The reader should not constantly navigate between different Markdown files to understand one concept.

Images can still live in an `images/` folder because they are supporting assets rather than separate articles.

---

# 🔗 Navigation Philosophy

As the repository grows, navigation will follow a simple pattern:

```text
Repository
   │
   ▼
Season
   │
   ▼
Episode
   │
   ▼
Concept
   │
   ├── Previous Episode
   ├── Next Episode
   ├── Related Concepts
   ├── Architecture
   └── Further Reading
```

Each episode should ideally provide links to:

- Previous episode
- Next episode
- Important related concepts
- External learning resources

---

# 🤝 How to Contribute

This repository is primarily a learning project, but **learning becomes better when people share ideas and corrections**.

If you find:

- A factual mistake
- A broken link
- A confusing explanation
- A better diagram
- A missing concept
- A useful research paper
- A better example
- A technical improvement

you are welcome to contribute.

## Contribution Workflow

```text
Find Something to Improve
          │
          ▼
      Fork Repository
          │
          ▼
     Create a Branch
          │
          ▼
     Make Your Changes
          │
          ▼
      Review Changes
          │
          ▼
      Commit Changes
          │
          ▼
       Push Branch
          │
          ▼
    Open Pull Request
```

### Suggested branch names

```text
docs/improve-episode-03
docs/add-episode-04
fix/broken-resource-link
docs/improve-diagram
```

### Suggested commit messages

```text
docs: improve episode 03 explanation
docs: add episode 04
docs: add transformer architecture diagram
fix: correct broken reference link
```

---

# 📝 Contribution Guidelines

When contributing, please try to keep the same philosophy as the rest of the repository:

### Keep explanations beginner-friendly

Avoid unnecessary jargon.

When a technical term is required, explain it before using it heavily.

### Prefer diagrams when they add value

A good architecture diagram can communicate what several paragraphs cannot.

### Explain the "why"

Don't only explain:

> **What is it?**

Also explain:

> **Why do we need it?**

and:

> **How does it work behind the scenes?**

### Cite useful sources

When adding technical information, prefer reliable sources such as:

- Official documentation
- Research papers
- University resources
- Well-known engineering blogs
- Original papers
- Reputable technical repositories

### Keep the reader's journey in mind

The goal is not to make the article as complicated as possible.

The goal is:

> **Make a difficult concept easier to understand without removing the important technical depth.**

---

# ⚠️ Important Note About the Content

This repository represents **my personal learning, interpretation, research, and documentation** of concepts discussed while studying Namaste AI.

It should not be considered an official NamasteDEV course repository or official documentation from Akshay Saini.

The original course remains the primary source for the course lessons.

This repository is intended to complement that learning by providing additional explanations, diagrams, references, and technical exploration.

---

# 👨‍💻 Author

## [Prakritish Bhattacharya](https://www.linkedin.com/in/prakritish-bhattacharya/)

This repository is part of my journey to understand AI beyond simply using AI tools.

I am trying to learn by following a cycle:

```text
        Learn
          ↓
       Question
          ↓
       Research
          ↓
      Experiment
          ↓
      Visualize
          ↓
      Understand
          ↓
        Write
          ↓
        Share
          ↓
      Learn More
```

The goal is not to pretend that I already know everything.

The goal is to **document the process of going deeper**.

---

# 🌱 Learning Philosophy

> **Don't just learn what the model does.  
> Try to understand why it works.**

A concept becomes much easier to remember when you can explain:

```text
What?
  ↓
Why?
  ↓
How?
  ↓
What happens behind the scenes?
  ↓
How does it connect to other concepts?
  ↓
Where is it used?
```

That is the philosophy behind this repository.

---

# 🗺️ Repository Roadmap

As the learning journey continues, this repository will gradually expand with:

- [ ] More Season 1 episodes
- [ ] Season 2 documentation
- [ ] More architecture diagrams
- [ ] More practical experiments
- [ ] More research references
- [ ] Cross-episode concept connections
- [ ] Better navigation between related concepts
- [ ] Deeper explorations of modern AI systems

---

# ⭐ If This Repository Helps You

If you find this repository useful for your own AI learning journey, consider giving it a **⭐ Star on GitHub**.

It is a small gesture, but it helps me know that these deep dives are useful to other learners and motivates me to keep documenting the journey.

<div align="center">

### ⭐ Found it useful? Give the repository a Star!

### 🧠 Learn. Research. Visualize. Understand. Share.

**Namaste AI × Deep Technical Learning**

<br/>

Made with curiosity by **Prakritish Bhattacharya**

</div>
