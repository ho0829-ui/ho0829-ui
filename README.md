<p align="center">
  <img src="./assets/header.svg" alt="JAEHO - Building reliable AI systems, one step at a time. Fields: AI Systems, Cloud, Architecture." width="100%">
</p>

## TECH STACK

<p align="center">
  <img src="./assets/board.svg" alt="Tech stack board. USING: Python, Linux, Git, SQL, PyTorch. LEARNING: Docker, LLM, CS/Network. NEXT: AWS, RAG, Agent, Guardrails, Evals. LATER: Kubernetes, Architecture." width="100%">
</p>

<details>
<summary>텍스트로 보기</summary>

| 단계 | 기술 |
|:--|:--|
| 🟢 USING · 사용 중 | Python, Linux, Git, SQL, PyTorch |
| 🔵 LEARNING · 학습 중 | Docker, LLM, CS / Network |
| ⚪ NEXT · 다음 | AWS, RAG, Agent, Guardrails, Evals |
| ⚫ LATER · 이후 | Kubernetes, Architecture |

</details>

## PROJECTS

| # | 프로젝트 | 한 줄 요약 | 형태 | 상태 |
|:--:|:--|:--|:--:|:--:|
| 01 | KLUE-YNAT 뉴스 주제 분류 | Hugging Face 모델 파인튜닝 + AI 에이전트 실습 | 개인 | 🔵 진행 중 |
| 02 | 알라딘 도서 데이터 + TTS | 알라딘 API 도서 데이터 수집 → 저장 → 음성 변환 | 페어 | 🟢 완료 |
| 03 | 텍스트 이미지 VQA | SSAFY 16기 AI 챌린지, 한글 텍스트 이미지 4지선다 질의응답 | 팀 | 🟢 완료 |
| 04 | Docker 실습 | Docker 기초를 단계별로 실습하고 저장소로 정리 | 개인 | 🔵 진행 중 |
| 05 | 장애 대응 트러블슈팅 게임 | 장애 시나리오를 풀며 원인을 찾는 웹 시뮬레이션 | 개인 | ⚪ 계획 |
| 06 | 카드 할인·실적 관리 앱 | 카드별 할인 규칙과 전월 실적을 관리하는 Android 앱 | 개인 | ⚪ 계획 |

<details>
<summary><b>01 · KLUE-YNAT 뉴스 주제 분류</b></summary>

| 항목 | 내용 |
|:--|:--|
| 기간 | — |
| 형태 | 개인 |
| 기술 | Python, Hugging Face Transformers, PyTorch, Miniconda |
| 링크 | — |

**목표**
- 뉴스 제목을 7개 주제로 분류하는 모델을 직접 파인튜닝하고, 1주 안에 짧게 완주하기
- 모델 학습과 함께 AI 에이전트를 코딩 도우미로 쓰고, 직접 에이전트도 만들어 보기

**한 일 · 결정**
- 로컬 GPU(VRAM 16GB) Windows 환경에서 학습 환경 구성
- transformers v5에서 발생한 에러를 버전을 내리지 않고 하나씩 해결하는 방식 선택

**결과 · 배운 점**
- —

</details>

<details>
<summary><b>02 · 알라딘 도서 데이터 + TTS</b></summary>

| 항목 | 내용 |
|:--|:--|
| 기간 | — |
| 형태 | 2인 페어 프로그래밍 |
| 기술 | Python, REST API, JSON, gTTS |
| 링크 | — |

**목표**
- 알라딘 API로 도서 데이터를 수집해 파일로 저장하고 음성으로 변환하기

**한 일 · 결정**
- 도서 데이터 수집 → JSON / txt 저장 → gTTS 음성 변환 과제(A, B 그룹) 완료
- 역할을 나눈 페어 프로그래밍으로 시작해, 서로 토론하며 구현하는 방식으로 진행

**결과 · 배운 점**
- —

</details>

<details>
<summary><b>03 · 텍스트 이미지 VQA (SSAFY 16기 AI 챌린지)</b></summary>

| 항목 | 내용 |
|:--|:--|
| 기간 | — |
| 형태 | 팀 |
| 역할 | — |
| 기술 | Python, PyTorch, Qwen 멀티모달 모델, LoRA |
| 링크 | — |

**문제**
- 이미지 1장 + 질문 + 4개 선지 중 정답 1개를 고르는 VQA. 한글 팻말·메뉴판 텍스트를 읽어야 하는 문제 포함
- 외부 API 추론 금지, train / test 각 6,714장

**한 일 · 결정**
- 객체 탐지(YOLO) 없이 멀티모달 모델 단독 파이프라인으로 설계
- 답변 생성 후 파싱 대신 a/b/c/d 첫 토큰 logits를 비교하고, 표면형 변형은 logsumexp로 합산
- zero-shot 베이스라인 → LoRA 파인튜닝 → 앙상블·캘리브레이션 순서로 진행
- 팀원은 로컬 RTX 5060 Ti로 실험하고, 팀장이 Colab H100에서 테스트하는 방식으로 컴퓨팅 분담

**결과 · 배운 점**
- —

</details>

<details>
<summary><b>04 · Docker 실습</b></summary>

| 항목 | 내용 |
|:--|:--|
| 기간 | — |
| 형태 | 개인 |
| 기술 | Docker, Linux, Git |
| 링크 | — |

**목표**
- Docker를 기초부터 단계별로 실습하고, 실습 내용을 Git 저장소로 정리하기

**진행 상황**
- —

</details>

<details>
<summary><b>05 · 장애 대응 트러블슈팅 게임</b></summary>

| 항목 | 내용 |
|:--|:--|
| 형태 | 개인 |
| 기술 | 웹(브라우저 가짜 터미널), Claude Code |
| 상태 | 계획 |

**목표**
- 장애를 일부러 만들고 원인을 찾는 연습을 게임 형태로 만들기 (학습 · 스터디 공유 · 포트폴리오)

**설계 결정**
- 실제 시스템이 아닌 웹 시뮬레이션으로 구현
- 장애 분야: 리눅스 서버 기초, 네트워크, 웹서버/DB, 클라우드(AWS)
- 고정 시나리오로 시작 (실행 중 LLM 호출 없음)

</details>

<details>
<summary><b>06 · 카드 할인·실적 관리 앱</b></summary>

| 항목 | 내용 |
|:--|:--|
| 형태 | 개인 |
| 기술 | Kotlin, Jetpack Compose, (백엔드) 맥미니 → 클라우드 |
| 상태 | 설계 중 |

**문제**
- 여러 카드의 전월 실적 조건과 할인 한도가 각각 달라, 혜택을 최대로 받으려면 카드별로 따로 관리해야 함

**설계 결정**
- 카드별 할인 규칙 저장, 사용 금액 입력 시 예상 할인액과 한도 소진 여부 안내
- 결제·취소는 직접 입력으로 시작하고, 알림 자동 처리는 단계적으로 추가
- 백엔드는 맥미니에 먼저 구축한 뒤 클라우드로 이전

</details>

## CERTIFICATIONS

- 리눅스마스터 2급
- SQLD
- ADsP

<details>
<summary><b>ROADMAP</b> — 전체 로드맵 펼치기</summary>

```text
2026
│
├── Foundation
│   ├── CS
│   ├── Network
│   └── Linux
│
├── AI Application
│   ├── LLM API
│   ├── RAG
│   └── Tool Calling
│
├── AI Systems
│   ├── Agent
│   ├── Harness
│   ├── Guardrails
│   └── Evals
│
└── Infrastructure
    ├── Docker
    ├── AWS
    └── Kubernetes
```

</details>
