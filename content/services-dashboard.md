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
│   ├── 공식 홈페이지 (Hugo) - https://flow-brand.tcgc.uk
│   └── 운영 시스템 (Cloudflare Workers) - https://flow.tcgc.uk
│
├── 모바일 서비스
│   ├── Android 앱 (Gradle) - 개발 중
│   ├── iOS 앱 (Swift) - 개발 중
│   └── Flow 앱 Android (Gradle) - 개발 중
│
└── 백엔드/API
    ├── Java API (Spring Boot) - 후보 검토 중
    ├── 관리자 화면 (eflow) - https://eflow.tcgc.uk
    ├── D1 DB (`eflow-admin-test-db-new`) - Cloudflare에서 작동 중
    └── 프론트엔드 (Cloudflare Worker) - 운영 중
```

## 현재 서비스 상태

### 웹 서비스

| 서비스 | URL | 상태 | 유형 | 설명 |
|--------|-----|------|------|------|
| 공식 홈페이지 | <a href="https://flow-brand.tcgc.uk" target="_blank" rel="noopener noreferrer">flow-brand.tcgc.uk</a> | ✅ 운영 중 | Hugo | (주)플로우 공식 사이트 |
| 운영 시스템 | <a href="https://flow.tcgc.uk" target="_blank" rel="noopener noreferrer">flow.tcgc.uk</a> | ⚠️ DNS 설정 필요 | Cloudflare Workers | 회사 운영 관리 시스템 |

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
| 관리자 화면 | <a href="https://eflow.tcgc.uk/" target="_blank" rel="noopener noreferrer">eflow.tcgc.uk</a> | ✅ 운영 중 | 별도 배포 | 관리자 대시보드 |
| D1 DB (`eflow-admin-test-db-new`) | <a href="https://dash.cloudflare.com/cedaf3a433ede6c25afb1bfad0943a4f/workers/d1/databases/8ed8bf5c-3ef7-4134-911d-d1c459ec8450/metrics" target="_blank" rel="noopener noreferrer">Cloudflare D1 Metrics</a> | ✅ Cloudflare에서 작동 중 | Cloudflare D1 | eflow 관리자용 데이터베이스 |
| 프론트엔드 | - | ✅ 운영 중 | Cloudflare Worker | 프론트엔드 서비스 |

## 서비스 통계

| 구분 | 운영 중 | 개발 중 | 검토 중 | 합계 |
|------|---------|---------|---------|------|
| 웹 서비스 | 1 | 0 | 0 | 1 |
| 모바일 서비스 | 0 | 3 | 0 | 3 |
| 백엔드/API | 2 | 0 | 1 | 3 |
| **합계** | **3** | **3** | **1** | **7** |

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
eflow-Admin  → 별도 관리 화면 → Java 8 / Tomcat → 별도 DB
eflow-admin-cloudflare-api → Cloudflare에 별도 배포된 Admin API 서비스
Android      → Java API (Retrofit)
D1 DB        → eflow 관리자 화면과 분리 운영되는 데이터 저장소
```

## 주요 인물

| 이름 | 역할 | 이메일 | 상태 |
|------|------|--------|------|
| 한경수 | (주)플로우 대표이사 | flow001@eflow.co.kr | 대표 |

## 참고 문서

- [AGENTS.md](../AGENTS.md): 프로젝트 지침
- [work-log.md](../work-log.md): 작업 기록

---

*최종 업데이트: 2026-08-22*
