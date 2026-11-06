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
| 2026.11.07 | [26N07a](https://velog.io/@youngkyoo_kim/26N07a-ggkt4e3v) | [@youngkyoo_kim](https://velog.io/@youngkyoo_kim) |
| 2026.11.07 | [오픈AI, 보안업체 핵트론과 공식 파트너십…"프런티어 AI로 취약점 선제 발굴"](https://velog.io/@bbzjun/%EC%98%A4%ED%94%88ai-%EB%B3%B4%EC%95%88%EC%97%85%EC%B2%B4-%ED%95%B5%ED%8A%B8%EB%A1%A0%EA%B3%BC-%EA%B3%B5%EC%8B%9D-%ED%8C%8C%ED%8A%B8%EB%84%88%EC%8B%AD%ED%94%84%EB%9F%B0%ED%8B%B0%EC%96%B4-ai%EB%A1%9C-%EC%B7%A8%EC%95%BD%EC%A0%90-%EC%84%A0%EC%A0%9C-%EB%B0%9C%EA%B5%B4-2026-11-06-4l9ye38h) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.07 | [오픈AI, 보안업체 핵트론과 공식 파트너십…"프런티어 AI로 취약점 선제 발굴"](https://velog.io/@bbzjun/%EC%98%A4%ED%94%88ai-%EB%B3%B4%EC%95%88%EC%97%85%EC%B2%B4-%ED%95%B5%ED%8A%B8%EB%A1%A0%EA%B3%BC-%EA%B3%B5%EC%8B%9D-%ED%8C%8C%ED%8A%B8%EB%84%88%EC%8B%AD%ED%94%84%EB%9F%B0%ED%8B%B0%EC%96%B4-ai%EB%A1%9C-%EC%B7%A8%EC%95%BD%EC%A0%90-%EC%84%A0%EC%A0%9C-%EB%B0%9C%EA%B5%B4-2026-11-06) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.07 | [메타, 뉴스 무단수집 논란 일자 AI 스크래핑 상업약관 업데이트 무기한 보류](https://velog.io/@bbzjun/%EB%A9%94%ED%83%80-%EB%89%B4%EC%8A%A4-%EB%AC%B4%EB%8B%A8%EC%88%98%EC%A7%91-%EB%85%BC%EB%9E%80-%EC%9D%BC%EC%9E%90-ai-%EC%8A%A4%ED%81%AC%EB%9E%98%ED%95%91-%EC%83%81%EC%97%85%EC%95%BD%EA%B4%80-%EC%97%85%EB%8D%B0%EC%9D%B4%ED%8A%B8-%EB%AC%B4%EA%B8%B0%ED%95%9C-%EB%B3%B4%EB%A5%98-2026-11-06) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.07 | [앤트로픽, IPO 몸값 1.5조 달러→1조 달러로 추락…AI 투매 쇼크에 11월 상장 '먹구름'](https://velog.io/@bbzjun/%EC%95%A4%ED%8A%B8%EB%A1%9C%ED%94%BD-ipo-%EB%AA%B8%EA%B0%92-15%EC%A1%B0-%EB%8B%AC%EB%9F%AC1%EC%A1%B0-%EB%8B%AC%EB%9F%AC%EB%A1%9C-%EC%B6%94%EB%9D%BDai-%ED%88%AC%EB%A7%A4-%EC%87%BC%ED%81%AC%EC%97%90-11%EC%9B%94-%EC%83%81%EC%9E%A5-%EB%A8%B9%EA%B5%AC%EB%A6%84-2026-11-06) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.07 | [[zaqoo자꾸]어제 작업](https://velog.io/@lco2009d/zaqoo%EC%9E%90%EA%BE%B8%EC%96%B4%EC%A0%9C-%EC%9E%91%EC%97%85) | [@lco2009d](https://velog.io/@lco2009d) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
