# ux-research-coach — design spec (2026-10-22)

Owner: Dmitry. Owner's words 2026-10-21: «по завершении всего сделай скилл по мотивам курса, а именно он будет
подготавливать пользователя к глубинным интервью, расшифровывать траскрипты интервью и делать анализ - отчет, посик
инсайтов и тд, он будет строить СОЬ [CJM], BluePrint, готовить вопросы к количественным исследованиям типа к
опроссам, и тд. и посмести его в тренажер по аналогии со скиллми для других курсов»; 2026-10-22: «делай репозиторий
для скилла коммит пуш и деплой изменений тренажера новой дисциплины». Design calls below are the builder's, marked
«call». Execution follows superpowers:writing-skills (RED baseline → GREEN skill → one review round), as the siblings.

## Goal

A self-contained personal skill that applies the Mini-MBA course «UX-дизайн и проектирование клиентского опыта» to
real client-experience research: preparing and running in-depth interviews, turning transcripts or notes into a
report and insights, building a CJM and a Service Blueprint, focusing on the main client problem and a «Как мы можем»
question, writing a survey that checks interview hypotheses, reading NPS / CSI / CSAT, and testing a prototype.
Works in Claude Code and Codex from `~/.claude/skills` / `~/.agents/skills`.

## Decisions

| # | Decision | Consequence |
|---|---|---|
| D1 | Eight modes in the course's process order (Интервью → Разбор → CJM → Blueprint → Фокусировка → Опрос; Индексы and Проверка прототипа stand alone), each an output contract of parts in order (call) | RED failures were wrong shape and omissions, so recipes, not prohibitions |
| D2 | Origin labels [из материала] / [вывод] / [допущение] / [?] and «never invent emotions, numbers, quotes, reasons» (call) | RED invented emotions, causes and «other clients»; hypotheses were stated as findings |
| D3 | No solutions in modes 1–7; ideas go to one line «Идеи на потом (не оценивали)»; idea work starts after Фокусировка (course: two common errors are «слишком рано к решению» and sticking to a ready idea) | RED jumped to fixes in S2, S3, S4, S6 |
| D4 | Interview questions have whitelisted shapes plus a reread step; yes/no only as a clarifying check (call) | RED guides contradicted their own rules (если бы, обычно, options in brackets) |
| D5 | A survey checks hypotheses and their spread; an index request is kept apart and never used as evidence (course rule; how to combine them is «вывод, не из курса») | RED cross-tabbed NPS by hypothesis and missed block 2 |
| D6 | Self-contained; course vocabulary; answers never cite locators. «Расшифровка» and «транскрипт» are domain words here and allowed by the gate (call) | the gate differs from siblings in this one pattern |
| D7 | Neighbours: a general work problem or cause tree → problem-solving-coach; own team → leadership-coach; agreement with others → negotiation-coach; the exam → its trainer (call) | no overlap in descriptions |
| D8 | Public GitHub repository like the three siblings, linked from the portal card (owner's word 2026-10-22; visibility follows the siblings — call) | the trainer link works for every learner |
| D9 | After the review round: ten modes (Идеи and Отчёт для руководства added, survey before Фокусировка as in the course's investment-committee logic); SKILL.md cap 3,000 words instead of the siblings' 2,500 (call) | the skill loads only on client-research topics; knowledge stays in references |

Necessity row. Cost of omitting = an agent asked for an interview guide, a report, a CJM or a survey produces a
plausible but off-method artefact: opinion and hypothetical questions, insights that restate pains, internal systems
in the CJM, a blueprint by internal stages, a survey without the experience block (RED: 13 of 36 criteria met).
Cheapest alternative = asking «по методике курса» each time, which the agent cannot do without the course content.
Measurement that justifies the skill = GREEN closes most RED failures on S1–S6.

## Non-goals

- Audio-to-text transcription itself (the skill works with text the user provides; recording a session and running a
  speech model are outside it).
- Visual UI design, prototypes in design tools, code.
- Full idea generation and selection workshops (a short pointer only); the course exam.
