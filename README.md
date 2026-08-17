![header](https://capsule-render.vercel.app/api?type=waving&color=0:1A1A1A,100:444444&height=220&section=header&text=Yoon%20Myeongwoo&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20Developer&descAlignY=58&descSize=20)

## 👋 About Me

안녕하세요. **백엔드 개발자 윤명우**입니다.

단순히 동작하는 코드를 넘어, **장애 상황에서도 데이터 일관성을 유지할 수 있는 구조와 문제가 발생했을 때 빠르게 원인을 추적할 수 있는 시스템**을 고민합니다.

- 🔄 Kafka 기반 이벤트 처리와 **Transactional Outbox Pattern**을 활용한 데이터 정합성 설계
- 🧩 **DDD / MSA** 기반 서비스 경계 설계 및 Spring Cloud 공통 인프라 구축
- 📊 **Prometheus · Grafana · Loki · Zipkin**을 활용한 Observability 환경 구성
- 🤖 LLM을 활용한 장애 로그 분석 및 **Slack 장애 알림 자동화**
- 🚀 Jenkins / Docker 기반 **CI/CD 및 배포 환경 구축**

<br>

## 🛠 Tech Stack

### Backend
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Cloud-6DB33F?style=flat-square&logo=spring&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white"/>
  <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white"/>
  <img src="https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square"/>
</p>

### Messaging & Data
<p>
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
</p>

### Infra & DevOps
<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white"/>
  <img src="https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white"/>
</p>

### Observability
<p>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white"/>
  <img src="https://img.shields.io/badge/Loki-F46800?style=flat-square&logo=grafana&logoColor=white"/>
  <img src="https://img.shields.io/badge/Zipkin-000000?style=flat-square"/>
</p>

<br>

## 🚀 Projects

### 🏦 Finlearn
> 퀴즈로 금융 지식을 학습하고 모의투자로 실전 감각을 쌓는 금융 학습 플랫폼  
> **Backend Developer | 2026.04 - 2026.05 | 5인 팀**

🔗 [GitHub](https://github.com/F1NLEARN)

- Holding / TradeHistory / Portfolio Analysis 도메인 개발
- **Transactional Outbox Pattern**을 적용해 DB Transaction과 Kafka 이벤트 발행 간 정합성 확보
- 규칙 기반 분석과 생성형 AI를 결합하고 검증·Fallback 구조를 적용해 AI의 비결정성 격리
- **Eureka · API Gateway · Config Server · Common Module** 기반 MSA 공통 인프라 구성
- Jenkins 기반 CI/CD 파이프라인 구축
- **Prometheus · Grafana · Loki · Zipkin** 기반 Observability 환경 구축
- 장애 발생 시 ERROR 로그를 LLM이 분석하여 Slack으로 전달하는 장애 알림 자동화 구현

`Java` `Spring Boot` `Spring Cloud` `Kafka` `Redis` `PostgreSQL`
`Spring AI` `Docker` `Jenkins` `AWS` `GCP`

---

### 🚚 다2조부르릉
> 물류 관리 및 배송 시스템을 위한 MSA 기반 B2B 플랫폼  
> **Backend Developer | 2026.03 - 2026.04 | 6인 팀**

🔗 [GitHub](https://github.com/Lazernes/da2joburureung)

- **DDD 기반 Delivery Domain** 설계 및 API 구현
- Kafka 주문 이벤트를 기반으로 배송 정보를 자동 생성하는 이벤트 기반 구조 구현
- OpenFeign을 활용해 Order · Company · Hub 서비스와 동기 통신
- HUB_WAITING · HUB_MOVING 등 배송 상태 전이 로직 구현
- 허브 간 이동 순서 · 거리 · 소요 시간을 관리하는 DeliveryRouteRecord 구현

`Java` `Spring Boot` `Spring Cloud` `Kafka` `OpenFeign`
`Redis` `PostgreSQL` `QueryDSL` `Docker`

---

### 🌱 Morak
> 사회적 기업 소개 및 가치 소비 촉진 플랫폼  
> **Backend Developer / Team Lead | 2025.03 - 2025.05 | 5인 팀**

🔗 [GitHub](https://github.com/Lazernes/Morak-Backend)

- 회원 · 리뷰 · 기업 스토리 · 사회적경제 지원 공고 API 구현
- **Kakao OAuth2 + JWT** 기반 인증 구조 구현
- Access Token을 HttpOnly Cookie로 전달하여 XSS 공격 위험 완화
- Spring Security 기반 인증/인가 및 Role 기반 접근 제어
- 프론트·백엔드 도메인 차이로 발생한 Cookie 전달 문제를 HTTPS와 도메인 설정으로 해결
- 백엔드 개발 일정 관리 및 업무 배정

`Java` `Spring Boot` `Spring Security` `OAuth2` `JWT`
`JPA` `MySQL` `AWS` `GitHub Actions`

<br>

## 🎓 Education & Certificate

- **홍익대학교**
  - 기계·시스템디자인공학과
  - 컴퓨터공학과 복수전공
- **정보처리기사**
- **SQLD**

<br>

## 🏆 Awards

- 🥇 2024 기계·시스템디자인공학과 졸업논문 발표회 **대상**

<br>

## 🧩 Algorithm

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=dbsauddn1)](https://solved.ac/dbsauddn1/)
