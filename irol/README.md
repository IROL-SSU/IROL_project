# IROL — VLA-DRL Hybrid Contact-Rich Manipulation

목표 물체가 주변 물체에 인접하거나 부분적으로 가려진 선반 환경에서, **자연어로 지정된 목표 물체를 주변 물체를 넘어뜨리지 않고 파지**하는 시스템 연구.

Frozen VLA + 저차원 인터페이스 + F/T 기반 단일 DRL 정책으로 구성하며, 대규모 컴퓨팅 없이(GPU 2대) 달성하는 것을 전제로 한다.

## 문서

| 문서 | 내용 |
|---|---|
| **[research_roadmap.md](research_roadmap.md)** | ⚠ 2026-08 사본. 최신 로드맵은 [contact-manipulation-research/roadmap](https://github.com/dhlee04/contact-manipulation-research/tree/main/roadmap) — 최종 아키텍처(Step-5), 기존 top-tier 연구 대비 기여도 분석(pros/cons), Step-1~5 단계별 로드맵, 2년 실행 계획 |
| **[adaptive_executor_routing_protocol.md](adaptive_executor_routing_protocol.md)** | VLM subtask와 RGB-D fused payload를 기반으로 Motion Planning·VLA·DRL 실행기를 선택하는 adaptive routing 프로토콜 |
| **[global_to_local_target_centric_perception.md](global_to_local_target_centric_perception.md)** | Global semantic perception에서 target-centric local 3D occupancy mapping과 closed-loop manipulation decision으로 이어지는 프레임워크 |
| **[topics/](topics/README.md)** | 연구원 배정용 주제 제안·실행 계획 (리비전 관리 문서). 첫 문서: 석사 하위단 강화학습 주제 2건 |

## 빠른 요약

- **최종 목표**: Step-5 — iterative handoff 구조로 다중장애물·부분관측 시나리오에서 파지 수행
- **핵심 설계**: VLA는 얼리고, 학습이 필요한 컴포넌트는 **DRL 접촉 정책 하나뿐**
- **기간**: 2026 H2 ~ 2028 H1
