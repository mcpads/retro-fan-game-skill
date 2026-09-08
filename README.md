# Retro Fan Game Skills

English | [한국어](README.ko.md)

AI skills for people who want to change a favorite retro game's story, artwork, or rules and play the result. A skill is a set of instructions and reference documents that an AI agent consults while working.

You decide what game you want to make. The agent investigates the game's structure, finds ways to change it, and implements them. You judge whether the result has the right atmosphere, whether a character would say a particular line, and which compromises you can accept.

## Included skills

| Skill | What it helps with |
| --- | --- |
| [create-retro-fan-game](skills/create-retro-fan-game/SKILL.md) | Define the intended game and carry work from investigating the original through changes and in-game checks. |
| [adapt-retro-game-narrative](skills/adapt-retro-game-narrative/SKILL.md) | Adapt an existing story or canon into retellings, alternate endings, and continuations. |
| [assemble-retro-game-assets](skills/assemble-retro-game-assets/SKILL.md) | Plan and review related artwork and audio across game contexts, such as a character's field sprite and portrait. |

Start with `create-retro-fan-game`. Add the other skills when story or asset work spans several scenes or representations. Each skill can also be used on its own.

## Getting started

If your AI agent supports skill installation, ask it:

```text
Install the skill at skills/create-retro-fan-game from
https://github.com/mcpads/retro-fan-game-skill
```

For manual installation, follow your agent's instructions for adding a skill folder. Include the whole folder, including `SKILL.md` and `references/`.

Supply your own original game files. This repository contains instructions and reference documents. Analysis and in-game checks require tools such as binary analysis utilities and an emulator that the agent can use. The changes that are possible depend on the game.

To begin, name the game, explain what you want to change, and say what you want to preserve. For example:

```text
I want to play an epilogue about two supporting characters in this game.
Keep their original voices, the combat rules, and save behavior.
My original game files are in this folder.
Start by making one short scene that I can see in the game.
Show me examples when a story decision needs my input.
```

If the idea is still vague, use a short scene or image to decide on a direction. You do not need to specify every technical method. Explain what you dislike about a result and what you are unwilling to give up.

## Continuing a long project

As work accumulates, experimental code and adopted results can become difficult to distinguish. These skills guide the agent to keep research, experiments, and inputs used to build the game distinguishable, and to record the next action. The aim is to recover the current state even after the agent loses the conversation context.

Start with a small change and check it in the game before expanding the work. Being able to play your intended route is a complete outcome. Prepare a package for others when you want to share it.

The agent's detailed guidance lives in [Intent And Authority](skills/create-retro-fan-game/references/strategy/intent-and-authority.md), [Project State](skills/create-retro-fan-game/references/conventions/project-state.md), and [Asset Distribution Policy](skills/create-retro-fan-game/references/strategy/asset-distribution-policy.md). The skill documents are written in English.

## License

The skills and documents in this repository are licensed under the GNU General Public License version 2 only ([GPL-2.0-only](https://spdx.org/licenses/GPL-2.0-only.html)). See [LICENSE](LICENSE) for the full text.

This license does not grant permission to use or redistribute the original games or their assets.
