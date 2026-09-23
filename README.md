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
| 2026.09.24 | [S3에 포트폴리오 올리기 (느린 문제 해결> CloudFront)](https://velog.io/@o980204/S3%EC%97%90-%ED%8F%AC%ED%8A%B8%ED%8F%B4%EB%A6%AC%EC%98%A4-%EC%98%AC%EB%A6%AC%EA%B8%B0-%EB%8A%90%EB%A6%B0-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0-CloudFront) | [@o980204](https://velog.io/@o980204) |
| 2026.09.24 | [[SlateKR #165] 6시 축 잔재 판정과 컨벤션 전수 probe](https://velog.io/@dh82680/SlateKR-165-6%EC%8B%9C-%EC%B6%95-%EC%9E%94%EC%9E%AC-%ED%8C%90%EC%A0%95%EA%B3%BC-%EC%BB%A8%EB%B2%A4%EC%85%98-%EC%A0%84%EC%88%98-probe) | [@dh82680](https://velog.io/@dh82680) |
| 2026.09.24 | [2026-09-22 부동산공법 건축법~농지법 4회독](https://velog.io/@hyungyugod/2026-09-22-%EB%B6%80%EB%8F%99%EC%82%B0%EA%B3%B5%EB%B2%95-%EA%B1%B4%EC%B6%95%EB%B2%95%EB%86%8D%EC%A7%80%EB%B2%95-4%ED%9A%8C%EB%8F%85) | [@hyungyugod](https://velog.io/@hyungyugod) |
| 2026.09.24 | [3. 포인터 멤버의 필요성과 주의점, 매개변수와 인자, Pass-by-value vs Pass-by-reference, 상수성(Constness), Pointer to constant value와 constant pointer to value, 매개변수와 리턴 타입의 constness, 매개변수 순서, 상수성 활용 코딩스타일, RVO](https://velog.io/@woon2lavi/3.-%ED%8F%AC%EC%9D%B8%ED%84%B0-%EB%A9%A4%EB%B2%84%EC%9D%98-%ED%95%84%EC%9A%94%EC%84%B1%EA%B3%BC-%EC%A3%BC%EC%9D%98%EC%A0%90-Pass-by-value-vs-Pass-by-reference-%EC%83%81%EC%88%98%EC%84%B1Constness-Pointer-to-constant-value%EC%99%80-constant-pointer-to-value-%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98%EC%99%80-%EB%A6%AC%ED%84%B4-%ED%83%80%EC%9E%85%EC%9D%98-constness-%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98-%EC%88%9C%EC%84%9C-%EC%83%81%EC%88%98%EC%84%B1-%ED%99%9C%EC%9A%A9-%EC%BD%94%EB%94%A9%EC%8A%A4%ED%83%80%EC%9D%BC-RVO) | [@woon2lavi](https://velog.io/@woon2lavi) |
| 2026.09.24 | [@ExceptionHandler가 많아질 때 BusinessException으로 정리하기](https://velog.io/@sleekydevzero86/ExceptionHandler%EA%B0%80-%EB%A7%8E%EC%95%84%EC%A7%88-%EB%95%8C-BusinessException%EC%9C%BC%EB%A1%9C-%EC%A0%95%EB%A6%AC%ED%95%98%EA%B8%B0) | [@sleekydevzero86](https://velog.io/@sleekydevzero86) |
| 2026.09.24 | [[코딩테스트] Python 필수 문법 총정리](https://velog.io/@lareina7486/%EC%BD%94%EB%94%A9%ED%85%8C%EC%8A%A4%ED%8A%B8-Python-%ED%95%84%EC%88%98-%EB%AC%B8%EB%B2%95-%EC%B4%9D%EC%A0%95%EB%A6%AC) | [@lareina7486](https://velog.io/@lareina7486) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
