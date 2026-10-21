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
| 2026.10.22 | [유기농 반려동물 사료 시장, 프리미엄 반려동물 영양에 대한 수요 증가에 힘입어 2036년까지 57억 달러 규모에 도달, 연평균 7.8% 성장 전망](https://velog.io/@fmifoodblogdata/%EC%9C%A0%EA%B8%B0%EB%86%8D-%EB%B0%98%EB%A0%A4%EB%8F%99%EB%AC%BC-%EC%82%AC%EB%A3%8C-%EC%8B%9C%EC%9E%A5-%ED%94%84%EB%A6%AC%EB%AF%B8%EC%97%84-%EB%B0%98%EB%A0%A4%EB%8F%99%EB%AC%BC-%EC%98%81%EC%96%91%EC%97%90-%EB%8C%80%ED%95%9C-%EC%88%98%EC%9A%94-%EC%A6%9D%EA%B0%80%EC%97%90-%ED%9E%98%EC%9E%85%EC%96%B4-2036%EB%85%84%EA%B9%8C%EC%A7%80-57%EC%96%B5-%EB%8B%AC%EB%9F%AC-%EA%B7%9C%EB%AA%A8%EC%97%90-%EB%8F%84%EB%8B%AC-%EC%97%B0%ED%8F%89%EA%B7%A0-7.8-%EC%84%B1%EC%9E%A5-%EC%A0%84%EB%A7%9D) | [@fmifoodblogdata](https://velog.io/@fmifoodblogdata) |
| 2026.10.22 | [통합 감미료 솔루션 시장은 2036년까지 128억 달러에 달할 것으로 예상되며, 연평균 9.0%의 성장률을 보일 전망입니다.](https://velog.io/@fmifoodblogdata/%ED%86%B5%ED%95%A9-%EA%B0%90%EB%AF%B8%EB%A3%8C-%EC%86%94%EB%A3%A8%EC%85%98-%EC%8B%9C%EC%9E%A5%EC%9D%80-2036%EB%85%84%EA%B9%8C%EC%A7%80-128%EC%96%B5-%EB%8B%AC%EB%9F%AC%EC%97%90-%EB%8B%AC%ED%95%A0-%EA%B2%83%EC%9C%BC%EB%A1%9C-%EC%98%88%EC%83%81%EB%90%98%EB%A9%B0-%EC%97%B0%ED%8F%89%EA%B7%A0-9.0%EC%9D%98-%EC%84%B1%EC%9E%A5%EB%A5%A0%EC%9D%84-%EB%B3%B4%EC%9D%BC-%EC%A0%84%EB%A7%9D%EC%9E%85%EB%8B%88%EB%8B%A4) | [@fmifoodblogdata](https://velog.io/@fmifoodblogdata) |
| 2026.10.22 | [폰단트 및 슈가 페이스트 시장, 2036년까지 30억 9천만 달러 규모에 도달 전망, 연평균 12.2% 성장](https://velog.io/@fmifoodblogdata/%ED%8F%B0%EB%8B%A8%ED%8A%B8-%EB%B0%8F-%EC%8A%88%EA%B0%80-%ED%8E%98%EC%9D%B4%EC%8A%A4%ED%8A%B8-%EC%8B%9C%EC%9E%A5-2036%EB%85%84%EA%B9%8C%EC%A7%80-30%EC%96%B5-9%EC%B2%9C%EB%A7%8C-%EB%8B%AC%EB%9F%AC-%EA%B7%9C%EB%AA%A8%EC%97%90-%EB%8F%84%EB%8B%AC-%EC%A0%84%EB%A7%9D-%EC%97%B0%ED%8F%89%EA%B7%A0-12.2-%EC%84%B1%EC%9E%A5) | [@fmifoodblogdata](https://velog.io/@fmifoodblogdata) |
| 2026.10.22 | [26O21a](https://velog.io/@youngkyoo_kim/26O21a) | [@youngkyoo_kim](https://velog.io/@youngkyoo_kim) |
| 2026.10.22 | [[1분 브리핑] AI가 코드를 쓰자 병목은 리뷰로 옮겨갔다](https://velog.io/@sdm77/1%EB%B6%84-%EB%B8%8C%EB%A6%AC%ED%95%91-2026-10-22) | [@sdm77](https://velog.io/@sdm77) |
| 2026.10.22 | [원샷 프롬프트, 155조 토큰 서빙, 에이전트 차단](https://velog.io/@sdm77/%EB%AA%A8%EB%8D%B8%EC%97%85%EA%B3%84-%EB%8F%99%ED%96%A5-2026-10-22) | [@sdm77](https://velog.io/@sdm77) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
