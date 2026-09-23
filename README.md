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

2022년에 공동 개발자와 시작후 일시중단된 프로젝트를 다시 만든 것입니다. 당시 핵심 기능이었던
백테스트는 DART가 일별 주가를 제공하지 않아 구현 자체가 불가능한 설계였고, 중단한 이유였습니다. 남은 코드에서 의도를 역추적한 기록은
[V1 회고](https://github.com/wnstjqaodls/side-market-data-platform/blob/main/docs/V1-RETROSPECTIVE.md)에
정리했습니다.

`Kotlin 2.0` · `Spring Boot 3.3` · `Vue 3` · `PostgreSQL 16` · `Flyway` · 단일 jar + systemd + nginx

---

## velog 최신 개발 글

<!-- VELOG:START -->
| 날짜 | 글 | 글쓴이 |
|---|---|---|
| 2026.09.23 | [오픈소스와 프론티어 AI가 개척하는 에이전틱 코딩의 미래](https://velog.io/@sdm77/%EB%AA%A8%EB%8D%B8%EC%97%85%EA%B3%84-%EB%8F%99%ED%96%A5-2026-09-23) | [@sdm77](https://velog.io/@sdm77) |
| 2026.09.23 | [LLM의 리스크 관리와 백테스팅 능력이 가르는 예측 시장 트레이딩 성패](https://velog.io/@sdm77/%EC%97%90%EC%9D%B4%EC%A0%84%ED%8A%B8%EC%9B%8C%ED%81%AC%ED%94%8C%EB%A1%9C-%EC%84%A4%EA%B3%84-2026-09-23) | [@sdm77](https://velog.io/@sdm77) |
| 2026.09.23 | [(BDAI 12기 SQL 입문반_1) 데이터 로딩 절차, ERD 해석방법, EDA (CTE, SELECT절, WHERE절 서브쿼리, CASE WHEN, 윈도우 순위함수 활용)](https://velog.io/@chaehwanjung/BDAI-12%EA%B8%B0-SQL-%EC%9E%85%EB%AC%B8%EB%B0%981-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EB%A1%9C%EB%94%A9-%EC%A0%88%EC%B0%A8-ERD-%ED%95%B4%EC%84%9D%EB%B0%A9%EB%B2%95-EDA-CTE-SELECT%EC%A0%88-WHERE%EC%A0%88-%EC%84%9C%EB%B8%8C%EC%BF%BC%EB%A6%AC-CASE-WHEN-%EC%9C%88%EB%8F%84%EC%9A%B0-%EC%88%9C%EC%9C%84%ED%95%A8%EC%88%98-%ED%99%9C%EC%9A%A9) | [@chaehwanjung](https://velog.io/@chaehwanjung) |
| 2026.09.23 | [JP 런칭 회고](https://velog.io/@sonomoo/JP-%E3%84%B9%E3%85%93%E3%84%B4%E3%85%8A%E3%85%A3%E3%85%87-%E3%85%8E%E3%85%97%E3%85%A3%E3%84%B1%E3%85%97) | [@sonomoo](https://velog.io/@sonomoo) |
| 2026.09.23 | [감정평가법인 전산담당자가 AI로 IT 인프라를 혁신하기 프로젝트에 들어서다](https://velog.io/@jelmano/%EA%B0%90%EC%A0%95%ED%8F%89%EA%B0%80%EB%B2%95%EC%9D%B8-%EC%A0%84%EC%82%B0%EB%8B%B4%EB%8B%B9%EC%9E%90%EA%B0%80-AI%EB%A1%9C-IT-%EC%9D%B8%ED%94%84%EB%9D%BC%EB%A5%BC-%ED%98%81%EC%8B%A0%ED%95%98%EA%B8%B0-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%EC%97%90-%EB%93%A4%EC%96%B4%EC%84%9C%EB%8B%A4) | [@jelmano](https://velog.io/@jelmano) |
| 2026.09.23 | [(Spring Boot) JwtToken을 이용하여 로그인, 로그아웃 구현하기](https://velog.io/@hellocode54/Spring-Boot-JwtToken%EC%9D%84-%EC%9D%B4%EC%9A%A9%ED%95%98%EC%97%AC-%EB%A1%9C%EA%B7%B8%EC%9D%B8-%EB%A1%9C%EA%B7%B8%EC%95%84%EC%9B%83-%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0) | [@hellocode54](https://velog.io/@hellocode54) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
