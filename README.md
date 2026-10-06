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
| 2026.10.06 | [파인튜닝 - 2단계: SFT 데이터와 loss를 이해한다](https://velog.io/@fpalzntm/%ED%8C%8C%EC%9D%B8%ED%8A%9C%EB%8B%9D-2%EB%8B%A8%EA%B3%84-SFT-%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%99%80-loss%EB%A5%BC-%EC%9D%B4%ED%95%B4%ED%95%9C%EB%8B%A4) | [@fpalzntm](https://velog.io/@fpalzntm) |
| 2026.10.06 | [파인튜닝 - 1단계: 사전학습, SFT, PEFT를 구분한다](https://velog.io/@fpalzntm/%ED%8C%8C%EC%9D%B8%ED%8A%9C%EB%8B%9D-1%EB%8B%A8%EA%B3%84-%EC%82%AC%EC%A0%84%ED%95%99%EC%8A%B5-SFT-PEFT%EB%A5%BC-%EA%B5%AC%EB%B6%84%ED%95%9C%EB%8B%A4) | [@fpalzntm](https://velog.io/@fpalzntm) |
| 2026.10.06 | [(원데이[무기명 테더가입가능]) 핸디캡/언더오버 연장미포함](https://velog.io/@mot597346/%EC%9B%90%EB%8D%B0%EC%9D%B4%EB%AC%B4%EA%B8%B0%EB%AA%85-%ED%85%8C%EB%8D%94%EA%B0%80%EC%9E%85%EA%B0%80%EB%8A%A5-%ED%95%B8%EB%94%94%EC%BA%A1%EC%96%B8%EB%8D%94%EC%98%A4%EB%B2%84-%EC%97%B0%EC%9E%A5%EB%AF%B8%ED%8F%AC%ED%95%A8-dsavu6g1) | [@mot597346](https://velog.io/@mot597346) |
| 2026.10.06 | [HBM과 반도체 섹터는 왜 주목받는가](https://velog.io/@jangjb_115/HBM%EA%B3%BC-%EB%B0%98%EB%8F%84%EC%B2%B4-%EC%84%B9%ED%84%B0%EB%8A%94-%EC%99%9C-%EC%A3%BC%EB%AA%A9%EB%B0%9B%EB%8A%94%EA%B0%80) | [@jangjb_115](https://velog.io/@jangjb_115) |
| 2026.10.06 | [땅따먹기_복습3](https://velog.io/@hi_soap/%EB%95%85%EB%94%B0%EB%A8%B9%EA%B8%B0%EB%B3%B5%EC%8A%B53) | [@hi_soap](https://velog.io/@hi_soap) |
| 2026.10.06 | [겨울철 코 건조와 물때 걱정 한 번에 잡는 에어메이드 아쿠아마린 9002 가습기](https://velog.io/@luisuh/%EA%B2%A8%EC%9A%B8%EC%B2%A0-%EC%BD%94-%EA%B1%B4%EC%A1%B0%EC%99%80-%EB%AC%BC%EB%95%8C-%EA%B1%B1%EC%A0%95-%ED%95%9C-%EB%B2%88%EC%97%90-%EC%9E%A1%EB%8A%94-%EC%97%90%EC%96%B4%EB%A9%94%EC%9D%B4%EB%93%9C-%EC%95%84%EC%BF%A0%EC%95%84%EB%A7%88%EB%A6%B0-9002-%EA%B0%80%EC%8A%B5%EA%B8%B0-pn5sx5sq) | [@luisuh](https://velog.io/@luisuh) |
<!-- VELOG:END -->

<sub>6시간마다 [GitHub Actions](.github/workflows/velog-feed.yml)로 자동 갱신됩니다.
velog 전역 피드에는 한국어 개발 글 외에 중국어 스팸 계정 글이 섞여 들어오므로,
[수집 스크립트](scripts/velog-feed.mjs)에서 한글·한자 비율로 걸러냅니다.</sub>
