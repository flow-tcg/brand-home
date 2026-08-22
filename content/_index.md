---
title: "(주)플로우"
description: "다양한 형태의 서비스를 운영하는 회사입니다."
---

# (주)플로우

> 다양한 형태의 서비스를 운영하는 회사입니다. 웹 서비스, 모바일 앱, 백엔드 API까지 하나의 브랜드 아래에서 통합된 경험을 제공합니다.

## 서비스 현황

(주)플로우가 운영 중인 서비스입니다.

- [서비스 대시보드](/services-dashboard/) - 전체 서비스 위계와 현재 상태
- [소개](/about/) - 회사 정보 및 사업 영역

## 기술 스택

(주)플로우가 사용하는 기술입니다.

- **Hugo** - 정적 사이트 생성
- **Cloudflare Workers** - 서버리스 컴퓨팅
- **Apple Container** - 컨테이너 운영
- **Gradle** - Android 앱 빌드
- **Swift** - iOS 앱 개발
- **Spring Boot** - Java API 서버

## 시스템 구성

```
eflow-front  → Cloudflare Worker
eflow-Admin  → Cloudflare Container → Java 8 / Tomcat → 별도 MySQL
eflow-admin-cloudflare-api → Cloudflare에 별도 배포된 Admin API 서비스
Android      → Java API (Retrofit)
Cloudflare D1 → 신규 기능 및 테스트 데이터
```

## 주요 인물

- **한경수** - (주)플로우 대표이사 (flow001@eflow.co.kr)

## 문서

- [AGENTS.md](/AGENTS.md) - 프로젝트 지침
- [work-log.md](/work-log.md) - 작업 기록
- [GitHub](https://github.com/flow-tcg/brand-home) - 소스 코드
