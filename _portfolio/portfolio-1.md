---
title: "IDEALAB"
excerpt: "상권 데이터 분석 및 AI 기반 회의 요약 기능을 제공하는 창업 지원 웹서비스<br/><img src='/images/idealab.png' style='width:60%; height:auto;'>"
collection: portfolio
---

### 📌 IDEALAB (팀 프로젝트)
*2025.07 ~ 2025.09*

💻 [Source Code](https://github.com/Likelion-Yonsei-13th/13-HACKATHON-BACKEND-IDEALAB.git)
📄 [API 명세서](https://www.notion.so/API-25653ab3199c804697c5f1446819a901)
📑 [서비스 소개자료](/files/idealab.pdf)

**Description.**  
지역 상권 데이터를 기반으로 다양한 지표(매출, 폐업률, 상권 변화 등)를 수집·분석하고, 이를 활용해 창업자나 사용자에게 직관적인 상권 인사이트를 제공하는 웹 서비스입니다.
서울열린데이터(OpenAPI)와 자체 구축한 CSV 데이터셋을 RDS(MySQL)에 적재하고, Django 기반 백엔드에서 이를 API로 제공하여 프론트엔드와 연동했습니다.
또한 회의 음성 데이터를 요약하는 기능과, 사용자가 제공한 키워드를 기반으로 자동으로 관련 상권 데이터를 찾아 프론트엔드에 전달하는 로직도 구현했습니다.

**Features.**  
- Django REST Framework 기반 API 서버 설계 및 구현  
- AWS RDS(MySQL) + Docker 환경에서의 데이터 적재 및 관리  
- 상권 데이터(CSV) → DB 적재용 custom management commands 작성
- 서울열린데이터(OpenAPI) 및 상권 반경 API 연동 → 상권별 업소 수 자동 집계  
- ClosureStat, TradingArea 등 주요 모델의 데이터 백필(backfill) 로직 설계  
- 회의 음성 데이터 요약 기능 구현 (OpenAI API 활용)
- 키워드 기반 데이터 매핑 로직 작성 → 사용자가 요청한 키워드와 관련된 상권 데이터 자동 추출 및 API 응답
- Gunicorn + Nginx + Docker Compose 기반의 배포 환경 구성  
- Let’s Encrypt + Nginx Reverse Proxy를 통한 HTTPS 보안 통신 지원  

**Tech Stack.**  
`Python` `Django REST Framework` `MySQL (AWS RDS)`  
`Docker` `Nginx` `Gunicorn`
`AWS EC2` `AWS S3`  
`OpenAI API` `OpenAPI (서울 열린데이터)`  
`Requests` `Regex` `JWT`
