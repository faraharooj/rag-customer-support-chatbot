# 🥐 RAG Customer Support Chatbot

A fully functional AI-powered customer support chatbot built with RAG (Retrieval Augmented Generation). Trained on business documents and answers customer questions instantly, 24/7.

**Live Demo:** [Zara's Bakery Chatbot](https://www.upwork.com/freelancers/~01aebffd4d10de4043?p=2041842717047816192)

---

## 🎯 What It Does

Businesses upload their documents (menu, FAQs, policies) and customers can ask any question and get accurate, instant answers — without any human involvement.

```
Business uploads documents (PDF, text)
            ↓
System chunks, embeds and stores in vector DB
            ↓
Customer asks a question on the website
            ↓
System finds most relevant document chunks
            ↓
GPT writes accurate answer from those chunks
            ↓
Customer gets instant, accurate reply 24/7
```

---

## ✨ Features

- ✅ **RAG Architecture** — answers only from real documents, no hallucination
- ✅ **Conversation Memory** — remembers full chat history per session
- ✅ **Any Business** — swap documents to deploy for any client
- ✅ **Beautiful UI** — professional chat widget embedded on website
- ✅ **Document Ingestion Pipeline** — upload PDF and it's ready instantly
- ✅ **Vector Search** — finds semantically relevant content, not just keywords
- ✅ **Deployed & Live** — hosted on Netlify, accessible worldwide

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **n8n** | Workflow automation & AI agent orchestration |
| **OpenAI GPT-4o-mini** | Language model for generating answers |
| **OpenAI text-embedding-3-small** | Converting text to vectors |
| **Supabase (pgvector)** | Vector database for document storage & search |
| **Supabase Postgres** | Conversation memory storage |
| **Netlify** | Website hosting |

---

## 🏗️ Architecture

### Workflow 1 — Document Ingestion
```
PDF Upload → Extract Text → Chunk Text → 
Embed with OpenAI → Store in Supabase Vector DB
```

### Workflow 2 — Live Chatbot
```
Customer Question → Embed Question → 
Search Supabase for Relevant Chunks → 
Send Chunks + Question to GPT → 
Return Accurate Answer
```

---


3. **Upload client documents** via the ingestion webhook

---

## 📁 Project Structure

```
├── Supabase_RAG_AI_Agent.json    # n8n workflow
└── README.md                     # You are here
```

---

## 💬 Example Questions & Answers

> **Q: What are your opening hours?**
> A: Zara's Bakery is open Monday to Saturday from 7 AM to 8 PM. We are closed on Sundays and all public holidays including Eid days.

> **Q: Do you offer delivery?**
> A: Yes! We offer home delivery within a 10km radius of our Gulberg location. Flat fee of Rs. 150 per order, minimum order Rs. 800. Delivery hours 10am–6pm, Monday to Saturday.

> **Q: What are your vegan options?**
> A: Our vegan options are the Sourdough Loaf, Focaccia, and Fresh Juice.

---

## 🔧 Requirements

- n8n instance (cloud or self-hosted)
- OpenAI API key
- Supabase project (free tier works)
- Netlify account (free tier works)

---

## 📦 Want This for Your Business?

This system can be deployed for any business in 48 hours.

**Contact:**  upwork : https://www.upwork.com/freelancers/~01aebffd4d10de4043?mp_source=share
gmail : ai.engrfaraharooj@gmail.com

---

