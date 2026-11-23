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
| 2026.11.23 | [웹개발기초 261123](https://velog.io/@fakeberry2021/%EC%9B%B9%EA%B0%9C%EB%B0%9C%EA%B8%B0%EC%B4%88-261123) | [@fakeberry2021](https://velog.io/@fakeberry2021) |
| 2026.11.23 | [[AI 강사 세리쌤 · 서순례] 검색창 대신 AI 비서에게 전화와 메일을 맡긴 월요일 — 혼자 다 하던 1인 강사의 일하는 법이 달라졌다](https://velog.io/@seriyo/AI-%EA%B0%95%EC%82%AC-%EC%84%B8%EB%A6%AC%EC%8C%A4-%EC%84%9C%EC%88%9C%EB%A1%80-%EA%B2%80%EC%83%89%EC%B0%BD-%EB%8C%80%EC%8B%A0-AI-%EB%B9%84%EC%84%9C%EC%97%90%EA%B2%8C-%EC%A0%84%ED%99%94%EC%99%80-%EB%A9%94%EC%9D%BC%EC%9D%84-%EB%A7%A1%EA%B8%B4-%EC%9B%94%EC%9A%94%EC%9D%BC-%ED%98%BC%EC%9E%90-%EB%8B%A4-%ED%95%98%EB%8D%98-1%EC%9D%B8-%EA%B0%95%EC%82%AC%EC%9D%98-%EC%9D%BC%ED%95%98%EB%8A%94-%EB%B2%95%EC%9D%B4-%EB%8B%AC%EB%9D%BC%EC%A1%8C%EB%8B%A4) | [@seriyo](https://velog.io/@seriyo) |
| 2026.11.23 | [AWS 프리티어로 LLM 게이트웨이 인프라 설계하기: EKS·NAT·ALB를 뺀 이유](https://velog.io/@jongwan_lim/llm-tollgate-00-infra-design) | [@jongwan_lim](https://velog.io/@jongwan_lim) |
| 2026.11.23 | [[Building WayCue #2] 길찾기보다 중요한 것은 선택해야 하는 순간이었다](https://velog.io/@ms_moon/Building-WayCue-2-%EA%B8%B8%EC%B0%BE%EA%B8%B0%EB%B3%B4%EB%8B%A4-%EC%A4%91%EC%9A%94%ED%95%9C-%EA%B2%83%EC%9D%80-%EC%84%A0%ED%83%9D%ED%95%B4%EC%95%BC-%ED%95%98%EB%8A%94-%EC%88%9C%EA%B0%84%EC%9D%B4%EC%97%88%EB%8B%A4) | [@ms_moon](https://velog.io/@ms_moon) |
| 2026.11.23 | [[Making Mutation Arcade #59] Pause와 Save는 마지막에 붙이는 기능이 아니었다](https://velog.io/@ms_moon/Making-Mutation-Arcade-59-Pause%EC%99%80-Save%EB%8A%94-%EB%A7%88%EC%A7%80%EB%A7%89%EC%97%90-%EB%B6%99%EC%9D%B4%EB%8A%94-%EA%B8%B0%EB%8A%A5%EC%9D%B4-%EC%95%84%EB%8B%88%EC%97%88%EB%8B%A4) | [@ms_moon](https://velog.io/@ms_moon) |
| 2026.11.23 | [13년차 보험 설계사가 퇴근 후 만든 여행 일정 검토 서비스 — LLM은 읽고, 판정은 코드가 합니다](https://velog.io/@tojkr/13%EB%85%84%EC%B0%A8-%EB%B3%B4%ED%97%98-%EC%84%A4%EA%B3%84%EC%82%AC%EA%B0%80-%ED%87%B4%EA%B7%BC-%ED%9B%84-%EB%A7%8C%EB%93%A0-%EC%97%AC%ED%96%89-%EC%9D%BC%EC%A0%95-%EA%B2%80%ED%86%A0-%EC%84%9C%EB%B9%84%EC%8A%A4-LLM%EC%9D%80-%EC%9D%BD%EA%B3%A0-%ED%8C%90%EC%A0%95%EC%9D%80-%EC%BD%94%EB%93%9C%EA%B0%80-%ED%95%A9%EB%8B%88%EB%8B%A4) | [@tojkr](https://velog.io/@tojkr) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
