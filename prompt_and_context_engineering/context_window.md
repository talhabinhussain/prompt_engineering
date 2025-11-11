# Context Window and associated keywords are covered in this repository.

## Learning Material

1. **Context window**
2. **Context window is measured**
3. **What is a “token**”
4. **How do LLMs process tokens within a context window**
5. **How can long context windows negatively affect model performance?**

## Context window

A context window represents the “working memory” of an LLM. It determines how much information from a conversation or input the model can retain and use to generate subsequent responses. If a conversation exceeds the context window’s capacity, the model begins to “forget” earlier parts of the exchange, potentially leading to less coherent or accurate outputs.

## Context window is measured

Context window size is measured in tokens A token is the smallest unit of language processed by an LLM. It can represent a character, part of a word, a whole word, or even a short multi-word phrase. The way a piece of text is broken into tokens depends on the tokenizer used by a specific LLM. A general rule of thumb is that a regular English word equates to roughly 1.5 tokens.

## What is a “token

A token is the basic building block of language for AI models. Unlike humans who process language at the character level, LLMs break down text into tokens. These tokens can represent various elements, such as single characters, parts of words, entire words, or even short phrases. For example, in the sentence “Martin drove a car,” the word “a” is represented by a single token, whereas in “Martin is amoral,” “amoral” would be represented by two tokens: one for “a” and another for “moral.”

## How do LLMs process tokens within a context window

Transformer models use a mechanism called self-attention to process tokens in a context window. Self-attention calculates the relationships and dependencies between different tokens, even those far apart in the input sequence. This allows the model to understand how words at the beginning of a paragraph relate to those at the end. The self-attention mechanism computes weights, indicating the relevance of each token to the others. The size of the context window determines the maximum number of tokens the model can consider at any one time.

## How can long context windows negatively affect model performance?

While longer context windows enable models to process more information, they can also negatively affect performance. LLMs, like humans, can be overwhelmed by an abundance of detail and may take cognitive shortcuts. Studies have shown that models perform best when relevant information is at the beginning or end of the input context, and performance degrades when the model must carefully consider information in the middle of a long context.
