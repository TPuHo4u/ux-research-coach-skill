# Round 1 — what was changed (2026-10-22)

Sources: `coverage.md` (22 findings), `fidelity.md` (29 findings), GREEN round-1 judge notes (`../with-skill/round1/`).

## Accepted and applied

| Finding | Change |
|---|---|
| fidelity critical: survey must precede Фокусировка | process order 1 → 2 → 3 → 4 → 6 → 5 → 9 → 8; mode 5 chooses the main problem with survey results, otherwise [допущение] and the survey |
| coverage: routing when the user names outputs; «closed» undefined | named outputs → those modes in process order in one answer; a step is closed when the message brings its output |
| both: «no fixes in 1–7» vs mode 7 plan with dates | mode 7's plan is a plan of checks; fixes only from mode 9 |
| coverage: no index questionnaire | mode 7 routes «анкета NPS/CSI/CSAT»; shapes in `metrics.md` §8 |
| coverage: report for management | mode 10 on the investment-committee structure; `analysis.md` §6 |
| coverage: several transcripts | mode 2 branch: cards, merged path «у кого (из N с данными)», matrix, persona splits, cross insights |
| coverage: ideas dead end | mode 9 Идеи (`analysis.md` §9) |
| coverage: client metric fell, no research | routing row to mode 1 opening with metric → scenario |
| coverage: review of the user's own guide / survey / map / interview | review shape in the router |
| fidelity: survey tasks include significance; hypothesis wording | mode 6 part 1 (наличие, значимость, периодичность; ясно, однозначно бинарно, не отрицанием); ranking question allowed; course survey-craft rules in `metrics.md` §2 |
| fidelity: NPS in the hypothesis survey | default per course: not added, existing reports used; insisting user → separate last question marked «вывод, не из курса» |
| fidelity: insight called a hypothesis | insight = вывод about why; problem hypotheses are checked by a survey; template and count marked |
| fidelity: guide rules stricter than the course | course's correct and wrong examples verbatim; «Покажите, как вы обычно…» allowed; ban limited to «часто/редко/иногда» as answer gradations; presupposing questions (course errors) added; «что улучшить» removed |
| fidelity: methods, respondents, roles, story case | ≥2 methods (interviews ≥5, second ≥3 times); users, internal/external experts, явные и невидимые участники; four course roles; «самый неприятный или долгий случай» |
| fidelity: base of percentages; conditional hypothesis | base = target respondents after block 1; conditional hypothesis read among those with the condition |
| fidelity: CSI steps applied to NPS | mode 7 splits NPS and CSI parts |
| fidelity: CJM rows, lanes, failure signs | need and process-ownership rows; one path by default, lanes marked; failure points also by the course's signs |
| fidelity / judges: misc | mode 8 numbered; persona-only request; next-turn full version; audio input; one tag set; examples marked «пример для расчёта (не из курса)»; 0 on a 0–10 scale; regulations never in CJM cells; no hypothesis labels in respondent text; no mode names in answers; marks either inline or in one closing line |

## Not accepted (decision)

- Retiring the separately installed `qualitative-research` skill — the owner's decision; reported to the owner.
- Removing the «вывод, не из курса» marks to satisfy CX — kept as the siblings' convention; CX clarified in
  `../scenarios.md`.
