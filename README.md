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
| 2026.09.09 | [프로그래머스 영어가 싫어요](https://velog.io/@youngjun_10/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%A8%B8%EC%8A%A4-%EC%98%81%EC%96%B4%EA%B0%80-%EC%8B%AB%EC%96%B4%EC%9A%94) | [@youngjun_10](https://velog.io/@youngjun_10) |
| 2026.09.09 | [전자정부 프레임 워크 개발 공부4일차](https://velog.io/@happyboy1269/%EC%A0%84%EC%9E%90%EC%A0%95%EB%B6%80-%ED%94%84%EB%A0%88%EC%9E%84-%EC%9B%8C%ED%81%AC-%EA%B0%9C%EB%B0%9C-%EA%B3%B5%EB%B6%804%EC%9D%BC%EC%B0%A8) | [@happyboy1269](https://velog.io/@happyboy1269) |
| 2026.09.09 | [2. 이커머스 반품 데이터 분석: 문구류와 공책의 반품률은 왜 높았을까?](https://velog.io/@ing_dataorange0/2.-%EC%9D%B4%EC%BB%A4%EB%A8%B8%EC%8A%A4-%EB%B0%98%ED%92%88-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EB%B6%84%EC%84%9D-%EB%AC%B8%EA%B5%AC%EB%A5%98%EC%99%80-%EA%B3%B5%EC%B1%85%EC%9D%98-%EB%B0%98%ED%92%88%EB%A5%A0%EC%9D%80-%EC%99%9C-%EB%86%92%EC%95%98%EC%9D%84%EA%B9%8C) | [@ing_dataorange0](https://velog.io/@ing_dataorange0) |
| 2026.09.09 | [[백엔드] 시스템과 가장 쉽고 강력하게 상호작용 할 수 있는 방법 #5 - Series4 : 추가 인프라 구축없이 Binlog Consuming/Local Cache(Caffeine) 체계 구성을 통한 Redis 대체재 성능 테스트](https://velog.io/@gyrbs22/%EB%B0%B1%EC%97%94%EB%93%9C-%EC%8B%9C%EC%8A%A4%ED%85%9C%EA%B3%BC-%EA%B0%80%EC%9E%A5-%EC%89%BD%EA%B3%A0-%EA%B0%95%EB%A0%A5%ED%95%98%EA%B2%8C-%EC%83%81%ED%98%B8%EC%9E%91%EC%9A%A9-%ED%95%A0-%EC%88%98-%EC%9E%88%EB%8A%94-%EB%B0%A9%EB%B2%95-5-Series4-%EC%B6%94%EA%B0%80-%EC%9D%B8%ED%94%84%EB%9D%BC-%EA%B5%AC%EC%B6%95%EC%97%86%EC%9D%B4-Binlog-ConsumingLocal-CacheCaffeine-%EC%B2%B4%EA%B3%84-%EA%B5%AC%EC%84%B1%EC%9D%84-%ED%86%B5%ED%95%9C-Redis-%EB%8C%80%EC%B2%B4%EC%9E%AC-%EC%84%B1%EB%8A%A5-%ED%85%8C%EC%8A%A4%ED%8A%B8) | [@gyrbs22](https://velog.io/@gyrbs22) |
| 2026.09.09 | [Docker 총정리](https://velog.io/@junyeol1009/Docker-%EC%B4%9D%EC%A0%95%EB%A6%AC) | [@junyeol1009](https://velog.io/@junyeol1009) |
| 2026.09.09 | [[LG CNS AM INSPIRE CAMP 6기] DAY 29 - Spring Data JPA (Entity-DTO 변환, 연관관계, Validation, 예외처리)](https://velog.io/@hyr031888-crypto/LG-CNS-AM-INSPIRE-CAMP-6%EA%B8%B0-DAY-29-Spring-Data-JPA-Entity-DTO-%EB%B3%80%ED%99%98-%EC%97%B0%EA%B4%80%EA%B4%80%EA%B3%84-Validation-%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC) | [@hyr031888-crypto](https://velog.io/@hyr031888-crypto) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
