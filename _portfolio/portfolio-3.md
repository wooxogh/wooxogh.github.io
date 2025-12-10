---
title: "GIFPT"
excerpt: "Generative-AI 기반 학습 플랫폼<br/><img src='/images/gifpt.png' style='width:60%; height:auto;'>"
collection: portfolio
---

### 📌 GIFPT
*2025.08 ~ Present*

💻 [Source Code](https://github.com/YonseiGenAi/GIFPT-RELEASE.git)
📑 [서비스 소개자료](/files/GIFPT.pdf)

**Description.** 
강의·논문 PDF를 입력하면, 내용을 자동 분석하여 GIF/MP4 형태의 시각적 애니메이션을 생성해주는 학습 플랫폼입니다.
아키텍처는 Spring Boot(인증·파일 관리) + Django REST(AI Worker API) + Celery(비동기 작업 큐) + Redis + MySQL로 구성된 멀티 서비스 구조로 설계했습니다.

**My Contributions.**  
- Spring Boot 인증/인가(JWT), 유저 세션, 파일 업로드 도메인 전체 설계
- Celery 기반 비동기 파이프라인 설계(작업 큐 → 상태 폴링 → 결과 수집) 및 Redis 연동
- AI Worker 서버(Django REST) 초기 구조 설계 및 LLM 호출 래퍼 템플릿 제작
- PDF 페이지 이미지 변환(ghostscript) + 메타데이터 저장 프로세스 개발
- AWS EC2 + Docker Compose 기반 멀티 컨테이너 배포 환경 구성
- GitHub Actions를 이용한 CI/CD 자동화 파이프라인 구축

**Features.**  
- Spring Boot 기반 유저 인증(JWT)·세션·프로필 관리
- PDF 업로드 및 파일 메타데이터 관리 (MySQL)
- Django 기반 AI Worker 서버 초기 구축
- Celery + Redis 기반 비동기 작업 처리 구조 설계 및 테스트 완료
- PDF를 단위 페이지 이미지로 변환하는 프리프로세싱 모듈 구축
- AI·LLM 호출을 위한 Python 기반 API Wrapper 템플릿 작성
- AWS EC2 + Docker Compose 기반 베이스 인프라 구성

**Tech Stack.** 
`Spring Boot` `Django` `REST` `Celery` `Redis`
`MySQL` `AWS` `EC2` `Docker`
`OpenAI` `JWT`
`Github Actions (CI/CD)`
