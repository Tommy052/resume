# 최재혁 | Frontend Developer

> 거북이처럼 차곡차곡, 꾸준히 성장하는 개발자입니다.

**Email:** eheh34w@naver.com
**GitHub:** [github.com/Tommy052](https://github.com/Tommy052)
**Blog:** [medium.com/@eheh34w](https://medium.com/@eheh34w)

---

## Summary

6년차 프론트엔드 개발자로 데이터 시각화와 웹 솔루션 개발을 전문으로 합니다.
D3.js, WebGL, WebGPU를 활용한 고성능 시각화 엔진 설계부터 GCP 인프라 운영까지, 제품의 전체 라이프사이클에 걸쳐 기여하고 있습니다.
현재 6명 규모의 개발팀을 리딩하며, 피파괴검사 AI 솔루션을 만들고 있습니다.

---

## Skills

**Core:** TypeScript, React, D3.js, WebGL, WebGPU
**Frontend:** Next.js, Vite, SVG Rendering, Canvas API
**Backend:** Node.js, NestJS, Django, FastAPI
**Infra:** AWS, GCP, Docker, Jenkins CI/CD, PostgreSQL
**Etc:** Electron, RabbitMQ, Prometheus/Grafana

---

## Experience

### 딥아이 — FE 개발팀장

`2023.11 ~ 현재`

피파괴검사(NDT) 분야의 AI 자동검사 솔루션을 개발하는 스타트업.
인공지능을 통해 검사 데이터의 이상 부위를 자동으로 탐지하고, 수동 검사도 지원하는 웹 기반 솔루션.

**역할:** 6명 개발팀 리딩 (Visualization, Product, Platform, ML 4개 파트)

#### 시각화 엔진 설계 및 구현

- Plotly.js의 커스터마이징 한계를 해결하기 위해 D3.js 기반 시각화 엔진을 직접 설계
- 초기 바닐라 JS → D3.js 계산 + React SVG 렌더링 구조로 단계적 리팩토링
- 대용량 검사 데이터(수만 포인트) 처리를 위해 WebGL/WebGPU 렌더링 파이프라인 도입
- 좌표계, 스케일, 줌/팬 인터랙션을 추상화한 차트 프레임워크 구축

#### TypeScript 마이그레이션 & 아키텍처 개선

- React.js(JS) 데모 버전을 TypeScript 프로젝트로 전면 리팩토링
- 모노레포 구조 설계 및 전환

#### 인프라 & DevOps

- GCP VM 기반 서비스 인프라 구축 (Bastion → Private 서버 구조)
- Jenkins CI/CD 파이프라인 구축 (개발 서버)
- AWS 파이프라인(React + FastAPI) 구축 (메인 서버)
- Prometheus + Grafana 모니터링 시스템 운영
- BigQuery + Cloud Logging 기반 로그 분석 체계 수립

#### Electron 데스크톱 앱

- 웹 FE + BE를 하나로 묶어 오프라인 Windows 데스크톱 앱으로 빌드
- 네트워크 없는 현장 환경에서도 검사 솔루션을 사용할 수 있도록 구현

#### 팀 리딩

- 4개 파트(Visualization, Product, Platform, ML) 업무 분배 및 코드 리뷰
- 2주 단위 스프린트 운영, 동시 다발적 멀티 프로젝트 관리

---

### 팀솔루션 — FE 개발자

`2022.05 ~ 2023.10`

공장 및 특정 장소에서 일어나는 일들을 3D로 시각화하는 디지털 트윈 솔루션 스타트업.

#### 3D 디지털 트윈 시각화

- WebGL 기반 3D 모델을 iframe으로 로드하고, 웹과 양방향 이벤트 통신 구현
- 실시간 데이터를 소켓 통신 및 Kafka로 연결하여 3D 화면에 반영
- 차트 및 알람 대시보드 구현, 사용자 커스텀 메뉴 구성 기능 개발

#### 인프라

- Azure Kubernetes 환경에서 서비스 배포 및 운영
- JWT 기반 인증 및 사용자별 권한 관리 구현

**기술:** Next.js, React, NestJS, PostgreSQL, Azure, WebGL, Kafka

---

### 트리피누 — 풀스택 개발자

`2020.09 ~ 2022.04`

여행 일정 추천 플랫폼. 사용자가 나라와 날짜를 입력하면 성격 유형에 맞는 여행 일정을 자동 추천.

#### 플랫폼 개발 (풀스택)

- Django REST Framework + React로 프론트엔드/백엔드 전체 개발
- OAuth 2.0 소셜 로그인(Google, Kakao) 구현
- Google Maps / React Leaflet 기반 지도 표시 및 장소 정보 연동
- 성격 유형별(MBTI 유사) 여행 일정 자동 생성 알고리즘 구현
- 관리자 / 여행사 / 일반사용자 3단계 권한별 페이지 및 기능 분리
- 자유여행 CRUD + 예약 기능 구현

#### 인프라

- AWS CI/CD 파이프라인 구축 및 운영

**기술:** Django, React, PostgreSQL, AWS, GCP, Google Maps API

---

### 아이엔지코리아 — SW 개발자

`2019.07 ~ 2020.07`

스마트 팩토리 솔루션 회사. 제조업 공장의 공정을 디지털로 전환하는 MES 시스템 개발.

#### 공정 관리 시스템 개발 (5개 고객사)

- 고객사별 맞춤 공정 시스템 설계 및 개발 (C#, WinForms)
- 입고 → 공정 → 출고 전체 프로세스의 CRUD 및 검색 기능 구현
- 현장직을 위한 키오스크 프로그램 개발
- 바코드 기반 완제품 관리 시스템 (Windows PDA, HTTP 통신)
- 블루투스 통신으로 측정 장비 데이터 자동 입력 기능 구현
- 출고 관리를 위한 Android 앱 개발 (Java, SQLite)
- 재고 현황 그래프 시각화 및 엑셀 다운로드 기능

**납품 고객사:** 금우수지, 청보산업, 남명, 정호산업, FQTC

**기술:** C#, WinForms, Java, Android, MySQL, GitLab, SVN

---

### 엔에스이 — IT 헬프데스크

`2018.06 ~ 2019.06`

원전 및 국방에 특화된 솔루션 회사. 실크로드 CMIS(형상관리 시스템) 부서.

- 형상관리 프로그램 유지보수 및 사용자 지원
- SQL DB 관리 및 쿼리 작성
- 버전 테스트, 배포 세팅 및 검증

**기술:** Java, MSSQL, SVN

---

## Education

- IOT 시스템 개발 전문가 과정 수료
