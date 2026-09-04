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

- **메인 메뉴 → 캠프(잠수함 허브) → 인게임 레벨 전환 플로우 구성**
  단계별 GameMode와 GameState를 분리하고, Listen Server 환경에서 맵 전환 이후에도
  게임 상태와 플레이어 상태가 이어지도록 구현
- GameInstance, GameMode, GameState, PlayerState, PlayerController 기반 멀티플레이 Gameplay Framework 구조 구현
- **Advanced Sessions 플러그인을 활용한 Steam 세션 생성·검색·참가 기능 구현**
  세션 생성, 세션 목록 조회, 개별 세션 참가까지의 흐름을 UI와 함께 구성
- 메인 메뉴 및 일시정지 UI 구성 및 구현
- Async Loading Screen 플러그인을 활용한 세션 전환 로딩 화면 구현
- G-Star 시연 버전까지 기능 개선 및 안정화

<br>

## 주요 파일

### Gameplay Framework

| 파일 | 역할 |
| --- | --- |
| `ADGameInstance` | 맵 전환에도 유지되어야 하는 데이터 보관 |
| `MainMenuGameMode` / `MainMenuPlayerController` | 메인 메뉴 레벨 규칙 및 입력 처리 |
| `ADCampGameMode` | 캠프(잠수함 허브) 레벨 규칙 처리 |
| `ADInGameMode` / `ADInGameState` | 인게임 진행 규칙 처리 및 매치 단위 상태 관리 |
| `ADPlayerController` | 입력 처리 및 UI 연결 |
| `ADPlayerState` | 플레이어별 데이터 보관 |

### UI

| 파일 | 역할 |
| --- | --- |
| `MainMenuWidget` | 메인 메뉴 화면 |
| `CreateTeamWidget` | 세션 생성 및 방 설정 |
| `SessionListWidget` | 검색된 세션 목록 표시 |
| `SessionEntryWidget` | 세션 목록의 개별 항목. 선택 시 참가 처리 |
| `PauseWidget` | 일시정지 화면 |

