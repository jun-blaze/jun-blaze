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
| 2026.10.27 | [[LG CNS AM - TIL 47일차] AM기반 MSA: Docker 컨테이너 관리, 포트 공개와 사용자 정의 네트워크 이해](https://velog.io/@lvmnt2/LG-CNS-AM-TIL-47%EC%9D%BC%EC%B0%A8-AM%EA%B8%B0%EB%B0%98-MSA-Docker-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88-%EA%B4%80%EB%A6%AC-%ED%8F%AC%ED%8A%B8-%EA%B3%B5%EA%B0%9C%EC%99%80-%EC%82%AC%EC%9A%A9%EC%9E%90-%EC%A0%95%EC%9D%98-%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%9D%B4%ED%95%B4) | [@lvmnt2](https://velog.io/@lvmnt2) |
| 2026.10.27 | [2026 triton, pytorch 컨퍼런스 후기](https://velog.io/@maxtnuk/2026-triton-pytorch-%EC%BB%A8%ED%8D%BC%EB%9F%B0%EC%8A%A4-%ED%9B%84%EA%B8%B0) | [@maxtnuk](https://velog.io/@maxtnuk) |
| 2026.10.27 | [[프로그래머스] 최고의 집합](https://velog.io/@j_keun/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%A8%B8%EC%8A%A4-%EC%B5%9C%EA%B3%A0%EC%9D%98-%EC%A7%91%ED%95%A9) | [@j_keun](https://velog.io/@j_keun) |
| 2026.10.27 | [구조적 사고는 하중이 어디로 가는가 — 아치 하나로 읽는 세 가지 길](https://velog.io/@linxiaohei/%EA%B5%AC%EC%A1%B0%EC%A0%81-%EC%82%AC%EA%B3%A0%EB%8A%94-%ED%95%98%EC%A4%91%EC%9D%B4-%EC%96%B4%EB%94%94%EB%A1%9C-%EA%B0%80%EB%8A%94%EA%B0%80-%EC%95%84%EC%B9%98-%ED%95%98%EB%82%98%EB%A1%9C-%EC%9D%BD%EB%8A%94-%EC%84%B8-%EA%B0%80%EC%A7%80-%EA%B8%B8-zpi2tf1v) | [@linxiaohei](https://velog.io/@linxiaohei) |
| 2026.10.27 | [버튼만 막으면 될까? 주소창으로 들어오는 사용자](https://velog.io/@ychany/%EB%B2%84%ED%8A%BC%EB%A7%8C-%EB%A7%89%EC%9C%BC%EB%A9%B4-%EB%90%A0%EA%B9%8C-%EC%A3%BC%EC%86%8C%EC%B0%BD%EC%9C%BC%EB%A1%9C-%EB%93%A4%EC%96%B4%EC%98%A4%EB%8A%94-%EC%82%AC%EC%9A%A9%EC%9E%90) | [@ychany](https://velog.io/@ychany) |
| 2026.10.27 | [Python Network Security Scanner DAY9](https://velog.io/@pingu_122/Python-Network-Security-Scanner-DAY9) | [@pingu_122](https://velog.io/@pingu_122) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
