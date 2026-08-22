---
title: "(주)플로우 서비스 현황"
description: "(주)플로우의 전체 서비스 위계와 현재 상태를 한눈에 확인할 수 있는 대시보드입니다."
date: 2026-08-22
layout: "services-dashboard"
type: "page"
---

# (주)플로우 서비스 현황

(주)플로우는 다수의 서비스를 운영하고 있습니다. 이 페이지는 모든 서비스의 위계 구조와 현재 상태를 한눈에 보여줍니다.

## 서비스 위계 구조

```
(주)플로우

├── 웹 서비스
│   ├── 공식 홈페이지 (Hugo) - /
│   └── 운영 시스템 (Cloudflare Workers) - https://flow.tcgc.uk
│
├── 모바일 서비스
│   ├── Android 앱 (Gradle) - 개발 중
│   ├── iOS 앱 (Swift) - 개발 중
│   └── Flow 앱 Android (Gradle) - 개발 중
│
└── 백엔드/API
    ├── Java API (Spring Boot) - 후보 검토 중
    ├── 관리자 화면 (Java) - 후보 검토 중
    └── 프론트엔드 (Cloudflare Worker) - 운영 중
```

## 현재 서비스 상태

### 웹 서비스

| 서비스 | URL | 상태 | 유형 | 설명 |
|--------|-----|------|------|------|
| 공식 홈페이지 | / | ✅ 운영 중 | Hugo | (주)플로우 공식 사이트 |
| 운영 시스템 | https://flow.tcgc.uk | ⚠️ DNS 설정 필요 | Cloudflare Workers | 회사 운영 관리 시스템 |

### 모바일 서비스

| 서비스 | URL | 상태 | 유형 | 설명 |
|--------|-----|------|------|------|
| Android 앱 | - | 📋 개발 중 | Gradle | 안드로이드 앱 서비스 |
| iOS 앱 | - | 📋 개발 중 | Swift | iOS 앱 서비스 |
| Flow 앱 Android | - | 📋 개발 중 | Gradle | Flow 앱 안드로이드 버전 |

### 백엔드/API

| 서비스 | URL | 상태 | 유형 | 설명 |
|--------|-----|------|------|------|
| Java API | - | 🔍 후보 검토 중 | Spring Boot | REST API 서버 |
| 관리자 화면 | - | 🔍 후보 검토 중 | Java | 관리자 대시보드 |
| 프론트엔드 | - | ✅ 운영 중 | Cloudflare Worker | 프론트엔드 서비스 |

## 서비스 통계

| 구분 | 운영 중 | 개발 중 | 검토 중 | 합계 |
|------|---------|---------|---------|------|
| 웹 서비스 | 1 | 0 | 0 | 1 |
| 모바일 서비스 | 0 | 3 | 0 | 3 |
| 백엔드/API | 1 | 0 | 2 | 3 |
| **합계** | **2** | **3** | **2** | **7** |

## 기술 스택 분포

| 기술 | 서비스 수 | 비율 |
|------|----------|------|
| Hugo | 1 | 14% |
| Cloudflare Workers | 2 | 29% |
| Gradle | 2 | 29% |
| Swift | 1 | 14% |
| Spring Boot | 1 | 14% |

## 시스템 구성

```
eflow-front  → Cloudflare Worker
eflow-Admin  → Cloudflare Container → Java 8 / Tomcat → 별도 MySQL
eflow-admin-cloudflare-api → Cloudflare에 별도 배포된 Admin API 서비스
Android      → Java API (Retrofit)
Cloudflare D1 → 신규 기능 및 테스트 데이터
```

## 주요 인물

| 이름 | 역할 | 이메일 | 상태 |
|------|------|--------|------|
| 한경수 | (주)플로우 대표이사 | flow001@eflow.co.kr | 기존 투자자, 지속 투자 |

## 참고 문서

- [AGENTS.md](../AGENTS.md): 프로젝트 지침
- [work-log.md](../work-log.md): 작업 기록

---

*최종 업데이트: 2026-08-22*
