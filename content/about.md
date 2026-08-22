---
title: "(주)플로우 소개"
description: "(주)플로우는 다양한 형태의 서비스를 운영하는 회사입니다."
date: 2026-08-22
layout: "about"
type: "page"
---

# (주)플로우 소개

(주)플로우는 다양한 형태의 서비스를 운영하는 회사입니다.

## 회사 개요

- **회사명**: (주)플로우
- **대표이사**: 한경수
- **이메일**: flow001@eflow.co.kr
- **설립일**: 확인 필요
- **위치**: 확인 필요

## 사업 영역

(주)플로우는 다음과 같은 사업 영역을 운영합니다:

### 웹 서비스
- 공식 홈페이지 (Hugo)
- 운영 시스템 (Cloudflare Workers)

### 모바일 서비스
- Android 앱 (Gradle)
- iOS 앱 (Swift)
- Flow 앱 Android (Gradle)

### 백엔드/API
- Java API (Spring Boot)
- 관리자 화면 (Java)
- 프론트엔드 (Cloudflare Worker)

## 시스템 구성

```
eflow-front  → Cloudflare Worker
eflow-Admin  → Cloudflare Container → Java 8 / Tomcat → 별도 MySQL
eflow-admin-cloudflare-api → Cloudflare에 별도 배포된 Admin API 서비스
Android      → Java API (Retrofit)
Cloudflare D1 → 신규 기능 및 테스트 데이터
```

## 비전

(주)플로우는 다양한 형태의 서비스를 통해 사용자에게 가치를 제공하고, 기술 혁신을 추구합니다.

## 연락처

- **이메일**: flow001@eflow.co.kr
- **웹사이트**: /

---

*최종 업데이트: 2026-08-22*
