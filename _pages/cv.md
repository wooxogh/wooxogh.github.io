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
* **Co-founder / Backend & AI Engineer**, *EdgH* — *Sep 2025 ~ Present*
  * “누구나 주체적인 투자 결정을 할 수 있는 세상”을 목표로 하는 초기 창업팀 활동  
  * 경쟁 서비스 조사, 타깃 사용자 분석, 문제 정의 등 **초기 기획·시장 검증 중심 역할 수행**  
  * 향후 투자 정보 분석 플랫폼 백엔드 구축을 위한 기술 검토 진행 중

Projects & Research
======
* **2nd Yonsei GenAI Contest — “컴은영 (Computer Speaks English)”** (*Sep 2024 ~ Nov 2024*)
  * 양육자 일기를 입력받아 감정 분석·RAG 기반 피드백을 생성하는 AI 서비스 개발  
  * Node.js + Python 백엔드, MongoDB 데이터 파이프라인, Flutter 앱 개발 참여 

* **SKYST Hackathon — UniStage** (*May 2025*)  
  * 공연 예약·티켓팅 서비스 백엔드 개발 (Django REST)  
  * 좌석·예약 API의 동시성 처리 및 DB 쿼리 최적화  
  * Docker + EC2 배포 환경 구축  

* **IDEALAB — Local Business Analytics Platform** (*Jun 2025 ~ Sep 2025*)
  * 서울 상권 데이터 기반 창업자 분석지원 플랫폼  
  * Django + MySQL 백엔드 구축 및 데이터 파이프라인 구성  
  * OpenAI GPT 기반 시장 리포트 자동 생성 모듈 개발

* **2025 Sinchonthon — “남사칭”** (*Sep 2025*)  
  * 보이스피싱·사기 메시지 탐지 웹서비스 백엔드 개발  
  * Django + MySQL FULLTEXT 검색 기반 실시간 유사도 탐지  
  * 정규식 기반 위험 패턴 추출 및 재랭킹 로직 구성  

* **3rd Yonsei GenAI Contest — GIFPT (Gold Prize)** (*Sep 2025 ~ Dec 2025*)
  * 학술 논문 PDF를 GIF/MP4로 자동 시각화하는 생성형 AI 학습 플랫폼 개발  
  * Spring Boot(인증·파일관리) + Django/Celery(AI Worker) 멀티 서비스 아키텍처 설계  
  * Redis 기반 작업 큐·세션 관리, MySQL 기반 메타데이터 저장 구조 구현  
  * AWS EC2 + Docker Compose 기반 배포 인프라 구성  

* **SAI — Structured Q&A & Debate Platform** (*Aug 2025 ~ Dec 2025*)
  * 사용자 생성 Q&A·토론방의 대화를 구조적으로 저장·조회하는 웹 플랫폼 개발  
  * Spring Boot + MySQL 기반 백엔드 아키텍처 및 도메인 모델링  
  * JWT 인증·인가, Redis 세션 캐싱, GitHub Actions 기반 CI/CD 구축  
  * Docker + EC2을 통한 자동 배포 환경 구성 
  
Skills and Techniques
======
* **Languages**: Python, Java, C/C++
* **Backend / Frameworks**: Django, DRF, Spring Boot
* **AI / Data**: OpenAI API, RAG, Prompt Engineering, Celery
* **Databases**: MySQL, MongoDB, Redis
* **Cloud / DevOps**: Docker, AWS (EC2, S3, RDS), Nginx, GitHub Actions (CI/CD)
* **Web**:REST API design, JWT/OAuth
* **Other**: Notion/Slack integration, Testing & Documentation

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Service and leadership
======
* **Vice President**, Yonsei Univ. Dept. of Computer Science Student Council (*Dec 2023 ~ Dec 2024*)

  Managed ~30 staff; planned & executed events for ~600 students; budgeting, scheduling, faculty coordination.

* **Member**, Yonsei AWS Summer Camp (*Jul 2024 ~ Aug 2024*)

  AWS EC2, RDS, S3 기반 배포 및 OAuth 로그인·CI/CD 실습  

* **Backend Track**, 멋쟁이사자처럼 연세대학교 13기 (*Mar 2025 ~ Dec 2025*)

  Django 기반 팀 프로젝트 참여, REST API 설계·배포 경험  

* **(Incoming)President**, 멋쟁이사자처럼 연세대학교 14기 (*Jan 2026 ~ Dec 2026*)

Links
======
* **Portfolio**: <https://wooxogh.github.io/portfolio/>
* **GitHub**: <https://github.com/wooxogh>
