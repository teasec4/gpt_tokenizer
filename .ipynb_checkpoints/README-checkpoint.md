# GPT Tokenizer

[![Python 3.14+](https://img.shields.io/badge/python-3.14%2B-blue)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A simple implementation of the Byte Pair Encoding (BPE) tokenization algorithm, exploring how text is converted into tokens for language models.

## What's in the badges

The badges at the top provide quick information about the project:
- **Python version requirement**: Indicates this notebook requires Python 3.14 or higher
- **License badge**: Shows the project is licensed under MIT

## How it works

This implementation demonstrates the tokenization pipeline:

1. **Text to bytes**: Convert UTF-8 text into raw byte sequences
2. **Byte pair analysis**: Identify the most frequently occurring consecutive byte pairs
3. **Merging**: Progressively merge the most frequent pairs into new tokens
4. **Encoding/Decoding**: Encode text into token sequences and decode them back

The algorithm compresses the token sequence by treating common patterns as single tokens, reducing the total number of tokens needed to represent the same text.

## Learning resource

This implementation is based on concepts introduced in Andrey Karpathy's excellent educational video on tokenization:
- **[Let's build the GPT Tokenizer](https://www.youtube.com/watch?v=zduSFxRajkE)** - A detailed walkthrough of how tokenization works in language models

## Example

The notebook demonstrates compression of Unicode text containing emojis and special characters, achieving a compression ratio of ~1.37x through 20 merge operations.

---

*Educational implementation for understanding LLM tokenization mechanisms*
