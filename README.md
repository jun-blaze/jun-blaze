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
| 2026.11.22 | [# LG 소액결제 정책 결제 제한이 발생하는 이유와 확인 방법](https://velog.io/@bareunbank/LG-%EC%86%8C%EC%95%A1%EA%B2%B0%EC%A0%9C-%EC%A0%95%EC%B1%85-%EA%B2%B0%EC%A0%9C-%EC%A0%9C%ED%95%9C%EC%9D%B4-%EB%B0%9C%EC%83%9D%ED%95%98%EB%8A%94-%EC%9D%B4%EC%9C%A0%EC%99%80-%ED%99%95%EC%9D%B8-%EB%B0%A9%EB%B2%95) | [@bareunbank](https://velog.io/@bareunbank) |
| 2026.11.22 | [OpenAI, '적대적 증류' 공격 대응 공개…체인오브쏘트 추출 방어 강화](https://velog.io/@bbzjun/openai-%EC%A0%81%EB%8C%80%EC%A0%81-%EC%A6%9D%EB%A5%98-%EA%B3%B5%EA%B2%A9-%EB%8C%80%EC%9D%91-%EA%B3%B5%EA%B0%9C%EC%B2%B4%EC%9D%B8%EC%98%A4%EB%B8%8C%EC%8F%98%ED%8A%B8-%EC%B6%94%EC%B6%9C-%EB%B0%A9%EC%96%B4-%EA%B0%95%ED%99%94-2026-11-21) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.22 | [메타, AI 데이터센터발 탄소배출 45% 급증에 2030년 넷제로 목표 재검토](https://velog.io/@bbzjun/%EB%A9%94%ED%83%80-ai-%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%84%BC%ED%84%B0%EB%B0%9C-%ED%83%84%EC%86%8C%EB%B0%B0%EC%B6%9C-45-%EA%B8%89%EC%A6%9D%EC%97%90-2030%EB%85%84-%EB%84%B7%EC%A0%9C%EB%A1%9C-%EB%AA%A9%ED%91%9C-%EC%9E%AC%EA%B2%80%ED%86%A0-2026-11-21) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.22 | [200만 개 '가짜 비밀번호'로 밝혀낸 AI 업계의 민감정보 유출 실태](https://velog.io/@bbzjun/200%EB%A7%8C-%EA%B0%9C-%EA%B0%80%EC%A7%9C-%EB%B9%84%EB%B0%80%EB%B2%88%ED%98%B8%EB%A1%9C-%EB%B0%9D%ED%98%80%EB%82%B8-ai-%EC%97%85%EA%B3%84%EC%9D%98-%EB%AF%BC%EA%B0%90%EC%A0%95%EB%B3%B4-%EC%9C%A0%EC%B6%9C-%EC%8B%A4%ED%83%9C-2026-11-21) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.22 | [[8주차 토픽] @Transactional만 붙이면 모든 문제가 해결될까?](https://velog.io/@chanhajeong/8%EC%A3%BC%EC%B0%A8-%ED%86%A0%ED%94%BD) | [@chanhajeong](https://velog.io/@chanhajeong) |
| 2026.11.22 | [작은 토큰 세트를 폴더로 나눌 때 색 이름과 지형 라벨을 섞지 않기](https://velog.io/@danielbrooks84/%EC%9E%91%EC%9D%80-%ED%86%A0%ED%81%B0-%EC%84%B8%ED%8A%B8%EB%A5%BC-%ED%8F%B4%EB%8D%94%EB%A1%9C-%EB%82%98%EB%88%8C-%EB%95%8C-%EC%83%89-%EC%9D%B4%EB%A6%84%EA%B3%BC-%EC%A7%80%ED%98%95-%EB%9D%BC%EB%B2%A8%EC%9D%84-%EC%84%9E%EC%A7%80-%EC%95%8A%EA%B8%B0) | [@danielbrooks84](https://velog.io/@danielbrooks84) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
