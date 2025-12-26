---
title: "남사칭"
excerpt: "실시간 텍스트 유사도 분석과 AI 기반 위험 탐지를 지원하는 보이스피싱·사기 예방 웹서비스<br/><img src='/images/남사칭.png' style='width:60%; height:auto;'>"
collection: portfolio
---

### 📌 남사칭 (Sinchonthon)
*2025.09*

💻 [Source Code](https://github.com/Sinchonthon-team7/Backend.git)
📄 [API 명세서](https://www.notion.so/API-26583f7524bc80518b47c39f2cec2e60)
📑 [서비스 소개자료](/files/남사칭.pdf)

**🔍 Overview**

실시간으로 입력되는 메시지를 기존 사례 데이터와 비교해 보이스피싱·사기·종교 포섭·마약 권유 등 위험 유형을 즉시 탐지하는 웹서비스입니다. 짧은 해커톤 환경에서 응답 속도와 탐지 신뢰도의 균형을 핵심 목표로 삼았습니다.

**🏗 Architecture**

- Django REST Framework 기반의 단일 API 서버 구조로 설계
- 실시간 응답이 중요한 서비스 특성을 고려해 요청–응답 경로를 단순화하고 동기 처리 위주로 구성
- 텍스트 검색(DB FULLTEXT) → LLM 재랭킹 → 위험 점수 산출을 하나의 요청 흐름으로 묶어 지연 시간을 최소화
- Docker 기반 컨테이너화 및 AWS EC2 단일 인스턴스 배포로 빠른 개발·배포 사이클에 집중

**🙋 My Contributions.**

- Django REST Framework 기반 REST API 서버 구현
- MySQL FULLTEXT INDEX 기반 후보 사례 검색 및 fallback 로직
- PII 마스킹된 카드 형태의 사례 요약 UI를 위한 응답 구조 설계
- LLM Prompting 기반 재랭킹 및 요약 파이프라인
- Docker 기반 컨테이너화 및 AWS EC2 배포

**🔑 Key Design Decisions**

- 왜 FULLTEXT INDEX를 선택했는가
    - 실시간 입력 텍스트에 대해 빠른 후보 검색이 필요했고,
    - 벡터 임베딩 기반 검색은 구축/튜닝 비용 대비 해커톤 환경에 과하다고 판단
    - MySQL FULLTEXT INDEX + 최신순 fallback으로
    
    → 응답 속도와 구현 안정성을 우선 확보
    
- 왜 LLM을 검색이 아니라 재랭킹에만 사용했는가
    - LLM 단독 판단은 비용·지연 시간 리스크가 큼
    - DB 검색으로 후보를 제한한 뒤, LLM은 문맥 이해가 필요한 순위 조정과 요약에만 사용
    
    → 응답 시간과 비용을 제어하면서도 탐지 품질 확보
    
- 왜 전화번호를 별도 신호로 분리했는가
    - 텍스트 유사도만으로는 위험도를 설명하기 부족
    - 정규식 기반 전화번호 추출 후 외부 스팸 API와 연동해
    
    → 텍스트 신호 + 번호 신호를 결합한 위험 점수 산출 구조 설계

**Tech Stack.**  
`Python` `Django REST Framework` `MySQL` `OpenAI API`  
`Docker` `AWS S3` `EC2`  
`Regex` `Requests` `JWT`
