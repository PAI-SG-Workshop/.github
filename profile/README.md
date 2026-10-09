# PAI-SG Workshop | Physical AI Spider Grid

**Reproducible implementation, practical experimentation, and hardware-connected validation for Physical AI.**

**재현 가능한 구현, 실용적인 실험, 실제 하드웨어 연동 검증을 위한 Physical AI Spider Grid 작업 공간입니다.**

[PAI-SG Foundation](https://github.com/PAI-SG-Foundation) · [PAI-SG Library](https://github.com/PAI-SG-Library) · [PAI-SG Workshop](https://github.com/PAI-SG-Workshop) · [PAI-SG Guild](https://github.com/PAI-SG-Guild) · [PAI-SG Research](https://github.com/PAI-SG-Research) · [PAI-SG Standards](https://github.com/PAI-SG-Standards)

---

## English

### Mission

PAI-SG Workshop is the implementation and experimentation working group within **Physical AI Spider Grid (PAI-SG)**. It connects algorithms, datasets, simulation, software interfaces, and physical platforms so that technical ideas can be tested, reproduced, compared, and eventually integrated into real robotic systems. The Workshop emphasizes executable evidence rather than claims based solely on documentation or demonstrations.

The Workshop is part of a six-group collaboration structure. It does not claim that every algorithm or hardware integration described here has already been implemented or validated. Repository-specific documentation, tests, and results are the authoritative evidence for implementation status.

### Scope of work

**Perception and scene understanding.** Develop and evaluate components for image classification, object detection, instance and semantic segmentation, multi-object tracking, depth and 3D perception, and video-based scene understanding. Compare architectures using explicit datasets, metrics, and runtime conditions.

**Physical state and temporal understanding.** Investigate object identities, trajectories, motion cues, spatial relations, and time-dependent observations that can support state estimation and downstream Physical AI reasoning. Keep observed measurements distinct from inferred states and predictions.

**Robot and sensor integration.** Build reference integrations for cameras, mobile robots, AMRs, AGVs, and other supported platforms. Where appropriate, use established robotics middleware and existing device SDKs instead of rebuilding mature low-level control stacks. Document safety boundaries and hardware assumptions.

**Experiment and benchmark engineering.** Prepare reproducible training and evaluation scripts, dataset adapters, baseline configurations, environment specifications, inference benchmarks, and regression tests. Record dataset provenance, licensing constraints, hardware, software versions, random seeds, and known limitations when applicable.

**Simulation-to-field validation.** Use simulation and controlled experiments to reduce integration risk before physical trials. Treat simulated success, laboratory verification, and field validation as separate evidence levels.

### Working principles

1. **Reproducibility:** A published result should identify the code revision, dependencies, input data, configuration, and evaluation method needed to reproduce it.
2. **Modularity:** Components should expose clear inputs, outputs, units, coordinate frames, and failure behavior so they can be replaced or compared independently.
3. **Evidence and traceability:** Link implementations to requirements, experiments, benchmark results, and relevant standards where possible.
4. **Safety and scope:** AI perception and planning experiments must not be represented as safety-certified robot control. Real-world deployments require separate engineering review and validation.
5. **Responsible publication:** Share approved public examples and derived results without exposing confidential designs, raw private evidence, supplier arrangements, credentials, or proprietary datasets.

### Example deliverables

The Workshop may publish reference implementations, experiment notebooks, reproducibility instructions, synthetic-data generators, dataset conversion tools, benchmark reports, interface examples, simulation scenarios, and integration tutorials. These are prospective categories, not a statement that every deliverable is currently available.

### Relationship to Statera Workshop

[Statera-Workshop](https://github.com/Statera-Workshop) is the corresponding Statera implementation working group. PAI-SG Workshop presents and organizes approved implementation materials for the Physical AI Spider Grid context. Source ownership, provenance, and synchronization should remain explicit; publication in PAI-SG does not imply that private Statera materials are automatically public.

### The six PAI-SG working groups

| Working group | Responsibility | GitHub |
| --- | --- | --- |
| **Foundation** | Mission, principles, governance, and stewardship | [PAI-SG-Foundation](https://github.com/PAI-SG-Foundation) |
| **Library** | Structured technical knowledge, learning resources, and reference materials | [PAI-SG-Library](https://github.com/PAI-SG-Library) |
| **Workshop** | Executable implementations, experiments, and engineering validation | [PAI-SG-Workshop](https://github.com/PAI-SG-Workshop) |
| **Guild** | Contributor collaboration, domain roles, and evidence-based contributions | [PAI-SG-Guild](https://github.com/PAI-SG-Guild) |
| **Research** | Research questions, hypotheses, experimental methods, and new approaches | [PAI-SG-Research](https://github.com/PAI-SG-Research) |
| **Standards** | Common schemas, interfaces, interoperability, and specification governance | [PAI-SG-Standards](https://github.com/PAI-SG-Standards) |

### Statera counterpart organizations

[Statera-Foundation](https://github.com/Statera-Foundation) · [Statera-Library](https://github.com/Statera-Library) · [Statera-Workshop](https://github.com/Statera-Workshop) · [Statera-Guild](https://github.com/Statera-Guild) · [Statera-Research](https://github.com/Statera-Research) · [Statera-Standards](https://github.com/Statera-Standards)

---

## 한국어

### 목적과 역할

**PAI-SG Workshop**은 **Physical AI Spider Grid(PAI-SG)**의 알고리즘 구현과 실험을 담당하는 작업 그룹(Working Group)입니다. 인공지능 알고리즘, 데이터셋, 시뮬레이션, 소프트웨어 인터페이스, 실제 로봇 플랫폼을 연결하여 기술을 재현하고 비교하며 검증할 수 있는 기반을 구축하는 것을 목표로 합니다. 단순한 개념 설명보다 실행 가능한 코드와 측정 가능한 검증 증거를 중요하게 다룹니다.

Workshop은 여섯 개 작업 그룹으로 구성된 협업 체계의 일부입니다. 여기에서 소개하는 모든 알고리즘이나 하드웨어 연동이 이미 구현되거나 검증되었다는 의미는 아닙니다. 실제 구현 상태는 개별 Repository의 코드, 시험 기록 및 결과를 기준으로 판단해야 합니다.

### 주요 기술 영역

**인지 및 장면 이해(Perception and Scene Understanding).** 이미지 분류(Image Classification), 객체 감지(Object Detection), 의미론적 분할(Semantic Segmentation), 인스턴스 분할(Instance Segmentation), 다중 객체 추적(Multi-Object Tracking), 깊이 및 3차원 인지(3D Perception), 비디오 기반 장면 이해(Video Understanding) 등을 구현하고 평가합니다. 비교 시 데이터셋, 정확도 지표, 실행 환경을 명시합니다.

**물리 상태와 시간적 이해(Physical State and Temporal Understanding).** 객체의 식별 정보, 이동 궤적, 움직임 특징, 공간적 관계, 시간에 따른 관측을 연결하여 물리 상태 추정과 후속 추론에 활용할 수 있는 기술을 다룹니다. 센서에서 직접 관측한 정보와 추론 또는 예측한 상태를 구분합니다.

**로봇 및 센서 연동(Robot and Sensor Integration).** 카메라, 자율이동로봇(AMR), 무인운반차(AGV) 및 기타 지원 플랫폼과의 인터페이스 구현을 검토합니다. 성숙한 장치 제어 기능은 기존 SDK와 로봇 미들웨어를 활용하고, AI 모듈과 장치 제어 계층 사이의 책임과 안전 경계를 명확히 합니다.

**실험 및 벤치마크(Experiment and Benchmark Engineering).** 학습·평가 스크립트, 데이터셋 어댑터, 기준 모델(Baseline), 환경 설정, 추론 속도 측정, 회귀 시험 등을 체계화합니다. 필요한 경우 데이터 출처, 라이선스, 하드웨어 사양, 소프트웨어 버전, 난수 시드 및 알려진 제약을 기록합니다.

**시뮬레이션과 현장 검증(Simulation-to-Field Validation).** 시뮬레이션과 통제된 실험으로 위험을 줄인 후 실제 로봇 환경으로 확장하는 접근을 지향합니다. 시뮬레이션 성공, 실험실 검증, 현장 검증은 서로 다른 증거 수준으로 관리합니다.

### 운영 원칙

1. **재현성(Reproducibility):** 코드 버전, 의존성, 입력 데이터, 실행 설정 및 평가 방법을 추적할 수 있도록 합니다.
2. **모듈성(Modularity):** 입력·출력, 단위, 좌표계 및 오류 처리 방식을 명확히 하여 구성 요소를 독립적으로 교체하거나 비교할 수 있게 합니다.
3. **증거와 추적성(Evidence and Traceability):** 구현 결과를 요구사항, 실험 기록, 벤치마크 및 관련 표준과 연결합니다.
4. **안전과 적용 범위(Safety and Scope):** 인지·계획 알고리즘의 시험 결과를 안전 인증된 로봇 제어 기능으로 혼동하지 않습니다. 실제 현장 적용에는 별도의 공학적 검토와 검증이 필요합니다.
5. **책임 있는 공개(Responsible Publication):** 공개 승인을 받은 예제와 파생 결과를 공유하며, 비공개 설계·원본 증거·공급사 계약 정보·인증 정보·독점 데이터셋은 임의로 공개하지 않습니다.

### 주요 산출물

Workshop의 산출물은 참조 구현(Reference Implementation), 실험용 Notebook, 재현 절차, 합성 데이터 생성기, 데이터 변환 도구, 벤치마크 보고서, 인터페이스 예제, 시뮬레이션 시나리오 및 통합 튜토리얼 등을 포함할 수 있습니다. 이는 추진 가능한 산출물의 유형이며, 모든 항목이 현재 공개되어 있다는 뜻은 아닙니다.

### Statera-Workshop과의 관계

[Statera-Workshop](https://github.com/Statera-Workshop)은 대응하는 Statera 구현 작업 그룹입니다. PAI-SG Workshop은 Physical AI Spider Grid의 목적에 적합한 **공개 승인 자료**를 구성하고 소개합니다. 원본의 소유권, 출처, 변경 이력 및 동기화 관계를 명확히 관리하며, Statera의 비공개 자료가 자동으로 PAI-SG에 공개되는 것은 아닙니다.

### PAI-SG의 여섯 개 작업 그룹

| 작업 그룹 | 주요 역할 | GitHub |
| --- | --- | --- |
| **Foundation** | 비전, 기본 원칙, 거버넌스 및 운영 방향 | [PAI-SG-Foundation](https://github.com/PAI-SG-Foundation) |
| **Library** | 기술 지식, 학습 자료, 참조 문서의 체계화 | [PAI-SG-Library](https://github.com/PAI-SG-Library) |
| **Workshop** | 실행 코드, 실험, 엔지니어링 검증 | [PAI-SG-Workshop](https://github.com/PAI-SG-Workshop) |
| **Guild** | 기여자 협업, 분야별 역할, 증거 기반 기여 기록 | [PAI-SG-Guild](https://github.com/PAI-SG-Guild) |
| **Research** | 연구 가설, 실험 방법, 새로운 알고리즘 탐색 | [PAI-SG-Research](https://github.com/PAI-SG-Research) |
| **Standards** | 공통 스키마, 인터페이스, 상호운용성 및 표준 관리 | [PAI-SG-Standards](https://github.com/PAI-SG-Standards) |

### Statera 대응 조직

[Statera-Foundation](https://github.com/Statera-Foundation) · [Statera-Library](https://github.com/Statera-Library) · [Statera-Workshop](https://github.com/Statera-Workshop) · [Statera-Guild](https://github.com/Statera-Guild) · [Statera-Research](https://github.com/Statera-Research) · [Statera-Standards](https://github.com/Statera-Standards)

---

## Contact

**Richard Minsoo Go**  
Head of AI, Hills Robotics  
Statera Working Group

**Personal / Research Contact:**  
[gominsoo888@gmail.com](mailto:gominsoo888@gmail.com)

**Hills Robotics / Business Contact:**  
[minsoo.go@hillslogis.com](mailto:minsoo.go@hillslogis.com)

---

*PAI-SG Workshop — Turning Physical AI knowledge into reproducible engineering evidence.*
