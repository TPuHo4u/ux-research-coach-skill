# DEVLOG — ux-research-coach skill

## 2026-10-22 — Claude (Opus 5.5, orchestrating Sonnet answerers and Opus judges/reviewers in workflows) — Skill from the course «UX-дизайн и проектирование клиентского опыта»

### What we built
- Fourth course skill next to negotiation-coach, leadership-coach and problem-solving-coach: SKILL.md with a router
  and ten mode contracts in the course's process order — Интервью, Разбор интервью, CJM, Service Blueprint, Опрос,
  Фокусировка, Идеи, Проверка прототипа, plus Индексы and Отчёт для руководства. References `interviews.md`,
  `analysis.md`, `journey.md`, `metrics.md` hold the course content; additions are marked «вывод, не из курса».
- Dev artifacts: spec (D1–D9), six scenarios with observable criteria, RED and GREEN answers with judged verdicts,
  two round-1 reviews (coverage, course fidelity), a round-2 fix verification, package gate `dev/check.sh`.

### Key decisions
- Output contracts, not prohibitions: RED failures were wrong shape and omissions (opinion and presupposing interview
  questions, insights restating pains, CRM and regulations inside a CJM, a blueprint by internal stages, a survey
  without the experience block, a metric never turned into a client problem).
- One origin-tag set and «never invent» rule: RED invented emotions, causes and «other clients».
- Process order follows the course's investment-committee logic: the survey checks the problem hypotheses before the
  key problem is chosen (fidelity review, critical).
- Course survey-craft from the quantitative-research session (5–7 questions, screening and branching, no questions
  about data the databases hold, binary non-negated hypotheses, NPS/CSI taken from existing reports) is course
  content; a «добавь NPS» request keeps NPS apart and is marked as not from the course.
- SKILL.md cap raised to 3,000 words (siblings 2,500) for ten modes; knowledge stays in the references.

### Evidence
- `bash dev/check.sh`: GATE: PASS (frontmatter 1,019 chars, SKILL.md 2,997 words).
- Criteria met: RED 13/36 → GREEN round 1 30/36 → round 2 33/36; without CX 7/30 → 27/30 → 27/30
  (`dev/with-skill/README.md`). Round-2 fix verification: 15 fixed, 3 partly, 2 declined with reasons.
- The last narrow wording fixes (S1 C3, S5 C2, S6 C4, analysis.md §9) were not re-run — residual risk.

### Gaps and owner decisions
- A separately installed older skill `qualitative-research` (~/.agents/skills, linked into ~/.claude/skills) claims the
  same scope; whether to retire it is the owner's call.

### Publication
- 2026-10-22: public repository https://github.com/TPuHo4u/ux-research-coach-skill (owner's word: «делай репозиторий
  для скилла коммит пуш»). Commits use the GitHub noreply address because the account blocks pushes that expose the
  private e-mail. Linked from the exam-practice ux-design card, production `dpl_6g3yLFRz29zaqsZAiQQygGkLmhfu`.
  Local install: symlinks in `~/.claude/skills` and `~/.agents/skills`.

### 2026-10-22 — older qualitative-research skill retired from Claude
- Owner: «да ссылку на старый скилл сними - можешь только из него взять что то новое чего нет у нас». Removed the
  `~/.claude/skills/qualitative-research` link; the original folder in `~/.agents/skills` is untouched.
- Taken over, all marked «вывод, не из курса» except the course-named «Карта стейкхолдеров»: three-level coding for
  several transcripts, the need/barrier insight form, persona frequency and key quote, the extended «Как мы можем»
  form, a stakeholder grouping, «моменты истины» on the emotion curve, line of interaction and physical evidence rows
  in the blueprint. Not taken: «возможности для улучшения» in the CJM (fixes before Фокусировка), a −3…+3 emotion
  scale (invented precision), «3+ respondents = trend» (spread is the survey's job).
- `bash dev/check.sh`: GATE: PASS (SKILL.md 3,000 words). Additive reference notes; scenarios not re-run.
