# blurr : 함께 흐리고 다시 그리는 마음의 공간 
<p align="center">
  <img src="thumbnail.png" width="70%">
</p>


- 🫥 익명으로 이야기할 수 있어요.
- 🎧 실시간 음성 변조로 목소리를 보호할 수 있어요.
- 🤖 AI 사회자가 대화를 안전하게 이끌어줘요.
- 🚨 위험 신호를 자동으로 감지할 수 있어요.
- 🎭 AR 필터로 부담 없이 참여할 수 있어요.

## WHAT WE REDESIGNED

✔ **상담 접근 방식의 리디자인**
기존: 대면 상담 중심 → 비용, 낙인, 대기시간으로 진입 장벽 높음
Blurr: 메타버스 아바타 + 음성변조 + 익명성,
누구나 들어올 수 있는 저마찰 AI 기반 접근 구조로 재설계

✔ **상담 운영 구조의 리디자인**
기존: 상담자 중심으로 진행 → 인력 의존도 높고 확장 어려움
Blurr: AI 사회자가 발언 순서·시간·주제 진행을 자동 운영
→ 전문 인력 없이도 일관된 세션 품질 유지 + 확장 가능

✔ **정서 케어 플로우의 리디자인**
기존: 그룹 상담–개인 상담–기관 연계가 단절
Blurr: AI가 중간허브로 개입하여
그룹 지지 → 전문가 1:1 → 공공기관 링크로 이어지는
연속형 정서 지원 루프로 재설계

✔ **위험 탐지·위기 개입 구조의 리디자인**
기존: 위험 신호는 사람이 직접 봐야 감지 가능
Blurr: 한국어 기반 AI 위험 감지 모델(우울·자살 스코어링)이 실시간 STT를 분석해 즉각 위험도 판단
→ 개입 지연(TAT)을 획기적으로 축소

✔ **상담 기록·관리 방식의 리디자인**
기존: 상담사가 모든 기록을 작성 → 시간·비용 많이 듦
Blurr: GPT 기반 상담 기록 자동요약 → 상담사가 검수
→ 문서화 비용 절감 + 품질 일관성 확보


## ✨ Product Highlights
- AI 기반 익명 그룹 상담 플랫폼
  - 메타버스 아바타 + 실시간 음성 변조로 노출 걱정 없이 이야기할 수 있는 안전한 공간을 제공합니다.
- AI 사회자(Moderation Engine)
  - 발언 순서·시간·주제를 자동 관리하고 대화 흐름을 유지하는 AI 사회자가 세션 품질을 일정하게 보장합니다.
- 저마찰(Zero-friction) 정서 케어 루프
  - 익명 그룹 상담 → 1:1 전문가 매칭 → 위기 연결까지 한 앱 안에서 자연스럽게 이동할 수 있습니다.
- 한국어 기반 위기 감지 AI 탑재
  - 우울·자살 위험 점수를 실시간 산출하여 필요 시 서울시 자살예방센터(1393) 등 긴급기관 연결을 지원합니다.
- LiveKit / WebRTC 기반 초저지연 음성 세션
  - 다수 참여자의 음성을 안정적으로 동기화하고, DataChannel로 텍스트·이모티콘 반응까지 실시간 경험을 제공합니다.
- 온디바이스 안전성 강화
  - 위험 감지 모델(ONNX)을 로컬 실행해 네트워크와 무관하게 즉각적인 대응이 가능합니다.
- Flutter + Server-Driven Session Flow
  - 앱 단에서는 UI/로직을 단순화하고, 서버가 세션 상태(PREAMBLE → SPEAKING → INTERMISSION)를 권위적으로 동기화합니다.
 
## 🎬 시연 영상

[![Blurr Demo](thumbnail2.png)](https://youtu.be/f17hUKxD40I?si=QWGlzGnhmBqF4agV&t=48)

<p align="center">
  <a href="https://youtu.be/f17hUKxD40I?si=QWGlzGnhmBqF4agV&t=48">
    👉 동영상으로 시연 보기
  </a>
</p>

## 👥 팀원 소개

<div align="center">

| <img src="jiwon.jpg" width="120"> | <img src="hyeryeong.png" width="120"> | <img src="sooyoung.png" width="120"> |
|:----------------------------------:|:----------------------------------:|:----------------------------------:|
| [**황지원**](https://github.com/hwngjwn) | [**김혜령**](https://github.com/h-ye-ryoung) | [**최수영**](https://github.com/soo0choi) |
| 기획 · 디자인 · 프론트 |  백엔드 · 인프라 · 디자인 | 기획 · AI |
| ![Flutter](https://img.shields.io/badge/Flutter-3.24-blue) ![MLKit](https://img.shields.io/badge/MLKit-Face_Landmarks-yellow) | ![SpringBoot](https://img.shields.io/badge/SpringBoot-3.2-green) ![LiveKit](https://img.shields.io/badge/LiveKit-WebRTC-orange) | ![AI](https://img.shields.io/badge/AI-Suicide_Detection-red) |
</div>

## 기술 스택
```mermaid
flowchart TB

    classDef client fill:#A3D8FF,stroke:#1D75B3,stroke-width:1px,color:#000
    classDef server fill:#FFE1A8,stroke:#D9983D,stroke-width:1px,color:#000
    classDef media fill:#FFD1DC,stroke:#C96A7B,stroke-width:1px,color:#000
    classDef ai fill:#D3F8E2,stroke:#63B58F,stroke-width:1px,color:#000
    classDef db fill:#E6D4FF,stroke:#8B6AD8,stroke-width:1px,color:#000

    A["Flutter Client
• LiveKit/WebRTC
• ML Kit Face Landmarks
• AR Overlay
• ONNX Runtime"]:::client

    B["LiveKit / OpenVidu Server
• SFU Audio
• Voice Modulation
• DataChannel Sync"]:::media

    C["Spring Boot Backend
• Auth
• SSE Sync
• GPT Orchestration
• Risk Routing"]:::server

    D["AI Pipeline
• Whisper STT
• GPT Prompting
• KoAlpaca Fine-tuned Model
• Suicide/Depression Classifier"]:::ai

    E["RDS(MySQL)
• User States
• Session Logs
• Risk Events"]:::db

    A -->|"WebRTC(Audio/Metadata)"| B
    A -->|"HTTPS / SSE"| C
    B -->|"STT Input"| D
    C -->|"AI 요청"| D
    D -->|"결과 저장"| E
    C -->|"Session State Sync"| A







