<div align="center">

# Tezash Mishra

**IT Student · Full-Stack Engineer · Builder** Building EchoSort!!

Learning to code, analyze data, and build real things, one project at a time.


</div>

---

## About Me

First-year Information Technology student exploring full-stack engineering, machine learning pipelines, and real-time systems. Not an expert, just curious, consistent, and building things that solve real problems.

I document my journey through projects here on GitHub and share the behind-the-scenes on Instagram.

---

## Tech Stack

**Languages**

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

**Backend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Convex](https://img.shields.io/badge/Convex-FFDA44?style=for-the-badge&logo=convex&logoColor=black)

**Databases & Infrastructure**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**ML & Data**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

**DevOps & Deployment**

![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

---

## Featured Projects

### EchoSort
https://github.com/mishradwaterlaw/echosort
> Event photo sharing with facial recognition. Upload a selfie, get back every photo of you from the entire event gallery.

A full-stack application built from scratch across five deployment platforms. Attendees visit a shared event link, take a selfie, and the system uses ArcFace face embeddings and pgvector cosine similarity search to find every matching photo in the event gallery.

**What makes it non-trivial**

- Decoupled ML pipeline: photo uploads are queued via Redis, processed asynchronously by a TensorFlow worker, and stored as 512-dimensional vectors in a pgvector HNSW index
- Secure by design: private storage buckets, time-limited signed URLs, Row Level Security on every table, and JWT verification using getUser() not getSession()
- Server Actions pattern: credentials never touch the browser bundle
- Real per-file upload progress via XHR (Fetch API does not expose upload progress)

**Stack**: Next.js 14 · FastAPI · DeepFace/ArcFace · Supabase (PostgreSQL + pgvector + Auth + Storage) · Upstash Redis · Modal.com · Vercel · Render

---

### Titanic Dataset Exploration

[github.com/mishradwaterlaw/titanicdatasetfirst-application](https://github.com/mishradwaterlaw/titanicdatasetfirst-application)

> Data exploration and analysis using Pandas and Matplotlib. Currently extending this toward a full predictive ML model.

**Stack**: Python · Pandas · NumPy · Matplotlib

---

## Currently Learning

- **Vector databases and semantic search**: pgvector, embedding models, approximate nearest neighbor indexing
- **ML deployment**: Serverless GPU workers, model serving, pipeline optimization
- **DSA in C++**: Strengthening problem-solving foundations for technical interviews
- **Open Source contribution**: Learning by reading and improving production codebases

---

<div align="center">

Everything here is a work in progress, just like me.

PS: I post behind-the-scenes on Instagram before things make it to GitHub. Progress is real, perfectionism is the delay.

</div>
