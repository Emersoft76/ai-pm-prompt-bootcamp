# 🚀📦 Projeto 04: Pipeline de Deploy para Aplicações de IA

## 🇧🇷 Descrição

Aqui você criará um pipeline completo de deploy de uma aplicação de IA usando FastAPI, Streamlit e arquivos `.env` para proteger chaves de API.

## 🇺🇸 Description

In this project, you’ll build a full deployment pipeline for an AI application using FastAPI, Streamlit, and `.env` files to secure API keys.

---

## 🚀 Tecnologias / Technologies

- FastAPI
- Streamlit
- Python-dotenv
- OpenAI API
- Render / Railway (opcional para deploy)

---

## 📂 Arquivos

- `main_api.py`: Endpoint da IA com FastAPI
- `interface_streamlit.py`: Interface visual para usuário
- `.env.example`: Exemplo de variáveis de ambiente
- `README.md`: Instruções de deploy local e na nuvem

---

## 📌 Habilidades trabalhadas / Skills practiced

- Deploy local e remoto de soluções de IA
- Boas práticas de segurança com `.env`
- Integração back-end + front-end com IA
- Preparação de produto para ambiente real

---

## ▶️ Execução local

```bash
pip install fastapi uvicorn streamlit openai python-dotenv
uvicorn main_api:app --reload
streamlit run interface_streamlit.py
```

---
