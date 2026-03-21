<div align="center">

# Amro Alhazouri

**Informatik-Student · TU Darmstadt · Cloud & DevOps · AI Engineering**

[![Email](https://img.shields.io/badge/amerhazzouri%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:amerhazzouri@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/amro-alhazouri)
[![Location](https://img.shields.io/badge/Viernheim%2C%20Germany-555?style=flat&logo=googlemaps&logoColor=white)](#)

</div>

---

Informatik-Student im 5. Semester an der TU Darmstadt mit praktischer Erfahrung in Cloud Engineering, DevOps und AI Engineering. Ich habe eigenständig produktionsreife Systeme aufgebaut — von Infrastructure as Code und automatisierten CI/CD-Pipelines bis hin zu einem Agentic RAG System für Enterprise-Support-Automatisierung. Ich suche einen Werkstudenten- oder Praktikumsplatz im Bereich Cloud / DevOps / Backend / AI.

---

## Projekte

### Enterprise AI Support Copilot — Agentic RAG System
> Full-Stack · FastAPI · ChromaDB · Google Gemini · React/TypeScript

[![Repo](https://img.shields.io/badge/GitHub-AI--Internal__Assistant-181717?style=flat&logo=github)](https://github.com/amer1211/AI-Internal_Assistant)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=google&logoColor=white)

Automatisiert die Erstellung von Support-Antworten: Ein Support-Agent fügt ein Ticket ein — das System durchsucht selbstständig die Wissensdatenbank, ruft die relevantesten Policy-Abschnitte per Cosine-Similarity-Suche ab und lässt Gemini eine fundierte, halluzinationsfreie Antwort generieren.

- **Data Pipeline** — `ingest.py` lädt PDFs, splittet in semantische Chunks (1000 Zeichen, 200 Overlap), generiert Gemini Embeddings, persistiert in ChromaDB
- **Backend** — saubere FastAPI-Architektur: Router → Service → RAG Core → Vector Store; typisierte Pydantic-Schemas, vollständige HTTP-Fehlerbehandlung
- **RAG Loop** — Ticket wird eingebettet, Top-4 Policy-Chunks per Cosine Similarity abgerufen, in strukturierten Prompt injiziert, Gemini 2.5 Flash generiert die Antwort
- **Frontend** — Zwei-Panel Enterprise-Dashboard in React/TypeScript: Skeleton Loader, Relevanz-Score-Badge pro Chunk, Zeichenzähler, ARIA-Attribute

```
Ticket  →  Gemini Embedding  →  ChromaDB Similarity Search
                                        ↓
                              Top-4 Policy Chunks
                                        ↓
                              RAG Prompt + Gemini LLM
                                        ↓
                              Grounded Draft + Quellangaben
```

---

### Cloud Homelab — DevOps Portfolio
> Infrastructure as Code · CI/CD · Container · Monitoring

[![Repo](https://img.shields.io/badge/GitHub-terraform--homelab-181717?style=flat&logo=github)](https://github.com/amer1211/terraform-homelab)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=github-actions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)

- **Terraform** — Server, Firewall, SSH-Keys und Remote State auf Hetzner Cloud als Code definiert
- **GitHub Actions** — pytest → Docker Multi-Stage Build (900 MB → 120 MB) → GHCR → SSH-Deploy mit Health-Check
- **FastAPI** — containerisierte API mit Swagger-Doku, Request-Tracking-Middleware und Git-SHA-Traceability
- **Prometheus + Grafana** — Docker Compose Stack mit Node Exporter, Live-Dashboards für CPU, RAM, Request-Rate

---

### Web-based Chess Application
> Full-Stack · Spring Boot REST Backend · Vanilla JS Frontend

[![Repo](https://img.shields.io/badge/GitHub-Web--based--Chess-181717?style=flat&logo=github)](https://github.com/amer1211/Web-based-Chess)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

- Vollständige Schachregeln: legale Zugberechnung, Zugverwaltung, Bauernumwandlung
- RESTful API-Endpunkte: start, legal moves, execute move
- Saubere Trennung zwischen Domain-Modellen, Services und Controllern

---

### PlantCellCounter — TU Darmstadt
> Semesterprojekt · Desktop-App · Cellpose Deep Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)

- Cellpose Deep Learning Inference für präzise Zellsegmentierung in Pflanzenbildern
- OpenCV-Integration als Bildlader und GUI-Backend

---

## Tech Stack

| Bereich | Technologien |
|---|---|
| **Cloud & DevOps** | Terraform · Docker · Docker Compose · GitHub Actions · Prometheus · Grafana · Linux · Hetzner Cloud |
| **AI & ML** | LangChain · ChromaDB · Google Gemini · RAG · Cellpose · OpenCV · Embeddings |
| **Backend** | FastAPI · Spring Boot · REST API · Pydantic · Uvicorn |
| **Frontend** | React · TypeScript · Vite · HTML/CSS/JS |
| **Programmierung** | Python · Java · C++ · JavaScript/TypeScript · ARM Assembler |
| **Methoden** | Agile/Scrum · IaC · CI/CD · OOP · UX/UI mit Figma |

---



<div align="center">

*Offen für Werkstudenten- und Praktikumsangebote im Bereich Cloud · DevOps · Backend · AI Engineering*

</div>
