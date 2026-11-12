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
| 2026.11.13 | [[바이브 코딩] 글을 10편 썼는데 검색 유입이 0이라, robots.txt와 sitemap.xml을 직접 열어봤습니다](https://velog.io/@returncare/%EB%B0%94%EC%9D%B4%EB%B8%8C-%EC%BD%94%EB%94%A9-%EA%B8%80%EC%9D%84-10%ED%8E%B8-%EC%8D%BC%EB%8A%94%EB%8D%B0-%EA%B2%80%EC%83%89-%EC%9C%A0%EC%9E%85%EC%9D%B4-0%EC%9D%B4%EB%9D%BC-robots.txt%EC%99%80-sitemap.xml%EC%9D%84-%EC%A7%81%EC%A0%91-%EC%97%B4%EC%96%B4%EB%B4%A4%EC%8A%B5%EB%8B%88%EB%8B%A4) | [@returncare](https://velog.io/@returncare) |
| 2026.11.13 | ["AI 데이터센터 전기요금, 결국 저소득·농촌 가구가 더 낸다"…코넬대 연구가 밝힌 불균형](https://velog.io/@bbzjun/ai-%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%84%BC%ED%84%B0-%EC%A0%84%EA%B8%B0%EC%9A%94%EA%B8%88-%EA%B2%B0%EA%B5%AD-%EC%A0%80%EC%86%8C%EB%93%9D%EB%86%8D%EC%B4%8C-%EA%B0%80%EA%B5%AC%EA%B0%80-%EB%8D%94-%EB%82%B8%EB%8B%A4%EC%BD%94%EB%84%AC%EB%8C%80-%EC%97%B0%EA%B5%AC%EA%B0%80-%EB%B0%9D%ED%9E%8C-%EB%B6%88%EA%B7%A0%ED%98%95-2026-11-12) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.13 | [앤스로픽, 나스닥 'ANT'로 IPO 로드쇼 돌입…주당 70~78달러, 최대 1조 달러대 몸값 저울질](https://velog.io/@bbzjun/%EC%95%A4%EC%8A%A4%EB%A1%9C%ED%94%BD-%EB%82%98%EC%8A%A4%EB%8B%A5-ant%EB%A1%9C-ipo-%EB%A1%9C%EB%93%9C%EC%87%BC-%EB%8F%8C%EC%9E%85%EC%A3%BC%EB%8B%B9-7078%EB%8B%AC%EB%9F%AC-%EC%B5%9C%EB%8C%80-1%EC%A1%B0-%EB%8B%AC%EB%9F%AC%EB%8C%80-%EB%AA%B8%EA%B0%92-%EC%A0%80%EC%9A%B8%EC%A7%88-2026-11-12) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.13 | [엔비디아 CEO 젠슨 황, 불륜·중국 스파이 스캔들 속 전격 사임…CFO 콜렛 크레스가 임시 지휘](https://velog.io/@bbzjun/%EC%97%94%EB%B9%84%EB%94%94%EC%95%84-ceo-%EC%A0%A0%EC%8A%A8-%ED%99%A9-%EB%B6%88%EB%A5%9C%EC%A4%91%EA%B5%AD-%EC%8A%A4%ED%8C%8C%EC%9D%B4-%EC%8A%A4%EC%BA%94%EB%93%A4-%EC%86%8D-%EC%A0%84%EA%B2%A9-%EC%82%AC%EC%9E%84cfo-%EC%BD%9C%EB%A0%9B-%ED%81%AC%EB%A0%88%EC%8A%A4%EA%B0%80-%EC%9E%84%EC%8B%9C-%EC%A7%80%ED%9C%98-2026-11-12) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.13 | [도란의 갱도에서 광석이 안 나올 때 \| 네크로맨서 RPG 첫 골렘 공략](https://velog.io/@ancoachstudio/%EB%8F%84%EB%9E%80%EC%9D%98-%EA%B0%B1%EB%8F%84%EC%97%90%EC%84%9C-%EA%B4%91%EC%84%9D%EC%9D%B4-%EC%95%88-%EB%82%98%EC%98%AC-%EB%95%8C-%EB%84%A4%ED%81%AC%EB%A1%9C%EB%A7%A8%EC%84%9C-RPG-%EC%B2%AB-%EA%B3%A8%EB%A0%98-%EA%B3%B5%EB%9E%B5) | [@ancoachstudio](https://velog.io/@ancoachstudio) |
| 2026.11.13 | [[1분 브리핑] Fable 5.2는 기획에만, 구현은 Opus 5.5](https://velog.io/@sdm77/1%EB%B6%84-%EB%B8%8C%EB%A6%AC%ED%95%91-2026-11-13) | [@sdm77](https://velog.io/@sdm77) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
