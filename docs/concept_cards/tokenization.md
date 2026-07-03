# Tokenization

## Definition

Tokenization is the process of breaking a sentence into smaller units called tokens.

---

## Why is it Needed?

Computers cannot understand complete sentences directly.

They first split the sentence into individual words.

---

## Example

Sentence

I love NLP.

Tokens

I

love

NLP

---

## Advantages

- Easy preprocessing
- Faster text analysis
- Used in almost every NLP task

---

## Limitations

- Cannot understand context
- Language dependent

---

## Applications

- Chatbots
- Search Engines
- Text Classification

---

## Python Example

```python
from nltk.tokenize import word_tokenize

text="I love NLP"

print(word_tokenize(text))
```

Output

```
['I','love','NLP']
```