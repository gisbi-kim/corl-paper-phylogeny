# CoRL Paper Phylogeny

**CoRL 2020–2025 (1,254 papers) — 17 Phylum × 127 Class × 246 Order semantic phylogeny**

👉 **[Live demo → gisbi-kim.github.io/corl-paper-phylogeny](https://gisbi-kim.github.io/corl-paper-phylogeny/)**

---

## 무엇인가

CoRL(Conference on Robot Learning) 2020–2025에 발표된 논문 1,254편 전체를  
**학습 패러다임(Learning Paradigm)** 을 Phylum 축으로 삼는 4-depth 시맨틱 계통도로 분류한 싱글-파일 인터랙티브 대시보드.

일반 로보틱스 학회(T-RO/IJRR/RSS) phylogeny([robotics-paper-phylogeny](https://github.com/gisbi-kim/robotics-paper-phylogeny))와 달리 **"무엇을 연구하는가(분야)"가 아니라 "어떻게 학습하는가(패러다임)"를 Phylum**으로 잡는다.  
CoRL 어휘에서 `learning` 단어가 529회로 압도적 1위라는 사실이 이 선택을 강제한다.

## 분류 구조

| 레벨 | 수 | 예시 |
|---|---|---|
| **Phylum** (L1) | 17 | Foundation Policies, Generative Policies, Imitation & Demo, RL … |
| **Class** (L2) | 127 | VLA Models, Diffusion Policies, Behavior Cloning, Legged Locomotion … |
| **Order** (L3) | 246 | Manipulation VLA, 6-DoF Grasp Detection, Cloth Folding … |
| **Leaf** (논문) | 1,254 | 실제 논문 제목 1편 1편 |

## 기능

| 탭 | 내용 |
|---|---|
| **🌳 Full Tree & Listing** | D3 인터랙티브 트리 (Phylum → Class → Order → 논문 제목까지 펼치기) + 노드 클릭 시 설명 & 논문 목록 사이드패널 + Phylum별 전체 일람(모두 펼치기/접기) + ASCII Tree / ASCII Tree+설명 / Mermaid source |
| **📊 EDA Charts** | Phylum × 연도 Stack chart · Sunburst · 3년 성장률 bar · 신생 카테고리 표 |

## 핵심 시그널 (2020 → 2025)

- **Foundation Policies** : 0편 → 28편 (+4,100%) — 2023년 첫 등장, 2년 만에 SOTA 점령
- **Generative Policies** : 2편 → 22편 (+1,700%) — Diffusion → Flow Matching으로 sub-paradigm 진화 중
- **Embodiment-Specific** : 6편 → 26편 (+220%) — Humanoid Whole-Body Control 2024년 폭발
- **RL** : 23편 → 18편 (−10%), **Control & MPC** : 11편 → 4편 (−42%) — 명시적 제어 이론이 학습된 정책에 흡수

## 방법론

- **제목 기반 분류** — abstract 없이 제목만으로 hierarchical regex + semantic synonym clustering
- **우선순위 규칙** — TAXONOMY 순서가 우선 (Foundation > Manipulation: "VLA-based manipulation"은 Foundation으로)
- **4-depth 완결** — 모든 논문이 정확히 하나의 (Phylum, Class, Order, Paper) 4-tuple에 속함
- **Unclassified** 130편 (10.4%) — 별도 카테고리로 명시 (정보 손실 아님)

참조: [robotics-paper-phylogeny](https://github.com/gisbi-kim/robotics-paper-phylogeny)의 4-depth semantic synonym clustering 사고방식 적용.

## 관련 프로젝트

| 리포 | 대상 |
|---|---|
| [robotics-paper-phylogeny](https://github.com/gisbi-kim/robotics-paper-phylogeny) | T-RO / IJRR / RSS (7,477편) |
| [cvml-paper-phylogeny](https://github.com/gisbi-kim/cvml-paper-phylogeny) | CVPR / ECCV / NeurIPS 외 (112k편) |
| **corl-paper-phylogeny** (이 리포) | CoRL 2020–2025 (1,254편) |
