# 최재혁 | Frontend Developer

**Email:** eheh34w@naver.com · **GitHub:** [Tommy052](https://github.com/Tommy052) · **Blog:** [Medium](https://medium.com/@eheh34w)

---

## Summary

대용량 데이터 시각화와 웹 기반 솔루션 개발에 강점을 가진 6년차 프론트엔드 개발자입니다.
기존 차트 라이브러리의 한계를 해결하기 위해 WebGL/WebGPU 기반 렌더링 엔진을 직접 설계·구축한 경험이 있으며, 현재 6명 개발팀을 리딩하며 제품의 FE 아키텍처와 인프라 전반을 책임지고 있습니다.

`TypeScript` `React` `D3.js` `WebGL` `WebGPU` `Babylon.js` `Electron`

---

## Experience

### 딥아이 — FE 개발팀장

`2023.11 ~ 현재` · 6명 팀 · 피파괴검사 AI 솔루션

#### GPU 기반 시각화 엔진 자체 개발

**문제:** 대규모 초음파 신호 데이터(수십만 포인트 × 멀티채널)에서 D3.js + SVG 렌더링이 버벅거렸고, Plotly.js는 커스텀 인터랙션과 자유로운 레이아웃 구성이 불가능했다.

**해결:**
- Plotly.js → D3.js 엔진 자체 설계 → WebGL GPU 렌더러 3개 패키지 직접 개발 (히트맵, 데이터 히트맵, 스트립/라인 차트)
- LOD 다운샘플링, 텍스처 타일 분할로 GPU 메모리 한계 극복
- 2D 맵의 3D 시각화를 위해 Babylon.js + WebGPU 기반 3D 뷰어 구축

**성과:**
- D3.js + SVG 대비 렌더링 성능 약 10배 향상, 수십만 포인트에서 60fps 유지
- 고정 3개 레이아웃 → 검사자가 자유롭게 차트를 선택·배치하는 구조로 전환
- 2D → 3D 맵 확장으로 검사 데이터의 입체적 분석 가능

#### 모노레포 전환 및 TypeScript 마이그레이션

**문제:** 4개 분산 레포에 중복 코드가 산재, 공통 UI 수정 시 레포마다 각각 수정·배포 필요. JS 기반으로 런타임 타입 에러 빈번.

**해결:**
- Turborepo + pnpm 모노레포로 통합 (apps 4개 + packages 9개)
- 공통 UI 패키지에 20+ 컴포넌트, 공통 유틸리티에 3D 로직·Worker 분리
- TypeScript strict 모드 전면 적용

**성과:**
- 공통 UI 변경 시 1회 수정으로 전체 앱 반영, 신규 화면 개발 속도 약 40% 단축
- 런타임 타입 에러 90% 이상 감소

#### 인프라 구축 및 DevOps

**문제:** 서버 인프라 부재, 수동 배포, 장애 인지는 고객 리포트에 의존.

**해결:**
- GCP VM Bastion → Private 서버 네트워크 아키텍처 설계
- Jenkins CI/CD, Prometheus + Grafana 모니터링, Sentry FE 에러 추적 구축

**성과:**
- 배포 시간 30분 → 5분, 장애 인지 수 시간 → 5분 내 감지

#### Electron 오프라인 데스크톱 앱

- 네트워크 없는 검사 현장을 위해 웹 FE + BE를 Electron으로 통합, 오프라인 Windows 앱으로 빌드
- 웹 코드 85% 재사용, 별도 네이티브 개발 없이 출시 → 오프라인 고객사 신규 확보

#### 팀 빌딩

- 4개 파트(Visualization, Product, Platform, ML) 구조 설계, 2주 스프린트 운영
- 코드 리뷰 문화 정착, 동시 3~4개 프로젝트 병렬 관리

---

### 팀솔루션 — FE 개발자

`2022.05 ~ 2023.10` · 디지털 트윈 3D 시각화 솔루션

#### 3D 디지털 트윈 대시보드 개발

**문제:** 공장 3D 모델과 웹 대시보드가 분리되어 운영자가 두 화면을 번갈아 확인해야 했다.

**해결:**
- WebGL 3D 모델 iframe 임베드 + postMessage 양방향 통신으로 단일 화면 통합
- 소켓 + Kafka로 실시간 센서 데이터를 3D 화면에 즉시 반영
- 드래그 기반 대시보드 위젯 커스터마이징 기능 개발

**성과:** 고객사 3곳 납품 완료, Azure Kubernetes 환경 안정 운영

**기술:** Next.js, React, NestJS, PostgreSQL, Azure, WebGL, Kafka

---

### 트리피누 — 풀스택 개발자

`2020.09 ~ 2022.04` · 여행 일정 추천 플랫폼

#### 1인 풀스택 MVP 개발 및 런칭

- Django REST Framework + React로 프론트/백엔드 단독 개발
- OAuth 2.0 소셜 로그인(Google, Kakao) 도입 → 회원가입 전환율 약 35% 향상
- Google Maps 연동 지도 기반 일정 시각화, 성격 유형별 자동 추천 알고리즘 구현
- AWS CI/CD 구축으로 무중단 배포 환경 확보

> 풀스택 경험을 통해 BE 개발자와의 API 설계 협업, DB 스키마 논의에서 원활한 커뮤니케이션이 가능합니다.

**기술:** Django, React, PostgreSQL, AWS, Google Maps API

---

### 아이엔지코리아 — SW 개발자

`2019.07 ~ 2020.07` · 스마트 팩토리 MES 시스템

#### 공정 모듈 재사용 구조 설계 및 5개 고객사 납품

- 입고 → 공정 → 출고 공통 프로세스를 모듈화, 고객사별 커스터마이징으로 전환
- 키오스크, 바코드(PDA), 블루투스 측정기 등 하드웨어 인터페이스 개발
- 고객사당 개발 기간 12주 → 6주로 50% 단축, 1년간 5개 고객사 전수 납품

> 제조 현장의 하드웨어 연동 경험이 현재 검사 장비 데이터를 다루는 도메인과 연결됩니다.

**기술:** C#, WinForms, Java, Android, MySQL

---

## Skills

| 분류 | 기술 |
|------|------|
| **Visualization** | D3.js, WebGL, WebGPU, Canvas API, SVG |
| **Frontend** | TypeScript, React, Next.js, Vite |
| **3D** | Babylon.js |
| **Backend** | Node.js, NestJS, Django, FastAPI |
| **Infra** | AWS, GCP, Docker, Jenkins, Prometheus/Grafana, Sentry |
| **Desktop** | Electron |
| **Database** | PostgreSQL, MySQL, BigQuery |

---

## Education

- IOT 시스템 개발 전문가 과정 수료
