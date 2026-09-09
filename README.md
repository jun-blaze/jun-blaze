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
| 2026.09.09 | [아직 체커기는 올라오지 않았다](https://velog.io/@yunsungyang-omc/%ED%9A%8C%EA%B3%A0-%EC%95%84%EC%A7%81-%EC%B2%B4%EC%BB%A4%EA%B8%B0%EB%8A%94-%EC%98%AC%EB%9D%BC%EC%98%A4%EC%A7%80-%EC%95%8A%EC%95%98%EB%8B%A4) | [@yunsungyang-omc](https://velog.io/@yunsungyang-omc) |
| 2026.09.09 | [[TIL] PM 수업 17일차 \| 이론과 실전 사이의 온도 차: 첫 문제 정의 보고서 피드백 복기](https://velog.io/@so_so_hanna31/TIL-PM-%EC%88%98%EC%97%85-17%EC%9D%BC%EC%B0%A8-%EC%9D%B4%EB%A1%A0%EA%B3%BC-%EC%8B%A4%EC%A0%84-%EC%82%AC%EC%9D%B4%EC%9D%98-%EC%98%A8%EB%8F%84-%EC%B0%A8-%EC%B2%AB-%EB%AC%B8%EC%A0%9C-%EC%A0%95%EC%9D%98-%EB%B3%B4%EA%B3%A0%EC%84%9C-%ED%94%BC%EB%93%9C%EB%B0%B1-%EB%B3%B5%EA%B8%B0) | [@so_so_hanna31](https://velog.io/@so_so_hanna31) |
| 2026.09.09 | [[내일배움캠프] 협업을 위한 git 활용 TIL](https://velog.io/@kim_da/%EB%82%B4%EC%9D%BC%EB%B0%B0%EC%9B%80%EC%BA%A0%ED%94%84-%ED%98%91%EC%97%85%EC%9D%84-%EC%9C%84%ED%95%9C-git-%ED%99%9C%EC%9A%A9-TIL) | [@kim_da](https://velog.io/@kim_da) |
| 2026.09.09 | [[Unity] 팀 - 전략 패턴 타워 공격 & 보스 던지기 #14](https://velog.io/@rkdalsrn1028/Unity-%EC%A0%84%EB%9E%B5-%ED%8C%A8%ED%84%B4-%ED%83%80%EC%9B%8C-%EA%B3%B5%EA%B2%A9-%EB%B3%B4%EC%8A%A4-%EB%8D%98%EC%A7%80%EA%B8%B0-14) | [@rkdalsrn1028](https://velog.io/@rkdalsrn1028) |
| 2026.09.09 | [홈 서버에 개인비서 만들기 2편 - OpenClaw에 두 번째 직원 `박실장` 채용하기](https://velog.io/@na_treeeum/%ED%99%88-%EC%84%9C%EB%B2%84%EC%97%90-%EA%B0%9C%EC%9D%B8%EB%B9%84%EC%84%9C-%EB%A7%8C%EB%93%A4%EA%B8%B0-2%ED%8E%B8-OpenClaw%EC%97%90-%EB%91%90-%EB%B2%88%EC%A7%B8-%EC%A7%81%EC%9B%90-%EB%B0%95%EC%8B%A4%EC%9E%A5-%EC%B1%84%EC%9A%A9%ED%95%98%EA%B8%B0) | [@na_treeeum](https://velog.io/@na_treeeum) |
| 2026.09.09 | [CSAPP_1장](https://velog.io/@pinn99u/CSAPP1%EC%9E%A5) | [@pinn99u](https://velog.io/@pinn99u) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
