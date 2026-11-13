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
| 2026.11.14 | [가마가 멈추면 수업도 옮겨야 한다: 작은 도자기 공방의 수강생별 일정 변경 안내법](https://velog.io/@maildoer/%EA%B0%80%EB%A7%88%EA%B0%80-%EB%A9%88%EC%B6%94%EB%A9%B4-%EC%88%98%EC%97%85%EB%8F%84-%EC%98%AE%EA%B2%A8%EC%95%BC-%ED%95%9C%EB%8B%A4-%EC%9E%91%EC%9D%80-%EB%8F%84%EC%9E%90%EA%B8%B0-%EA%B3%B5%EB%B0%A9%EC%9D%98-%EC%88%98%EA%B0%95%EC%83%9D%EB%B3%84-%EC%9D%BC%EC%A0%95-%EB%B3%80%EA%B2%BD-%EC%95%88%EB%82%B4%EB%B2%95) | [@maildoer](https://velog.io/@maildoer) |
| 2026.11.14 | [고정 하단 탭바 하나 붙였더니 아이폰에서 세 번 다시 만졌습니다 — Tailwind safe-area와 입력창 16px](https://velog.io/@returncare/%EA%B3%A0%EC%A0%95-%ED%95%98%EB%8B%A8-%ED%83%AD%EB%B0%94-%ED%95%98%EB%82%98-%EB%B6%99%EC%98%80%EB%8D%94%EB%8B%88-%EC%95%84%EC%9D%B4%ED%8F%B0%EC%97%90%EC%84%9C-%EC%84%B8-%EB%B2%88-%EB%8B%A4%EC%8B%9C-%EB%A7%8C%EC%A1%8C%EC%8A%B5%EB%8B%88%EB%8B%A4-Tailwind-safe-area%EC%99%80-%EC%9E%85%EB%A0%A5%EC%B0%BD-16px) | [@returncare](https://velog.io/@returncare) |
| 2026.11.14 | [마이크로소프트 M365 20시간 넘는 장애…"레드먼드 의존"의 위험성 다시 부각](https://velog.io/@bbzjun/%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8-m365-20%EC%8B%9C%EA%B0%84-%EB%84%98%EB%8A%94-%EC%9E%A5%EC%95%A0%EB%A0%88%EB%93%9C%EB%A8%BC%EB%93%9C-%EC%9D%98%EC%A1%B4%EC%9D%98-%EC%9C%84%ED%97%98%EC%84%B1-%EB%8B%A4%EC%8B%9C-%EB%B6%80%EA%B0%81-2026-11-13) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.14 | [AI가 괴델의 암호 같은 노트를 열다…80년 만에 드러난 663개의 정리](https://velog.io/@bbzjun/ai%EA%B0%80-%EA%B4%B4%EB%8D%B8%EC%9D%98-%EC%95%94%ED%98%B8-%EA%B0%99%EC%9D%80-%EB%85%B8%ED%8A%B8%EB%A5%BC-%EC%97%B4%EB%8B%A480%EB%85%84-%EB%A7%8C%EC%97%90-%EB%93%9C%EB%9F%AC%EB%82%9C-663%EA%B0%9C%EC%9D%98-%EC%A0%95%EB%A6%AC-2026-11-13) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.10.15 | [AI Native FE 개발로의 전환, 150일간의 여정](https://velog.io/@teo/ai-native-fe) | [@teo](https://velog.io/@teo) |
| 2026.06.23 | [더이상 사람이 코딩하지 않는 시대, 개발자는 무엇을 해야 할까?](https://velog.io/@teo/ai-era-developer-role) | [@teo](https://velog.io/@teo) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
