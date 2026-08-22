---
title: "(주)플로우"
description: "다양한 형태의 서비스를 운영하는 회사입니다."
---

# (주)플로우

다양한 형태의 서비스를 운영하는 회사입니다.

## 서비스

- [서비스 대시보드](/services-dashboard/) - 전체 서비스 위계와 현재 상태
- [소개](/about/) - 회사 정보 및 사업 영역

## 기술

- Hugo - 정적 사이트 생성
- Cloudflare Workers - 서버리스 컴퓨팅
- Apple Container - 컨테이너 운영
- Gradle - Android 앱 빌드
- Swift - iOS 앱 개발
- Spring Boot - Java API 서버

## 구성

```
eflow-front  → Cloudflare Worker
eflow-Admin  → Cloudflare Container → Java 8 / Tomcat → 별도 MySQL
eflow-admin-cloudflare-api → Cloudflare에 별도 배포된 Admin API 서비스
Android      → Java API (Retrofit)
Cloudflare D1 → 신규 기능 및 테스트 데이터
```

## 팀

- 한경수 - (주)플로우 대표이사

## 문서

- [AGENTS.md](/AGENTS.md)
- [work-log.md](/work-log.md)
- [GitHub](https://github.com/flow-tcg/brand-home)
