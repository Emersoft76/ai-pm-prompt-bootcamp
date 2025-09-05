# 🧠🔌 Tutorial: Usando a OpenAI API | Using the OpenAI API

---

## 🇧🇷 Introdução

A API da OpenAI permite integrar modelos como GPT-4 diretamente em suas aplicações. Aqui, você aprenderá como criar e testar requisições simples com Python.

## 🇺🇸 Introduction

The OpenAI API allows you to integrate models like GPT-4 directly into your applications. Here you'll learn how to create and test basic requests using Python.

---

## ✅ Pré-requisitos | Requirements

- Conta na OpenAI: https://platform.openai.com
- Chave de API (copie do painel)
- Python 3.10+ instalado

---

## 📦 Instalação | Install

```bash
pip install openai
```

---

## 🧪 Exemplo básico | Basic example

```python
import openai
import os

openai.api_key = os.getenv("OPENAI_API_KEY")

response = openai.ChatCompletion.create(
    model="gpt-3.5-turbo",
    messages=[
        {"role": "system", "content": "Você é um assistente útil."},
        {"role": "user", "content": "Explique IA em uma frase simples."}
    ]
)

print(response['choices'][0]['message']['content'])
```

---

## 📁 Boas práticas | Best Practices

* Use .env para armazenar sua chave com segurança
* Teste diferentes temperaturas para controlar criatividade
* Limite tokens para reduzir custos

---
