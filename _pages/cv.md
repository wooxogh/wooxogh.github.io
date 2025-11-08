---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in Computer Science, Yonsei University, Mar 2023 ~ Current

Work experience
======
* **Co-founder / Backend & AI Engineer**, *EdgH* — *Aug 2025 ~ Present*
  * Building a generative-AI platform that connects US tech stock creators and retail investors via real-time issue tracking and opinion aggregation.
  * Django REST + OpenAI GPT backend for news summarization and creator insight visualization; React dashboard for investor transparency.

* **Backend Developer**, *LikeLion Yonsei 13th* — *2025 ~ Present*
  * Team projects using Django/DRF; API design, authentication, deployment workflows.

Projects & Research (Selected)
======
* **2nd Yonsei GenAI Contest — “컴은영 (Computer Speaks English)”** (*Sep 2024 ~ Nov 2024*)
  * Generative-AI parenting support app using **RAG**, **sentiment analysis**, and **OpenAI API** to turn diary inputs into structured feedback & To-Do lists.
  * Node.js + Python backend, **MongoDB** data pipeline, **Flutter** cross-platform UI.

* **SKYST Hackathon — UniStage** (*May 2025*)
  * Performance-ticketing platform (Django REST); booking/ticketing APIs optimized for concurrency

* **IDEALAB — Local Business Analytics Platform** (*Jun 2025 ~ Sep 2025*)
  * Django + MySQL service analyzing Seoul commercial-district data for entrepreneurs.
  * **OpenAI GPT** generates natural-language market briefs (trends, competitive density, revenue potential).

* **Sinchonthon Hackathon — “남사칭”** (*Sep 2025*)
  * Real-time harmful-message detection (voice phishing, scams, cult recruitment).
  * Django REST + **MySQL FULLTEXT** retrieval; **OpenAI GPT** semantic re-ranking; regex phone extraction + spam API; Docker + AWS EC2.

* **3rd Yonsei GenAI Contest — GIFPT** (*Sep 2025 ~ Present*)
  * Generative-AI learning platform that converts academic PDFs into **GIF/MP4** visual explanations.
  * Spring Boot + MySQL (auth/files) + Django/Celery AI worker; Dockerized multi-service (Spring/Django/Redis/MySQL) on AWS EC2.

* **SAI — AI-Driven Cultural Debate & Discussion Platform** (*Aug 2025 ~ Present*)
  * Spring Boot + MySQL Q&A rooms with **AI conversation summaries**; **JWT + Redis** for secure, scalable sessions.
  
Skills and Techniques
======
* **Languages**: Python, Java, C/C++
* **Backend / Frameworks**: Django, DRF, Spring Boot
* **AI / Data**: OpenAI API, RAG, Prompt Engineering, Celery
* **Databases**: MySQL, MongoDB, Redis
* **Cloud / DevOps**: Docker, AWS (EC2, S3, RDS), Nginx, GitHub Actions (CI/CD)
* **Web**: React, REST API design, JWT/OAuth
* **Other**: Regex, Notion/Slack integration, Testing & Documentation

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* **Vice President**, Yonsei Univ. Dept. of Computer Science Student Council — *Dec 2023 ~ Dec 2024*  
  Managed ~30 staff; planned & executed events for ~600 students; budgeting, scheduling, faculty coordination.

Links
======
* **Portfolio**: <https://wooxogh.github.io/portfolio/>
* **GitHub**: <https://github.com/wooxogh>