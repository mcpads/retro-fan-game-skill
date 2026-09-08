# Retro Fan Game Skills

[English](README.md) | 한국어

좋아하는 레트로 게임을 고쳐 직접 플레이하려는 사람들을 위한 AI 스킬 모음입니다. 이야기, 그림, 규칙을 바꾸는 작업을 다룹니다. 스킬은 AI 에이전트가 작업할 때 참고하는 지침과 문서입니다.

만들고 싶은 게임의 모습은 사람이 정합니다. AI는 게임 구조를 조사하고 수정 방법을 찾아 구현합니다. 나온 결과가 원하는 분위기인지, 캐릭터가 그런 말을 할 법한지, 어떤 불편은 받아들일 수 있는지는 사람이 판단합니다.

## 들어 있는 스킬

| 스킬 | 쓰임 |
| --- | --- |
| [create-retro-fan-game](skills/create-retro-fan-game/SKILL.md) | 만들고 싶은 게임을 정하고 원본 조사부터 수정·실행 확인까지 작업을 이어갑니다. |
| [adapt-retro-game-narrative](skills/adapt-retro-game-narrative/SKILL.md) | 원작의 이야기나 설정을 참고해 각색, 다른 결말, 후속 이야기를 만듭니다. |
| [assemble-retro-game-assets](skills/assemble-retro-game-assets/SKILL.md) | 같은 캐릭터의 필드 모습과 초상화처럼 여러 화면에 쓰이는 그림·소리를 함께 계획하고 검토합니다. |

처음에는 `create-retro-fan-game`부터 시작하세요. 이야기나 자산을 여러 장면에 걸쳐 다뤄야 할 때 나머지 스킬을 함께 쓸 수 있습니다. 각 스킬은 따로 사용해도 됩니다.

## 시작하기

스킬 설치를 지원하는 AI 에이전트에는 이렇게 요청하세요.

```text
https://github.com/mcpads/retro-fan-game-skill 저장소의
skills/create-retro-fan-game 스킬을 설치해줘.
```

직접 설치할 때는 에이전트의 설치 방법에 따라 필요한 스킬 폴더를 등록하세요. `SKILL.md`와 `references/`를 비롯한 폴더 내용을 함께 넣어야 합니다.

게임 원본 파일은 별도로 준비하세요. 이 저장소에는 작업 지침과 참고 문서가 들어 있습니다. 실제 분석과 실행 확인에는 분석 도구와 에뮬레이터 등이 필요합니다. AI 에이전트가 이 도구들을 사용할 수 있어야 하며 가능한 수정 범위는 게임에 따라 달라집니다.

게임 이름, 바꾸고 싶은 내용, 유지하고 싶은 부분을 알려주면 작업을 시작할 수 있습니다.

```text
이 게임에서 조연 둘의 후일담을 플레이하고 싶어.
원작 말투는 유지하고, 전투 규칙과 세이브는 그대로 두자.
내가 가진 원본 파일은 이 폴더에 있어.
우선 짧은 장면 하나를 게임에서 볼 수 있게 만들어줘.
이야기 방향을 정해야 하는 부분은 예시와 함께 보여줘.
```

막연한 아이디어라면 짧은 장면이나 그림을 보고 방향을 정해도 됩니다. AI에게 기술적인 방법을 일일이 지정할 필요는 없습니다. 결과에서 무엇이 마음에 들지 않는지, 어떤 부분은 포기할 수 없는지 구체적으로 알려주세요.

## 오래 작업해도 이어갈 수 있도록

작업이 길어지면 실험용 코드와 채택한 결과가 뒤섞이기 쉽습니다. 이 스킬은 조사 자료, 실험 결과, 실제 게임을 만드는 데 쓰는 자료를 구분하고 다음에 이어갈 작업을 기록하도록 안내합니다. 에이전트가 대화 내용을 잊어도 현재 상태를 다시 확인할 수 있게 하려는 것입니다.

작은 변경부터 실제 게임에서 확인하며 작업 범위를 넓혀갑니다. 자신이 원하는 구간을 플레이할 수 있으면 작업을 마쳐도 됩니다. 다른 사람에게 배포할 패키지는 공유를 원할 때 준비합니다.

에이전트가 따를 자세한 기준은 [의도와 판단 권한](skills/create-retro-fan-game/references/strategy/intent-and-authority.md), [현재 상태와 작업 재개](skills/create-retro-fan-game/references/conventions/project-state.md), [공유 자료의 범위](skills/create-retro-fan-game/references/strategy/asset-distribution-policy.md)에 있습니다. 스킬 내부 문서는 영어로 작성되어 있습니다.

## 라이선스

이 저장소의 스킬과 문서는 GNU General Public License version 2 only ([GPL-2.0-only](https://spdx.org/licenses/GPL-2.0-only.html))로 배포합니다. 전문은 [LICENSE](LICENSE)에 있습니다.

이 라이선스는 원작 게임과 그 자산의 이용·배포 권한을 부여하지 않습니다.
