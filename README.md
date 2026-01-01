# 🏢 Autonomous Building Operations Agent

An autonomous AI-driven system that ingests live building sensor data, detects abnormal energy usage patterns, and automatically executes operational decisions such as HVAC schedule optimization and maintenance task creation.

This project demonstrates how applied AI can be embedded into real-world operational workflows, focusing on reliability, decision-making, and system integration rather than standalone model experimentation.

---

## 📚 Table of Contents
<details>
<summary>Click to expand</summary>

- [Overview](#toc-overview)
- [Key Capabilities](#toc-key-capabilities)
- [System Architecture](#toc-system-architecture)
- [Technology Stack](#toc-technology-stack)
- [Design Principles](#toc-design-principles)
- [Example Workflow](#toc-example-workflow)
- [Evaluation & Validation](#toc-evaluation-validation)
- [Local Development](#toc-local-development)
- [Extensibility](#toc-extensibility)
- [Why This Project Matters](#toc-why-this-project-matters)
- [Contact](#toc-contact)

</details>

---

## 🧠 Overview

Modern buildings generate large volumes of sensor data, but acting on this data in a timely and reliable way remains a challenge. This project implements an autonomous agent that continuously monitors sensor streams, identifies energy anomalies, and takes corrective actions without human intervention.

The system is designed as a modular, production-oriented AI service that integrates data ingestion, pattern detection, decision logic, and backend execution into a single end-to-end pipeline.

---

## ⚙️ Key Capabilities

- 📡 Real-time ingestion of building sensor data (energy usage, temperature, etc.)
- 🔍 Detection of abnormal energy consumption patterns
- 🌡️ Autonomous HVAC schedule optimization
- 🛠️ Automatic maintenance task generation on anomaly detection
- 🧾 Traceable and auditable AI-driven decisions
- 🔗 API-first design for easy system integration

---

## 🏗️ System Architecture

The system is structured as loosely coupled components to ensure scalability and maintainability:

1. **Ingestion Layer**  
   Receives live sensor events via API or message queue and persists raw data.

2. **Processing & Aggregation Layer**  
   Aggregates sensor readings over time windows for evaluation.

3. **Decision Engine**  
   Applies deterministic rules and thresholds to detect anomalies.

4. **Action Layer**  
   Executes operational actions:
   - HVAC schedule adjustments  
   - Maintenance task creation

5. **Backend Integration Layer**  
   Exposes actions and decisions to external systems (e.g., CMMS).

---

## 🧰 Technology Stack

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white" />
</p>

- **Language:** Python  
- **API Framework:** FastAPI  
- **Database:** PostgreSQL  
- **Streaming / Messaging:** Kafka  
- **Containerization:** Docker  

The stack was intentionally chosen to reflect production-ready technologies commonly used in AI-enabled backend systems.

---

## 🧩 Design Principles

- **Autonomy:** Decisions are triggered without manual intervention  
- **Reliability:** Clear, deterministic decision logic  
- **Traceability:** All actions can be logged and audited  
- **Modularity:** Components are independently replaceable  
- **Production Readiness:** Designed for deployment and monitoring  

---

## 🔄 Example Workflow

1. A sensor event with high energy usage is ingested.
2. Recent readings are aggregated for the affected building.
3. Thresholds are evaluated by the decision engine.
4. If an anomaly is detected:
   - HVAC schedules are optimized
   - A maintenance task is generated
5. Actions are exposed via backend APIs.

---

## 📊 Evaluation & Validation

The system can be evaluated by replaying historical sensor data and analyzing:

- Anomaly detection frequency
- False positives vs. missed anomalies
- Operational impact of automated actions

This approach prioritizes **decision reliability and system behavior**, not just offline model metrics.

---

## 🧪 Local Development

The project runs locally using Docker:

```bash
docker-compose up --build
```

---

## 📬 Contact

Feel free to reach out or explore more of my work:

- 📧 **Email:** [ma.shamshiri@gmail.com](mailto:ma.shamshiri@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/ma-shamshiri](https://www.linkedin.com/in/ma-shamshiri)
- 🧑‍💻 **GitHub:** [github.com/ma-shamshiri](https://github.com/ma-shamshiri)

