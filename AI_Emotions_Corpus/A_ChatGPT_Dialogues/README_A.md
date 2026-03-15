# Subcorpus A: ChatGPT Dialogues

## Overview

This subcorpus contains **8 elicited dialogues** produced through ChatGPT (**GPT-5.4 Thinking**) in **March 2026**. All prompts were written by the researcher as first-person emotional disclosures, with memory disabled between sessions to ensure each dialogue was independent.

The subcorpus functions as a **controlled baseline** for the analysis of institutional, safety-aligned empathic discourse in a general-purpose large language model.

## Items

| ID | Emotion category | File |
|----|-----------------|------|
| A001 | sadness / grief | A001.json |
| A002 | anxiety | A002.json |
| A003 | disappointment | A003.json |
| A004 | guilt | A004.json |
| A005 | chronic stress | A005.json |
| A006 | anger | A006.json |
| A007 | interpersonal conflict | A007.json |
| A008 | positive emotion | A008.json |

## Elicitation procedure

- Each prompt was written as a first-person emotional disclosure without explicitly requesting empathy or advice.
- All dialogues were generated in separate conversations with memory disabled.
- The coding unit is the AI response turn (one per dialogue).
- No post-editing was applied to the system responses.

## Metadata fields

| Field | Description |
|-------|-------------|
| `id` | Item identifier |
| `subcorpus` | Always `A_ChatGPT_dialogues` |
| `system` | Always `ChatGPT` |
| `model` | Model version |
| `source_type` | Always `elicited_dialogue` |
| `elicited_by_researcher` | Always `true` |
| `date` | Date of elicitation |
| `language` | Always `en` |
| `emotion_category` | Target emotion of the prompt |
| `turn_count` | Number of turns (always 2: user + AI) |
| `memory_disabled` | Always `true` |
| `analytical_role` | Role in the analysis |
| `used_in_sections` | Sections of the accompanying study where the item is cited |
| `analysis_tags` | Discourse strategies identified in the response |
| `prompt` | User turn (researcher-authored) |
| `response` | AI response turn (coding unit) |

## Notes

Two items (A005, Chronic stress) triggered the safety protocol activation, which is discussed in Section 3.2.4 of the accompanying analysis.
