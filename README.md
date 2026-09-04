# AbyssDiver_Portfolio
UE5 Gameplay Framework Portfolio

Unreal Engine 5 팀 프로젝트에서 제가 담당한 Gameplay Framework 및 멀티플레이 접속 플로우 소스를 정리한 저장소입니다.

참고 — 포트폴리오 목적으로 본인이 작성한 소스만 발췌했습니다. 빌드 가능한 전체 프로젝트가 아니며, 에셋과 바이너리는 포함되어 있지 않습니다.

기술 스택  C++ · Unreal Engine 5 · Blueprint · Listen Server · Replication · RPC · Git/GitHub

<br>
1. Abyss Diver : Underworld

심해를 배경으로 한 최대 4인 멀티플레이 협동 호러 서바이벌 게임 10인 팀 · 2개월 · 2025.05 ~ 2025.11

부트캠프 최우수상 수상 · 2025 G-Star 시연 관람객 118명 설문에서 만족도 4점 이상 63.6%, 난이도 긍정 평가 89.8%

담당 — Gameplay Framework 및 멀티플레이 접속 플로우

-GameInstance, GameMode, GameState, PlayerState, PlayerController 기반 멀티플레이 Gameplay Framework 구조 구현 
-로비 → 인게임 전환 플로우 구성. Listen Server 환경에서 맵 전환 이후에도 게임 상태와 플레이어 상태가 유지되도록 처리
-Advanced Sessions 플러그인을 활용한 Steam 세션 생성·검색·참가 기능 구현
-Async Loading Screen 플러그인을 활용한 세션 전환 로딩 화면 구현
-MainMenu UI 구성 및 구현
-G-Star 시연 버전까지 기능 개선 및 안정화





<br>
