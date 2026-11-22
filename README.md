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
| 2026.11.23 | [이젠 AI끼리 대화를 한다. 정말 사람같다.](https://velog.io/@reipier/%EC%9D%B4%EC%A0%A0-AI%EB%81%BC%EB%A6%AC-%EB%8C%80%ED%99%94%EB%A5%BC-%ED%95%9C%EB%8B%A4.-%EC%A0%95%EB%A7%90-%EC%82%AC%EB%9E%8C%EA%B0%99%EB%8B%A4) | [@reipier](https://velog.io/@reipier) |
| 2026.11.23 | [[기후·환경 뉴스 브리핑] 빅토리아, 2028년 석탄발전 종료 앞두고 전력 공백 논란 (11.22)](https://velog.io/@hyuckjin/%EA%B8%B0%ED%9B%84%ED%99%98%EA%B2%BD-%EB%89%B4%EC%8A%A4-%EB%B8%8C%EB%A6%AC%ED%95%91-%EB%B9%85%ED%86%A0%EB%A6%AC%EC%95%84-2028%EB%85%84-%EC%84%9D%ED%83%84%EB%B0%9C%EC%A0%84-%EC%A2%85%EB%A3%8C-%EC%95%9E%EB%91%90%EA%B3%A0-%EC%A0%84%EB%A0%A5-%EA%B3%B5%EB%B0%B1-%EB%85%BC%EB%9E%80-11.22) | [@hyuckjin](https://velog.io/@hyuckjin) |
| 2026.11.23 | [붙여넣기한 본문 4,914자가 발행에서 사라졌습니다 — 저장되지 않은 DOM과 에디터 모델이 갈라질 때](https://velog.io/@returncare/%EB%B6%99%EC%97%AC%EB%84%A3%EA%B8%B0%ED%95%9C-%EB%B3%B8%EB%AC%B8-4914%EC%9E%90%EA%B0%80-%EB%B0%9C%ED%96%89%EC%97%90%EC%84%9C-%EC%82%AC%EB%9D%BC%EC%A1%8C%EC%8A%B5%EB%8B%88%EB%8B%A4-%EC%A0%80%EC%9E%A5%EB%90%98%EC%A7%80-%EC%95%8A%EC%9D%80-DOM%EA%B3%BC-%EC%97%90%EB%94%94%ED%84%B0-%EB%AA%A8%EB%8D%B8%EC%9D%B4-%EA%B0%88%EB%9D%BC%EC%A7%88-%EB%95%8C) | [@returncare](https://velog.io/@returncare) |
| 2026.11.23 | [엔비디아의 두 얼굴: 사상 최대 실적 속 흔들리는 리더십과 중국 리스크](https://velog.io/@bbzjun/%EC%97%94%EB%B9%84%EB%94%94%EC%95%84%EC%9D%98-%EB%91%90-%EC%96%BC%EA%B5%B4-%EC%82%AC%EC%83%81-%EC%B5%9C%EB%8C%80-%EC%8B%A4%EC%A0%81-%EC%86%8D-%ED%9D%94%EB%93%A4%EB%A6%AC%EB%8A%94-%EB%A6%AC%EB%8D%94%EC%8B%AD%EA%B3%BC-%EC%A4%91%EA%B5%AD-%EB%A6%AC%EC%8A%A4%ED%81%AC-2026-11-22) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.23 | ['하이퍼스케일' 저자가 짚은 빅테크 데이터센터 반발의 진짜 이유](https://velog.io/@bbzjun/%ED%95%98%EC%9D%B4%ED%8D%BC%EC%8A%A4%EC%BC%80%EC%9D%BC-%EC%A0%80%EC%9E%90%EA%B0%80-%EC%A7%9A%EC%9D%80-%EB%B9%85%ED%85%8C%ED%81%AC-%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%84%BC%ED%84%B0-%EB%B0%98%EB%B0%9C%EC%9D%98-%EC%A7%84%EC%A7%9C-%EC%9D%B4%EC%9C%A0-2026-11-22) | [@bbzjun](https://velog.io/@bbzjun) |
| 2026.11.23 | [OpenAI 수석과학자, AI 개발 속도 제한 위한 공동 지표로 '퍼플렉시티' 제안](https://velog.io/@bbzjun/openai-%EC%88%98%EC%84%9D%EA%B3%BC%ED%95%99%EC%9E%90-ai-%EA%B0%9C%EB%B0%9C-%EC%86%8D%EB%8F%84-%EC%A0%9C%ED%95%9C-%EC%9C%84%ED%95%9C-%EA%B3%B5%EB%8F%99-%EC%A7%80%ED%91%9C%EB%A1%9C-%ED%8D%BC%ED%94%8C%EB%A0%89%EC%8B%9C%ED%8B%B0-%EC%A0%9C%EC%95%88-2026-11-22) | [@bbzjun](https://velog.io/@bbzjun) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
