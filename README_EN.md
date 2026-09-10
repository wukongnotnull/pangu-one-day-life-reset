# pangu-one-day-life-reset

[中文](README.md) · [English](README_EN.md)

A runnable skill distilled from *How to fix your entire life in 1 day*.

It does not promise to fix an entire life in one day. It uses one day to do four things:

1. Use behavioral evidence to identify the current trajectory and possible protective goals
2. Write a concrete anti-vision and a revisable vision MVP
3. Interrupt autopilot throughout the day
4. Write constraints first, then compress them into one-year evidence, a monthly project, next-day actions, and a feedback time

## Trigger examples

- "Walk me through the one-day life reset protocol."
- "I keep saying I want to publish, but I only research tools. What does my behavior say I actually want?"
- "Help me write an anti-vision and a vision MVP, but don't invent the answers for me."
- "Organize my yearly goal, monthly project, and tomorrow's actions into a life game."
- "I see it clearly in the morning and fall back at night. Help me interrupt autopilot."

## Install

### Option 1: Install with `npx skills`

```bash
npx skills add wukongnotnull/pangu-one-day-life-reset
```

### Option 2: Ask an agent to install it

```text
Help me install this skill: https://github.com/wukongnotnull/pangu-one-day-life-reset
```

## How to use

After activation, start at the safety gate, then move through morning, daytime, evening, and next-day launch. Complete it question by question. Do not let the agent write the entire reflection in one pass.

The session should end with:

```text
The dominant pattern that has me stuck:
Anti-vision:
Vision MVP:
Non-negotiable constraints:
One-year evidence:
One-month project:
Next-day actions:
Next feedback check:
```

## Boundaries

- This is a reflection and planning tool, not therapy or diagnosis.
- Stop intensification exercises if there is self-harm risk, severe depression, mania, psychotic symptoms, or real-world danger.
- The one-day protocol only pushes reversible experiments. It does not push same-day resignation, breakup, stopping medication, or large financial commitments.
- Absolute psychological claims in the source article were not independently verified in this distillation.

## Contents

- `SKILL.md`: Full operating manual
- `examples/publishing-reset.md`: From creative procrastination to a next-day experiment
- `references/distillation/`: Sources, extraction, expression, limits, and key quotes
- `FIDELITY.md`: Independent agent factory score
