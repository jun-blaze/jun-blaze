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
| 2026.10.21 | [면접스터디 day6](https://velog.io/@khjoo1203/%EB%A9%B4%EC%A0%91%EC%8A%A4%ED%84%B0%EB%94%94-day6) | [@khjoo1203](https://velog.io/@khjoo1203) |
| 2026.10.21 | [배포 파이프라인 만들기 - 사전: 뜻 — 층과 방식](https://velog.io/@neosiureu/%EB%B0%B0%ED%8F%AC-%ED%8C%8C%EC%9D%B4%ED%94%84%EB%9D%BC%EC%9D%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0-%EC%82%AC%EC%A0%84-%EB%9C%BB-%EC%B8%B5%EA%B3%BC-%EB%B0%A9%EC%8B%9D) | [@neosiureu](https://velog.io/@neosiureu) |
| 2026.10.21 | [[Making Mutation Arcade #30] 캐릭터를 움직였더니 비로소 게임처럼 보이기 시작했다](https://velog.io/@ms_moon/Making-Mutation-Arcade-30-%EC%BA%90%EB%A6%AD%ED%84%B0%EB%A5%BC-%EC%9B%80%EC%A7%81%EC%98%80%EB%8D%94%EB%8B%88-%EB%B9%84%EB%A1%9C%EC%86%8C-%EA%B2%8C%EC%9E%84%EC%B2%98%EB%9F%BC-%EB%B3%B4%EC%9D%B4%EA%B8%B0-%EC%8B%9C%EC%9E%91%ED%96%88%EB%8B%A4) | [@ms_moon](https://velog.io/@ms_moon) |
| 2026.10.21 | [팀 스터디 \| 1회차 [26.10.21]](https://velog.io/@datamong/%ED%8C%80-%EC%8A%A4%ED%84%B0%EB%94%94-1%ED%9A%8C%EC%B0%A8-26.10.21) | [@datamong](https://velog.io/@datamong) |
| 2026.10.21 | [네 제품의 SNS를 준비하며 정한 운영 원칙](https://velog.io/@davidmundev/%EB%84%A4-%EC%A0%9C%ED%92%88%EC%9D%98-SNS%EB%A5%BC-%EC%A4%80%EB%B9%84%ED%95%98%EB%A9%B0-%EC%A0%95%ED%95%9C-%EC%9A%B4%EC%98%81-%EC%9B%90%EC%B9%99) | [@davidmundev](https://velog.io/@davidmundev) |
| 2026.10.21 | [Jenkins 재시작 후 GitLab 자격증명만 사라진 이유](https://velog.io/@diqkraud/Jenkins-%EC%9E%AC%EC%8B%9C%EC%9E%91-%ED%9B%84-GitLab-%EC%9E%90%EA%B2%A9%EC%A6%9D%EB%AA%85%EB%A7%8C-%EC%82%AC%EB%9D%BC%EC%A7%84-%EC%9D%B4%EC%9C%A0) | [@diqkraud](https://velog.io/@diqkraud) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
