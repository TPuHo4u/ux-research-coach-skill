# ux-research-coach

A personal Claude Code / Codex skill that applies the course «UX-дизайн и проектирование клиентского опыта» to real
client-experience research: preparing in-depth interviews (research plan and guide), working an interview transcript
or notes into a report with insights, building a customer journey map (CJM) and a Service Blueprint, choosing the main
client problem and a «Как мы можем…» question, writing a survey that checks the interview hypotheses, reading NPS,
CSI and CSAT, and testing a prototype with clients. Self-contained: all course knowledge lives in
`skills/ux-research-coach/references/`.

- `skills/ux-research-coach/` — the skill (SKILL.md + references `interviews.md`, `analysis.md`, `journey.md`,
  `metrics.md`). Symlinked from `~/.agents/skills/ux-research-coach` and `~/.claude/skills/ux-research-coach`.
- `dev/` — spec, test scenarios with criteria, baseline (no skill) and with-skill runs with judged verdicts, review
  notes, package gate (`bash dev/check.sh`).

## Install

Claude Code:

```sh
git clone https://github.com/TPuHo4u/ux-research-coach-skill.git
mkdir -p ~/.claude/skills
ln -s "$PWD/ux-research-coach-skill/skills/ux-research-coach" ~/.claude/skills/
```

Codex: the same folder linked into `~/.agents/skills/`. Then ask in plain words, for example «подготовь гайд глубинного
интервью», «вот расшифровка — сделай отчёт и найди инсайты», «собери CJM по заметкам», «составь анкету, чтобы
проверить гипотезы»; the skill can also be called by name.

## Siblings

Sibling of negotiation-coach, leadership-coach and problem-solving-coach: a work problem that is not about a client's
experience, or a cause tree, belongs to problem-solving-coach; how the user leads their own team to leadership-coach;
agreement from others to negotiation-coach. The skill works with text the user provides and does not transcribe
audio. Answers never cite the course materials. The course exam has its own trainer and is out of scope.
