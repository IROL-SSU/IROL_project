# IROL Project

접촉이 많은 복잡한 환경에서 자연어로 지정된 물체를 안전하게 탐색하고 파지하기 위한 IROL 연구 프로젝트입니다.

이 저장소는 연구 문서와 관련 구현 저장소를 한곳에서 관리합니다.

## 구성

| 경로 | 설명 |
|---|---|
| [`irol/`](irol/) | VLA–DRL 기반 contact-rich manipulation 연구 문서와 로드맵 |
| [`Contact-Rich-Manipulation-v2/`](Contact-Rich-Manipulation-v2/) | Contact-rich manipulation 구현 (submodule) |
| [`2D-PDM_DINOv3_SigLIP/`](2D-PDM_DINOv3_SigLIP/) | DINOv3·SigLIP 기반 2D probability distribution mapping 구현 (submodule) |

## 시작하기

서브모듈을 포함해 저장소를 복제합니다.

```bash
git clone --recurse-submodules https://github.com/IROL-SSU/IROL_project.git
```

이미 저장소를 복제했다면 다음 명령으로 서브모듈을 초기화합니다.

```bash
git submodule update --init --recursive
```

자세한 연구 방향과 각 프로젝트의 사용 방법은 [`irol/README.md`](irol/README.md) 및 각 서브모듈의 README를 참고하세요.
