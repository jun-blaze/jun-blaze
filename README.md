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
| 2026.10.19 | [DOJ 663 '탈옥 작전' (WIP)](https://velog.io/@doubledeltas/doj-663) | [@doubledeltas](https://velog.io/@doubledeltas) |
| 2026.10.19 | [34주 차;-
학생 테스트를 통한 학습과 개선](https://velog.io/@baintai/34%EC%A3%BC-%EC%B0%A8-%ED%95%99%EC%83%9D-%ED%85%8C%EC%8A%A4%ED%8A%B8%EB%A5%BC-%ED%86%B5%ED%95%9C-%ED%95%99%EC%8A%B5%EA%B3%BC-%EA%B0%9C%EC%84%A0) | [@baintai](https://velog.io/@baintai) |
| 2026.10.19 | [이진 탐색은 정렬된 배열에서 값을 찾는 공식이 아니다](https://velog.io/@vxdeveloper/algorithm33) | [@vxdeveloper](https://velog.io/@vxdeveloper) |
| 2026.10.19 | [Linux PataOS: Debian 13과 Cinnamon 기반의 CAD/CAM/CAE 전용 커스텀 리눅스 아키텍처 설계](https://velog.io/@alessandropatane/Linux-PataOS-Debian-13%EA%B3%BC-Cinnamon-%EA%B8%B0%EB%B0%98%EC%9D%98-CADCAMCAE-%EC%A0%84%EC%9A%A9-%EC%BB%A4%EC%8A%A4%ED%85%80-%EB%A6%AC%EB%88%85%EC%8A%A4-%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98-%EC%84%A4%EA%B3%84) | [@alessandropatane](https://velog.io/@alessandropatane) |
| 2026.10.19 | [Socket.IO가 잠깐 끊겨도 STT를 살려 두면서 비용 카운터를 둘로 나눈 이야기](https://velog.io/@florian13/Socket.IO%EA%B0%80-%EC%9E%A0%EA%B9%90-%EB%81%8A%EA%B2%A8%EB%8F%84-STT%EB%A5%BC-%EC%82%B4%EB%A0%A4-%EB%91%90%EB%A9%B4%EC%84%9C-%EB%B9%84%EC%9A%A9-%EC%B9%B4%EC%9A%B4%ED%84%B0%EB%A5%BC-%EB%91%98%EB%A1%9C-%EB%82%98%EB%88%88-%EC%9D%B4%EC%95%BC%EA%B8%B0) | [@florian13](https://velog.io/@florian13) |
| 2026.10.19 | [되돌아오는 길이 없으면 끝난 것은 갇힌 것이다 — 구조인식(構造認識) 노트 ②](https://velog.io/@linxiaohei/%EB%90%98%EB%8F%8C%EC%95%84%EC%98%A4%EB%8A%94-%EA%B8%B8%EC%9D%B4-%EC%97%86%EC%9C%BC%EB%A9%B4-%EB%81%9D%EB%82%9C-%EA%B2%83%EC%9D%80-%EA%B0%87%ED%9E%8C-%EA%B2%83%EC%9D%B4%EB%8B%A4-%EA%B5%AC%EC%A1%B0%EC%9D%B8%EC%8B%9D%E6%A7%8B%E9%80%A0%E8%AA%8D%E8%AD%98-%EB%85%B8%ED%8A%B8) | [@linxiaohei](https://velog.io/@linxiaohei) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
