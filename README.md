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
| 2026.09.11 | [[논문 리뷰] Claude, GPT 모델 교체 시 '메모리'가 증발하는 기술적 이유](https://velog.io/@sue77/%EB%85%BC%EB%AC%B8-%EB%A6%AC%EB%B7%B0-Claude-GPT-%EB%AA%A8%EB%8D%B8-%EA%B5%90%EC%B2%B4-%EC%8B%9C-%EB%A9%94%EB%AA%A8%EB%A6%AC%EA%B0%80-%EC%A6%9D%EB%B0%9C%ED%95%98%EB%8A%94-%EA%B8%B0%EC%88%A0%EC%A0%81-%EC%9D%B4%EC%9C%A0) | [@sue77](https://velog.io/@sue77) |
| 2026.09.11 | [프로그래머스 - 뒤에 있는 큰 수 찾기](https://velog.io/@gwangmin-kim/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%A8%B8%EC%8A%A4-%EB%92%A4%EC%97%90-%EC%9E%88%EB%8A%94-%ED%81%B0-%EC%88%98-%EC%B0%BE%EA%B8%B0) | [@gwangmin-kim](https://velog.io/@gwangmin-kim) |
| 2026.09.11 | [Codex 0.154.0 Worktree: AI Agent 여러 개가 같은 Spring Boot 저장소를 건드릴 때 충돌을 막는 방법](https://velog.io/@gwanghun-choi/Codex-0.154.0-Worktree-AI-Agent-%EC%97%AC%EB%9F%AC-%EA%B0%9C%EA%B0%80-%EA%B0%99%EC%9D%80-Spring-Boot-%EC%A0%80%EC%9E%A5%EC%86%8C%EB%A5%BC-%EA%B1%B4%EB%93%9C%EB%A6%B4-%EB%95%8C-%EC%B6%A9%EB%8F%8C%EC%9D%84-%EB%A7%89%EB%8A%94-%EB%B0%A9%EB%B2%95) | [@gwanghun-choi](https://velog.io/@gwanghun-choi) |
| 2026.09.11 | [Gradle 9.8 RC1: Java 27 지원과 Maven Mirror 설정 재사용, 사내 빌드 인프라가 단순해진다](https://velog.io/@gwanghun-choi/Gradle-9.8-RC1-Java-27-%EC%A7%80%EC%9B%90%EA%B3%BC-Maven-Mirror-%EC%84%A4%EC%A0%95-%EC%9E%AC%EC%82%AC%EC%9A%A9-%EC%82%AC%EB%82%B4-%EB%B9%8C%EB%93%9C-%EC%9D%B8%ED%94%84%EB%9D%BC%EA%B0%80-%EB%8B%A8%EC%88%9C%ED%95%B4%EC%A7%84%EB%8B%A4) | [@gwanghun-choi](https://velog.io/@gwanghun-choi) |
| 2026.09.11 | [라즈베리 파이 AP 보안 강화와 트래픽 가시성 (3)](https://velog.io/@kyhw/pihole3) | [@kyhw](https://velog.io/@kyhw) |
| 2026.09.11 | [[DirectX12] 17.1 사원수](https://velog.io/@rladuddbs/DirectX12-17.1-%EC%82%AC%EC%9B%90%EC%88%98) | [@rladuddbs](https://velog.io/@rladuddbs) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
