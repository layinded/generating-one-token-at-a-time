# Generating One Token at a Time

This notebook explores how Large Language Models (LLMs) generate text — **one token at a time** — using probability distributions and subword tokenization.

🧠 **Concepts Covered**
- Subword tokenization
- Predictive token generation
- Using pretrained models with Hugging Face Transformers
- Visualizing logits and token probabilities

---

## 🔍 Key Questions

### Q1: What is subword tokenization?

Subword tokenization is a method that splits words into smaller, more frequent units (e.g., "unbreakable" → "un", "break", "able"). It reduces the size of the model's vocabulary while allowing it to understand rare or out-of-vocabulary words.

### Q2: Code Snippet Matching

| Code Snippet | Action |
|--------------|--------|
| `tokenizer` | Tokenize a piece of text |
| `AutoTokenizer.from_pretrained()` | Load a tokenizer |
| `AutoModelForCausalLM.from_pretrained()` | Load a pretrained model |
| `torch.nn.functional.softmax()` | Convert logits into probabilities |

---

## 🛠 Tools & Libraries

- Hugging Face Transformers
- PyTorch
- Tokenizer APIs
- Softmax & Logits

---

## 📁 Included

- `Exercise2-generating-one-token-at-a-time.ipynb` (main notebook)
- Reflections in `notes/reflection.txt`

---

## 💬 My Reflection

> “This was the first time I fully understood how an LLM doesn’t just *write*, it predicts — token by token, using math, probability, and context. Subword tokenization blew my mind a bit. You don’t need to know every word if you can build them.”

---

## 🔗 Learn More

Udacity Generative AI Nanodegree  
📚 [https://learn.udacity.com/nanodegrees/nd608-bmann-nextgen-challenge/](https://learn.udacity.com/nanodegrees/nd608-bmann-nextgen-challenge/)
