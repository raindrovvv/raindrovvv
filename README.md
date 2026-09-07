# Jungmin Cha 👋
**Game Builder - Game Programmer** 
vnrs97@gmail.com

사운드를 만드는 사람에서 시작해, 클라이언트 작업까지 합니다.  
음악 프로듀싱이 주특기였고, 지금은 그 감각과 창의력을 **게임**으로 옮기고 있습니다.

전공 프로그래머는 아니지만 필요한 구현은 AI로 빠르게 만든 뒤, **인게임에서 직접 확인하고 고칩니다.**

`UE5` `Wwise` `C++ / Blueprint` `Git` `FL Studio` `MCP` `AI Agents`

---

## 어떻게 만드나

1. 플레이 문제부터 정함  
   (예: 소리로 공간이 안 갈린다, 전투 상태가 안 읽힌다)
2. 사운드/로직 구조를 먼저 그림  
   (Event, State, Switch, 컴포넌트 책임)
3. C++/BP 초안은 Codex · Claude Code · Cursor로 뽑음
4. 에디터·플레이테스트에서 재현하고, 틀린 구현은 버리거나 고침
5. 구현 방법·QA를 팀원 또는 에이전트가 이어서 쓸 수 있게 문서로 정리

관련 글  
- [AI를 Unreal Editor 안으로: UnrealAgent](https://raindrovvv.tistory.com)  
- [1인 개발자가 팀 단위 속도를 내는 법](https://raindrovvv.tistory.com)  
- [미니맵 DX12 / GPU 크래시 디버깅](https://raindrovvv.tistory.com)

---

## Featured

### Guardian & Seeker — G-STAR 2025 / 인디 팀 진행 중
4v1 비대칭 PvP · Unreal Engine 5.4 → 5.6  
**Greed Fennec Studio** · **부팀장** · 게임 오디오 디자이너 · 클라이언트 개발자(빌더)

2025년 5월부터 **1년째** 팀을 유지하며 만들어 가고 있습니다.  
G-STAR 2025 출품 이후에도 인디 타이틀로 개발을 이어가는 중입니다.

- G-STAR 전시 플레이테스트 **299명**, 만족도 **4.36 / 5**

한 일
- `UGS_AudioComponentBase` 기준으로 Monster / Seeker / UI 책임 분리
- 전투 State → Wwise BGM 전환 (사운드만으로 교전 여부 인지)
- Physical Material + Switch 발소리 (흙 · 돌 · 물 · 용암 · 금속)
- Occlusion: 벽/문 너머 소리가 그대로 들리던 문제를  
  Line Trace · Collision · Wwise Occlusion으로 재현 가능한 구조로 수정
- 팀용 오디오 네이밍 컨벤션 배포 (`EV_Mon_NeedleFang_Attack`)


- 코드: [Sound 시스템](https://github.com/raindrovvv/GuardianAndSeeker/tree/Dev/Source/GAS/Public/Sound)
- 플레이: [Demo](https://www.youtube.com/watch?v=MGSCKdCAgDY)
- 시스템 시연: [Audio](https://www.youtube.com/watch?v=d7xon5fv-kg)

### UnrealAgent
언리얼 에디터 안에서 쓰는 로컬 AI 에이전트.

왜 만들었나  
에디터 작업과 코드 초안을 오갈 때마다 컨텍스트가 끊기는 게 병목이었습니다.

무엇을 하나
- 에디터 상태 조회, 액터/애셋/BP/UMG 조작, 뷰포트 캡처, 로그 확인
- MCP로 도구를 고정해서, AI가 임의로 파일을 못 건드치게 함
- loopback only. 생성은 에이전트, 적용 여부는 사람

- 코드: [UnrealAgent](https://github.com/raindrovvv/UnrealAgent)

### 생산성 툴 / 진행 중
- [Unreal-Engine-Build-Monitor](https://github.com/raindrovvv/Unreal-Engine-Build-Monitor) — 빌드 상태를 웹으로 확인
- [UnityMCP](https://github.com/raindrovvv/UnityMCP) — Unity 에디터 ↔ 로컬 에이전트
- MapleStory Worlds로 2인 팀 게임 제작 중

[Game Portfolio](https://jungmin-cha-portfolio.pages.dev/) · [AI Builder Portfolio](https://jungmin-cha-ai-builder.pages.dev) · [AI Video Portfolio](https://jungmin-cha-ai-video.pages.dev)

---

<details>
<summary>English</summary>

Game audio designer and technical builder.  
Vice team lead on the indie title Guardian & Seeker (4v1 PvP, UE5), in development since May 2025, shown at G-STAR 2025.

I prototype C++/Blueprint with AI agents, then verify and fix everything in play.  
Not a CS-first programmer — I build, debug, and ship the audio systems the game actually needs.

</details>
