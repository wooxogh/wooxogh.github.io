---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

안녕하세요, 연세대학교 컴퓨터과학과에 재학 중인 우태호입니다.
저는 백엔드 개발에 깊은 관심을 가지고 있으며, 데이터베이스·API 설계·클라우드 인프라와 같은 영역을 탐구하고 있습니다. 개발을 할 때는 명확한 구조와 일관된 코드 스타일을 지향하며, 협업 시 다른 개발자가 이해하기 쉬운 코드를 작성하려 노력합니다. 또한 테스트와 문서화를 통해 유지보수가 용이한 코드를 만드는 것을 중요하게 생각합니다. 새로운 기술을 배우는 데 적극적이며, 실제 프로젝트와 협업 경험을 통해 실무적인 역량을 키워가고 있습니다.

Experiences
------
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

### 📌 남사칭 (Sinchonthon)
*2025.09*

💻 [Source Code](https://github.com/Sinchonthon-team7/Backend.git)
📄 [API 명세서](https://www.notion.so/API-26583f7524bc80518b47c39f2cec2e60)
📑 [서비스 소개자료](/files/남사칭.pdf)

**Description.**  
실시간으로 입력된 텍스트와 DB에 축적된 사례들을 비교하여 유사도를 분석하고, 보이스피싱·사기·종교 포섭·마약 권유 등 위험 사례를 자동 탐지하는 웹서비스입니다.
LLM을 활용해 검색된 사례를 재랭킹하고, 전화번호 패턴 추출 + 외부 스팸 API를 연동해 위험도를 종합 평가합니다.  

**Features.**  
- Django REST Framework 기반의 REST API 서버 구현
- MySQL FULLTEXT INDEX (MATCH ... AGAINST)를 활용한 후보 사례 검색 및 최신순 fallback 로직
- 검색된 사례를 카드 형태로 축약(PII 마스킹 포함) 후 LLM Prompting을 통한 재랭킹 및 요약
- 본문 내 전화번호를 정규식으로 자동 추출하고 외부 스팸번호 API와 연동
- 텍스트 유사도 + 전화번호 위험도를 조합한 종합 위험 점수 산출 로직 설계
- Docker 기반 컨테이너화 및 AWS 배포 환경 구성

**Tech Stack.**  
`Python` `Django REST Framework` `MySQL` `OpenAI API`  
`Docker` `AWS S3` `EC2`  
`Regex` `Requests` `JWT`

Honors & Awards 
------
**Academic Scholarship**  
  Yonsei University, 2nd Semester of 2023 (Feb 2024)  
  성적 우수 장학금 수여

Extracurricular Activities
------
### 연세대학교 컴퓨터과학과 학생회 — 부학생회장 (2024)
- 학과 학생회 부학생회장으로서 약 600명 규모의 학과 학생들을 대상으로 한 주요 행사(OT, MT, 축제 부스 등) 기획 및 운영 총괄
- 약 20명 규모의 집행부를 관리하며 회의 주재, 예산 및 일정 관리 수행
- 학생, 교수, 교직원 등 다양한 이해관계자와의 조율을 통해 원활한 의사소통 능력과 문제 해결 능력을 배양
