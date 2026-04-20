# pictionary-word-generator-skill

> An AI agent skill for generating themed, difficulty-graded Pictionary word packs — powered by [PictionaryHub](https://pictionaryhub.com).

## Overview

This skill turns any AI coding agent into a **Pictionary word pack factory**. Given a topic, difficulty level, scene, and language, the agent will guide you through producing a polished 100–150 word pack ready to upload to [PictionaryHub](https://pictionaryhub.com).

Word packs follow the **long-tail principle** — instead of generic words like "cat", the skill generates specific, drawable, scene-appropriate phrases like _"Garfield napping on a Monday"_ or _"Maneki-neko with a gold coin"_.

## Install

```bash
npx skills add MarkYuanGo/pictionary-word-generator-skill
```

Or install from a local clone:

```bash
npx skills add ./
```

## Usage

Once installed, trigger the skill by asking your agent:

> "Generate a Pictionary word pack for **Ocean Life**, difficulty **Hard**, scene **Science Quiz Night**, in **English**."

The skill will:

1. Prompt you for any missing inputs (keyword / difficulty / scene / language)
2. Provide a ready-to-paste master system prompt for ChatGPT / Claude / Copilot
3. Walk you through reviewing the output against a quality checklist
4. Guide you to upload the final pack to [PictionaryHub](https://pictionaryhub.com)

## Inputs

| Field      | Required | Options                                                |
| ---------- | -------- | ------------------------------------------------------ |
| Keyword    | Yes      | Any theme (e.g., `Space`, `Food`, `Sports`)            |
| Difficulty | Yes      | `Easy` / `Medium` / `Hard` / `Hell`                    |
| Scene      | Yes      | e.g., `Family Party`, `Kids' Learning`, `Trivia Night` |
| Language   | Yes      | Any language (e.g., `English`, `Chinese`, `Spanish`)   |

## Difficulty Levels

| Level      | Description                                  |
| ---------- | -------------------------------------------- |
| **Easy**   | Common, universally recognizable concepts    |
| **Medium** | Requires some domain knowledge               |
| **Hard**   | Niche references, rare items, cultural icons |
| **Hell**   | Obscure, compound concepts — experts only    |

## Example Output (snippet)

**Keyword:** Ocean Life | **Difficulty:** Hard | **Scene:** Science Quiz Night | **Language:** English

```
bioluminescent plankton bloom
mantis shrimp striking with a dactyl club
giant Pacific octopus changing color
anglerfish with a glowing lure
sea cucumber expelling Cuvierian tubules
hydrothermal vent tube worm colony
```

## About PictionaryHub

[PictionaryHub](https://pictionaryhub.com) is an online platform for competitive themed Pictionary. Players choose from curated word packs across dozens of topics, difficulty tiers, and languages — then compete live in drawing sessions.

This skill is the official content-generation workflow used to build PictionaryHub's word pack library.

## License

MIT
