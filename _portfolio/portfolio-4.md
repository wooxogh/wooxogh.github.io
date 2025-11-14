---
title: "EdgH"
excerpt: "미국 주식 AI 기반 뉴스 요약 및 크리에이터 의견 집계 플랫폼 (진행 중)<br/><img src='/images/' style='width:60%; height:auto;'>"
collection: portfolio
---

### 📌 EdgH
*2025.08 ~ Present*

💻 [Source Code](https://github.com/EdgHgde/mail2notion_demo.git)  
📄 [API 명세서]()  
📑 [서비스 소개자료](/files/)

**Description.**  
미국 주식 관련 뉴스·리포트·크리에이터 콘텐츠를 자동으로 수집·요약해 투자자에게 정제된 인사이트를 제공하는 플랫폼입니다.  
핵심 구조는 Gmail → GPT → Notion 자동화 파이프라인으로, 실시간 뉴스 분석 및 콘텐츠 큐레이션을 위한 기반 엔진 역할을 합니다.

**Features.**  
- Gmail API OAuth 연동 → 뉴스/리포트 자동 수집  
- HTML/본문 정규화 파서 구축 → 다양한 뉴스 포맷 안정적 처리  
- 해시 기반 중복 제거 + 실패 fallback 처리 로직 구현  
- GPT 기반 뉴스 요약 파이프라인 개발  
- 요약 내용을 Notion DB에 자동 업데이트하는 통합 자동화  
- React 기반 간단한 대시보드 초기 버전 개발  
- 크리에이터별 키워드/의견 히스토리 매핑 로직 설계(초안)

**Tech Stack.**  
`Python` `Gmail API` `Notion API` `OpenAI API`  
`Regex` `Requests`  
`React` `AWS EC2`