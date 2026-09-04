# Abyss Diver : Underworld — Gameplay Framework

심해를 배경으로 한 **최대 4인 멀티플레이 협동 호러 서바이벌 게임**에서
제가 담당한 Gameplay Framework 및 멀티플레이 접속 플로우 소스입니다.

> **참고** — 포트폴리오 목적으로 본인이 작성한 소스만 발췌했습니다.
> 빌드 가능한 전체 프로젝트가 아니며, 에셋과 바이너리는 포함되어 있지 않습니다.

<br>

## 프로젝트 개요

| | |
| --- | --- |
| **기간** | 2025.05 ~ 2025.11 (개발 2개월 + G-Star 시연 준비) |
| **팀 규모** | 10인 |
| **엔진** | Unreal Engine 5 |
| **네트워크** | Listen Server |
| **성과** | 부트캠프 최우수상 수상 · 2025 G-Star 시연 |

G-Star 시연에서 관람객 118명 대상 설문 결과, 만족도 4점 이상 63.6%,
난이도 항목 긍정 평가 89.8%를 기록했습니다.

**기술 스택** &nbsp;C++ · Unreal Engine 5 · Blueprint · Listen Server · Replication

<br>

## 담당 업무

- GameInstance, GameMode, GameState, PlayerState, PlayerController 기반 멀티플레이 Gameplay Framework 구조 구현
- 로비 → 인게임 전환 플로우 구성. Listen Server 환경에서 맵 전환 이후에도 게임 상태와 플레이어 상태가 유지되도록 처리
- Advanced Sessions 플러그인을 활용한 Steam 세션 생성·검색·참가 기능 구현
- Async Loading Screen 플러그인을 활용한 세션 전환 로딩 화면 구현
- MainMenu UI 구성 및 구현
- G-Star 시연 버전까지 기능 개선 및 안정화

<br>

## 주요 파일

| 파일 | 역할 |
| --- | --- |
| `파일명.h/.cpp` | 한 줄 설명 |
| `파일명.h/.cpp` | 한 줄 설명 |
| `파일명.h/.cpp` | 한 줄 설명 |
