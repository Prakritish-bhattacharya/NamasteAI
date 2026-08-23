<div align="center">

# The Secret Language of LLMs

</div>


<div style="display: flex; justify-content: space-between;">

<a href="../episode-03/README.md">← Previous Episode</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="../episode-05/README.md">Next Episode →</a>

</div>

---



LLMs basically does not understand words. They turn words into numbers and map them into a giant mathematical space. Sequence of token ID LLMs understand. Spliting words into [token]() is called [tokenization](###-Tokenization).

<p align="center">
  <a href="./images/token.png">
    <img 
      src="./images/token.png" 
      width="400"
      alt="Architecture diagram"
    />
  </a>
  <p align="center">
    <em>From Text to Token IDs: How Tokenization Works</em>
  </p>
</p>

### Tokenization

Tokenization is the process of converting text into a sequence of tokens. 

Tokens can be words, subwords or characters. 

Tokens are the smallest meaning of a text that can be processed by a LLM ( Large Language Model ). In the LLM pre-training phase after tokenization each token assigned a unique integer. For each integer, there is a corresponding row in a `lookup table`, which is the vector presentation of that token. 

#### Why do we need Tokenization?

Suppose Prakritish want to `pre-train` his own language model. And he have `100 GB` textual data.Main problem is  Language models or any ML models can only process numbers. Here he needs a method to convert his text into numbers. There is where tokenization comes into play. 

To use language model, we'll first tokenize the text.

Then we'll assign each token a unique integer. 

These integers are then vectorized and fed into the language model. 

The language model processes this vectorized input and outputs integers again

which are subsequently converted back into text.

<p align="center">
  <a href="./images/tokenization-pipeline.png">
    <img 
      src="./images/tokenization-pipeline.png" 
      width="400"
      alt="Architecture diagram"
    />
  </a>
  <p align="center">
    <em>Tokenization process in LLMs</em>
  </p>
</p>

Without tokenization, language models would not be able to operate on just raw textual data.