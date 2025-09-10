---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! My name is Woo Taeho. I'm currently studying Computer Science at Yonsei University in Korea.  
My interests include systems programming, networking, and cloud infrastructure.  
I am passionate about learning new technologies and developing practical skills through projects and collaboration.

Experiences
------



### 남사칭 (백엔드 4인)
*2025.09*
💻 [Source Code](https://github.com/Sinchonthon-team7/Backend.git)
📄 [api 명세서](https://www.notion.so/API-26583f7524bc80518b47c39f2cec2e60)

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
`Python` `Django REST Framework` `MySQL` `pgvector` `OpenAI API`  
`Docker` `AWS S3` `EC2`  
`Regex` `Requests` `JWT`

Honors & Awards
------
ss

Extracurricular Activities
------
Sss
