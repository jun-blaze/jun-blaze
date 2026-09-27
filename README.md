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
| 2026.09.28 | [클링(Kling) 4.0 프리뷰 화면 유출…30초 생성·키프레임 10개, AI 영상 '감독 시대' 성큼](https://velog.io/@aiinsider1bd/%ED%81%B4%EB%A7%81Kling-4.0-%ED%94%84%EB%A6%AC%EB%B7%B0-%ED%99%94%EB%A9%B4-%EC%9C%A0%EC%B6%9C30%EC%B4%88-%EC%83%9D%EC%84%B1%ED%82%A4%ED%94%84%EB%A0%88%EC%9E%84-10%EA%B0%9C-AI-%EC%98%81%EC%83%81-%EA%B0%90%EB%8F%85-%EC%8B%9C%EB%8C%80-%EC%84%B1%ED%81%BC) | [@aiinsider1bd](https://velog.io/@aiinsider1bd) |
| 2026.09.28 | [동시성 vs 병행성](https://velog.io/@niki8533/%EB%8F%99%EC%8B%9C%EC%84%B1-vs-%EB%B3%91%ED%96%89%EC%84%B1) | [@niki8533](https://velog.io/@niki8533) |
| 2026.09.28 | [종합Project(ACE) - 발급부분 - 5 - 초기 convention세팅(git hook )](https://velog.io/@jungchoi1/%EC%A2%85%ED%95%A9ProjectACE-%EB%B0%9C%EA%B8%89%EB%B6%80%EB%B6%84-5-%EC%B4%88%EA%B8%B0-convention%EC%84%B8%ED%8C%85git-hook) | [@jungchoi1](https://velog.io/@jungchoi1) |
| 2026.09.28 | [[부트캠프 회고] TypeScript 고급 문법부터 React·Express 적용까지 한 흐름으로 이해하기](https://velog.io/@yangjoonwon/%EB%B6%80%ED%8A%B8%EC%BA%A0%ED%94%84-%ED%9A%8C%EA%B3%A0-TypeScript-%EA%B3%A0%EA%B8%89-%EB%AC%B8%EB%B2%95%EB%B6%80%ED%84%B0-ReactExpress-%EC%A0%81%EC%9A%A9%EA%B9%8C%EC%A7%80-%ED%95%9C-%ED%9D%90%EB%A6%84%EC%9C%BC%EB%A1%9C-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0) | [@yangjoonwon](https://velog.io/@yangjoonwon) |
| 2026.09.28 | [Samsung Cloud Platform[Terraform]: 실습 - Terraform 설치 + Provider 설정 + VPC 생성](https://velog.io/@moonabcd/Samsung-Cloud-PlatformTerraform-%EC%8B%A4%EC%8A%B5-Terraform-%EC%84%A4%EC%B9%98-Provider-%EC%84%A4%EC%A0%95-VPC-%EC%83%9D%EC%84%B1) | [@moonabcd](https://velog.io/@moonabcd) |
| 2026.09.28 | [Amazon SQS와 SNS 정리](https://velog.io/@jennie-infra/Amazon-SQS%EC%99%80-SNS-%EC%A0%95%EB%A6%AC) | [@jennie-infra](https://velog.io/@jennie-infra) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
