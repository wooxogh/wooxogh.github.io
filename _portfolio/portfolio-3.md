---
title: "GIFPT"
excerpt: "Generative-AI 기반 학습 플랫폼<br/><img src='/images/gifpt.png' style='width:60%; height:auto;'>"
collection: portfolio
---

### 📌 GIFPT
*2025.08 ~ Present*

💻 [Source Code](https://github.com/YonseiGenAi/GIFPT-RELEASE.git)  
📑 [서비스 소개자료](/files/GIFPT.pdf)

**🔍 Overview**

강의·논문 PDF를 입력하면 내용을 자동으로 분석해 GIF/MP4 형태의 시각적 학습 애니메이션을 생성하는 플랫폼입니다.
단일 서버에서 모든 기능을 처리하는 구조의 한계를 피하기 위해, AI 연산과 사용자 트래픽을 분리한 멀티 서비스 아키텍처로 설계했습니다.
- 사용자 인증·파일 관리와
- AI 기반 비동기 연산 파이프라인을 명확히 분리하여
확장성과 장애 격리를 우선 고려했습니다.

**🏗 Architecture & Design Decisions**
- Spring Boot
    - 인증/인가, 유저 세션, 파일 도메인을 담당
    - 트랜잭션 관리와 타입 안정성이 중요한 영역에 적합하다고 판단
- Django REST + Celery (AI Worker)
    - LLM 호출, PDF 전처리, 영상 생성 등 CPU·IO 집약 작업을 비동기화
    - 요청-응답 서버와 분리하여 사용자 경험 저하 방지
- Celery + Redis
    - 작업 큐 기반 파이프라인으로
    - 작업 생성 → 상태 추적 → 결과 수집 흐름을 명확히 분리
- Docker Compose 기반 멀티 컨테이너 배포
    - 로컬/서버 환경 차이를 제거하고
    - 서비스 단위 확장 및 장애 대응을 용이하게 하기 위함

**My Contributions.**  
- Backend Core (Spring Boot)
    - JWT 기반 인증/인가 시스템 설계
    - Stateless 구조로 확장성과 배포 유연성 확보
- 유저 세션·파일 업로드 도메인 전체 설계
    - 인증 컨텍스트와 파일 접근 권한을 명확히 분리

- Asynchronous Pipeline
	- Celery 기반 비동기 처리 파이프라인 설계
	- 작업 큐 → 상태 폴링 → 결과 수집 구조 정의
	- 장시간 AI 연산으로 인한 요청 블로킹 문제 해결
	- Redis를 상태 저장소로 활용하여

- AI Worker 설계
	- Django REST 기반 AI Worker 서버 초기 구조 설계
	- LLM 호출 로직을 공통 Wrapper 템플릿으로 추상화
    → 모델 교체·프롬프트 변경 시 영향 최소화
	- PDF 페이지 단위 이미지 변환 파이프라인 구축
	- ghostscript 사용
	- 페이지 메타데이터를 DB에 구조화하여 저장

- Infra & DevOps
	- AWS EC2 + Docker Compose 기반 배포 환경 구성
	- GitHub Actions 기반 CI/CD 파이프라인 구축
	- 빌드 → 컨테이너 배포 자동화
	- 반복적인 수동 배포 제거 및 배포 안정성 확보

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
