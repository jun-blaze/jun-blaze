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
| 2026.10.06 | [AI 도입을 결정하기 전에 어떤 운영 조건을 점검할까](https://velog.io/@bbqgo807/ai-%EB%8F%84%EC%9E%85%EC%9D%84-%EA%B2%B0%EC%A0%95%ED%95%98%EA%B8%B0-%EC%A0%84%EC%97%90-%EC%96%B4%EB%96%A4-%EC%9A%B4%EC%98%81-%EC%A1%B0%EA%B1%B4%EC%9D%84-%EC%A0%90%EA%B2%80%ED%95%A0%EA%B9%8C-e13290) | [@bbqgo807](https://velog.io/@bbqgo807) |
| 2026.10.06 | [[정보처리기사] 데이터 모델 3요소와 DB 설계 단계](https://velog.io/@jedi/%EC%A0%95%EB%B3%B4%EC%B2%98%EB%A6%AC%EA%B8%B0%EC%82%AC-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EB%AA%A8%EB%8D%B8-3%EC%9A%94%EC%86%8C%EC%99%80-DB-%EC%84%A4%EA%B3%84-%EB%8B%A8%EA%B3%84) | [@jedi](https://velog.io/@jedi) |
| 2026.10.06 | [엔비디아가 투자한 리플렉션AI, 501B 파라미터 오픈웨이트 모델 '빔' 공개](https://velog.io/@bbzjun/%EC%97%94%EB%B9%84%EB%94%94%EC%95%84%EA%B0%80-%ED%88%AC%EC%9E%90%ED%95%9C-%EB%A6%AC%ED%94%8C%EB%A0%89%EC%85%98ai-501b-%ED%8C%8C%EB%9D%BC%EB%AF%B8%ED%84%B0-%EC%98%A4%ED%94%88%EC%9B%A8%EC%9D%B4%ED%8A%B8-%EB%AA%A8%EB%8D%B8-%EB%B9%94-%EA%B3%B5%EA%B0%9C-2026-10-05) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.10.06 | [일기장처럼 쓴 클로드가 신고했다…앤트로픽 제보로 중범죄 기소된 플로리다 여성](https://velog.io/@bbzjun/%EC%9D%BC%EA%B8%B0%EC%9E%A5%EC%B2%98%EB%9F%BC-%EC%93%B4-%ED%81%B4%EB%A1%9C%EB%93%9C%EA%B0%80-%EC%8B%A0%EA%B3%A0%ED%96%88%EB%8B%A4%EC%95%A4%ED%8A%B8%EB%A1%9C%ED%94%BD-%EC%A0%9C%EB%B3%B4%EB%A1%9C-%EC%A4%91%EB%B2%94%EC%A3%84-%EA%B8%B0%EC%86%8C%EB%90%9C-%ED%94%8C%EB%A1%9C%EB%A6%AC%EB%8B%A4-%EC%97%AC%EC%84%B1-2026-10-05) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.10.06 | [직접 만들고, 부딪히고, 기록하기](https://velog.io/@jedi/%EC%A7%81%EC%A0%91-%EB%A7%8C%EB%93%A4%EA%B3%A0-%EB%B6%80%EB%94%AA%ED%9E%88%EA%B3%A0-%EA%B8%B0%EB%A1%9D%ED%95%98%EA%B8%B0) | [@jedi](https://velog.io/@jedi) |
| 2026.10.06 | [신한·KB국민은행까지 뚫렸다…AI 공격도구 'ARTEX'發 전 금융권 보안 비상](https://velog.io/@bbzjun/%EC%8B%A0%ED%95%9Ckb%EA%B5%AD%EB%AF%BC%EC%9D%80%ED%96%89%EA%B9%8C%EC%A7%80-%EB%9A%AB%EB%A0%B8%EB%8B%A4ai-%EA%B3%B5%EA%B2%A9%EB%8F%84%EA%B5%AC-artex%E7%99%BC-%EC%A0%84-%EA%B8%88%EC%9C%B5%EA%B6%8C-%EB%B3%B4%EC%95%88-%EB%B9%84%EC%83%81-2026-10-05) | [@bbzjun](https://velog.io/@bbzjun) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
