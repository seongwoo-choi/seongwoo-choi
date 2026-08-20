# 최성우 · Seongwoo Choi

**Platform Engineer — Observability** · Seoul

무신사 Service Platform에서 사내 관측 가능성(Observability) 플랫폼을 만들고 운영합니다.
멀티 클러스터 Kubernetes 환경의 로그·메트릭·트레이스를 수집부터 저장·쿼리·알림까지 책임집니다.

---

### 하는 일

**Observability 플랫폼 운영**
- Grafana · Loki · Mimir · Tempo · Alloy · OpenTelemetry Collector 기반 멀티테넌트 스택
- 여러 EKS 클러스터의 수집 파이프라인 설계, 테넌트 격리, 저장소·쿼리 튜닝

**로그 파이프라인 이관 — MSK → Confluent Cloud**
- 무중단 이관을 위한 dual-write · 컷오버 표준 프로세스 설계
- 유실 0 을 증명하는 정합성 검증 게이트 구축

**용량 · 비용 최적화**
- 카디널리티 감사, retention 정책 재설계, 트래픽 경로 변경
- 절감액을 볼륨 효과와 토폴로지 효과로 분해해 귀속까지 검증

**인시던트 대응**
- 프로덕션 장애의 근본 원인을 실측으로 규명
- 재발 차단을 자동 검증(preflight)과 문서화된 교훈으로 영속화

---

### 기술

`Kubernetes` `AWS (EKS · EC2 · MSK)` `Terraform` `ArgoCD` `Helm` `Istio`
`Go` `Kotlin` `Kafka` `Grafana Stack (Loki · Mimir · Tempo)` `OpenTelemetry` `Datadog`

---

### 프로젝트

**[node-drain](https://github.com/seongwoo-choi/node-drain)** · Go

Karpenter 가 관리하는 NodePool 의 워크로드 노드를 안전하게 비우고 교체하는 CLI 입니다.
Prometheus / Mimir 메트릭으로 NodePool 사용률을 산출해 동시 드레인 대수를 계산하고,
cordon → 파드 제거 → 종료 대기 순으로 처리합니다. PDB 차단 요인과 파드 위험도를 사전 분석하는
`analyze` 명령, 멀티테넌트 Prometheus 지원, Slack 알림을 포함합니다.

---

### 글

[ssunw.tistory.com](https://ssunw.tistory.com/)

### 연락

[LinkedIn](https://www.linkedin.com/in/seongwoo-choi/) · hibogo789@gmail.com
