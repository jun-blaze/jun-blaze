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
| 2026.09.12 | [kubernetes pod란?](https://velog.io/@dreaming/kubernetes-pod%EB%9E%80) | [@dreaming](https://velog.io/@dreaming) |
| 2026.09.12 | [[PostgreSQL] 24. 물리 백업 (2) - pgBackRest: 백업과 복구](https://velog.io/@jinwoo_study/PostgreSQL-24.-%EB%AC%BC%EB%A6%AC-%EB%B0%B1%EC%97%85-2-pgBackRest-%EA%B8%B0%EB%B3%B8-%EB%B0%B1%EC%97%85%EA%B3%BC-%EB%B3%B5%EA%B5%AC) | [@jinwoo_study](https://velog.io/@jinwoo_study) |
| 2026.09.12 | [앱스토어 리젝 3번 당하고 알게 된 것들 — 사유 코드가 아니라 스크린샷을 봐라](https://velog.io/@takixzsx/%EC%95%B1%EC%8A%A4%ED%86%A0%EC%96%B4-%EB%A6%AC%EC%A0%9D-3%EB%B2%88-%EB%8B%B9%ED%95%98%EA%B3%A0-%EC%95%8C%EA%B2%8C-%EB%90%9C-%EA%B2%83%EB%93%A4-%EC%82%AC%EC%9C%A0-%EC%BD%94%EB%93%9C%EA%B0%80-%EC%95%84%EB%8B%88%EB%9D%BC-%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%EC%9D%84-%EB%B4%90%EB%9D%BC) | [@takixzsx](https://velog.io/@takixzsx) |
| 2026.09.12 | [AI 답답해서 내가 정리하는TerraForm](https://velog.io/@jkijki12/AI-%EB%8B%B5%EB%8B%B5%ED%95%B4%EC%84%9C-%EB%82%B4%EA%B0%80-%EC%A0%95%EB%A6%AC%ED%95%98%EB%8A%94TerraForm) | [@jkijki12](https://velog.io/@jkijki12) |
| 2026.09.12 | [NVIDIA는 커널을 부르고, Trainium은 프로그램을 올린다](https://velog.io/@victorjo/NVIDIA%EB%8A%94-%EC%BB%A4%EB%84%90%EC%9D%84-%EB%B6%80%EB%A5%B4%EA%B3%A0-Trainium%EC%9D%80-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8%EC%9D%84-%EC%98%AC%EB%A6%B0%EB%8B%A4) | [@victorjo](https://velog.io/@victorjo) |
| 2026.09.12 | [Unity 타격감 구현 - 히트스톱,화면 흔들림,히트 플래시,사운드 동기화](https://velog.io/@byjun9804/Unity-%ED%83%80%EA%B2%A9%EA%B0%90-%EA%B5%AC%ED%98%84-%ED%9E%88%ED%8A%B8%EC%8A%A4%ED%86%B1%ED%99%94%EB%A9%B4-%ED%9D%94%EB%93%A4%EB%A6%BC%ED%9E%88%ED%8A%B8-%ED%94%8C%EB%9E%98%EC%8B%9C%EC%82%AC%EC%9A%B4%EB%93%9C-%EB%8F%99%EA%B8%B0%ED%99%94) | [@byjun9804](https://velog.io/@byjun9804) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
