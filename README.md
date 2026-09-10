# 김준섭

백엔드와 인프라를 함께 다룹니다. 직접 만든 서비스를 [qwer4.org](https://qwer4.org)에 올려
운영하고, 배포와 모니터링까지 붙여 끝까지 굴러가게 만드는 쪽에 관심이 있습니다.

---

## 기술 스택

**Backend**

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Ktor](https://img.shields.io/badge/Ktor-087CFA?style=flat-square&logo=ktor&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)

**Frontend**

![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square&logo=vuedotjs&logoColor=black)

**Data**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

**Infra / Ops**

![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=flat-square&logo=nginx&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 공개 포털 — [qwer4.org](https://qwer4.org)

직접 만든 서비스를 하나의 도메인 아래에 모아 운영합니다. 전부 지금 접속되는 주소입니다.

| 서비스 | 주소 | 스택 |
|---|---|---|
| **포털** | [qwer4.org](https://qwer4.org) | Vue 3, TypeScript, Tailwind, Vite |
| **블로그** | [blog.qwer4.org](https://blog.qwer4.org) | Quartz |
| **앨범** | [album.qwer4.org](https://album.qwer4.org) | Kotlin, Ktor, SQLite |
| **쇼핑·결제** | [shop.qwer4.org](https://shop.qwer4.org) | Java 21, Spring Boot 3.3, Spring Security, JPA, PostgreSQL |
| **공공주택 알리미** | [housing.qwer4.org](https://housing.qwer4.org) | Kotlin, Spring Boot, WebFlux, 코루틴 |
| **MKDP** | [mkdp.qwer4.org](https://mkdp.qwer4.org) | Kotlin, Spring Boot, Vue 3, PostgreSQL |

서비스마다 같은 순서를 따릅니다 — 컨테이너 생성 → nginx → Cloudflare Tunnel → 헬스체크
→ 관리 대시보드 등록 → 모니터링 편입. 외부에는 Cloudflare Tunnel로만 열고, 관리자 경로는
Cloudflare Access와 OAuth 뒤에 둡니다.

---

## 공개 저장소

### [side-market-data-platform](https://github.com/wnstjqaodls/side-market-data-platform) — MKDP

DART 공시·재무를 조회하고, 주식과 ETF로 포트폴리오 백테스트를 돌리는 서비스입니다.

2022년에 다른 개발자와 시작했다가 멈춘 프로젝트를 다시 만든 것입니다. 당시 핵심 기능이었던
백테스트는 DART가 일별 주가를 제공하지 않아 구현 자체가 불가능한 설계였고, 그게 프로젝트가
멈춘 진짜 이유였습니다. 남은 코드에서 의도를 역추적한 기록은
[V1 회고](https://github.com/wnstjqaodls/side-market-data-platform/blob/main/docs/V1-RETROSPECTIVE.md)에
정리했습니다.

`Kotlin 2.0` · `Spring Boot 3.3` · `Vue 3` · `PostgreSQL 16` · `Flyway` · 단일 jar + systemd + nginx

---

## velog 최신 개발 글

<!-- VELOG:START -->
| 날짜 | 글 | 글쓴이 |
|---|---|---|
| 2026.09.11 | ["use client" 많이 쓰면 진짜로 안 좋은걸까?](https://velog.io/@sunoly/use-client-%EB%A7%8E%EC%9D%B4-%EC%93%B0%EB%A9%B4-%EC%A7%84%EC%A7%9C%EB%A1%9C-%EC%95%88-%EC%A2%8B%EC%9D%80%EA%B1%B8%EA%B9%8C) | [@sunoly](https://velog.io/@sunoly) |
| 2026.09.11 | [AIO 프리코스 2일차 학습회고 ㅣ Python ch.4 (반복문 · 리스트 · 딕셔너리)](https://velog.io/@pdistudy_02/AIO-%ED%94%84%EB%A6%AC%EC%BD%94%EC%8A%A4-%ED%95%99%EC%8A%B5-2%EC%9D%BC%EC%B0%A8-%ED%9A%8C%EA%B3%A0-Python-ch.4-%EB%B0%98%EB%B3%B5%EB%AC%B8-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EB%94%95%EC%85%94%EB%84%88%EB%A6%AC) | [@pdistudy_02](https://velog.io/@pdistudy_02) |
| 2026.09.11 | [FD(File Descriptor)란?](https://velog.io/@eunduk/FDFile-Descriptor%EB%9E%80) | [@eunduk](https://velog.io/@eunduk) |
| 2026.09.11 | [c# 베이직 2일차](https://velog.io/@mustbehumble/c-%EB%B2%A0%EC%9D%B4%EC%A7%81-2%EC%9D%BC%EC%B0%A8) | [@mustbehumble](https://velog.io/@mustbehumble) |
| 2026.09.11 | [RAG 기반 학습 지원 프론트엔드 #2 — 화면 흐름 설계와 Expo Router 파일 구조 구성](https://velog.io/@jin0503/RAG-%EA%B8%B0%EB%B0%98-%ED%95%99%EC%8A%B5-%EC%A7%80%EC%9B%90-%ED%94%84%EB%A1%A0%ED%8A%B8%EC%97%94%EB%93%9C-2-%ED%99%94%EB%A9%B4-%ED%9D%90%EB%A6%84-%EC%84%A4%EA%B3%84%EC%99%80-Expo-Router-%ED%8C%8C%EC%9D%BC-%EA%B5%AC%EC%A1%B0-%EA%B5%AC%EC%84%B1) | [@jin0503](https://velog.io/@jin0503) |
| 2026.09.11 | [[CS] "Every CS Major Should Know" 릴스 속 CS 질문 5가지 풀이](https://velog.io/@asb041022/CS-Every-CS-Major-Should-Know-%EB%A6%B4%EC%8A%A4-%EC%86%8D-CS-%EC%A7%88%EB%AC%B8-5%EA%B0%80%EC%A7%80-%ED%92%80%EC%9D%B4) | [@asb041022](https://velog.io/@asb041022) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
