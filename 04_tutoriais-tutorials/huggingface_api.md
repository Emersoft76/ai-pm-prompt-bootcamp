# 🤗 Tutorial: Usando Hugging Face Transformers

---

## 🇧🇷 Introdução

A Hugging Face fornece uma vasta biblioteca de modelos de linguagem prontos para uso. Aqui você aprenderá como carregar e usar um modelo localmente.

## 🇺🇸 Introduction

Hugging Face provides a rich library of ready-to-use language models. You'll learn how to load and run a model locally.

---

## 📦 Instalação

```bash
pip install transformers
```

---

## 🧪 Exemplo: Análise de sentimentos

```python
from transformers import pipeline

analisador = pipeline("sentiment-analysis")

resultado = analisador("Este bootcamp é incrível!")
print(resultado)
```

---

## 📌 Dicas

* Você pode usar modelos em português, como pierreguillou/bert-base-cased-sentiment
* Acesse huggingface.co/models

---
