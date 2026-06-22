# Academic Naturalizer

A prompt-based tool that revises AI-generated academic prose into clearer,
more natural, and source-faithful writing — without altering the author's
argument, citations, or scholarly tone.

## What it does

The tool detects and corrects patterns common in AI-generated academic text:
inflated phrasing, formulaic transitions, overstrong claims, vague attributions,
and mechanical formatting. It applies a 29-pattern rewrite catalogue and
8 supplemental AI-tell checks, with built-in rules for claim discipline,
citation integrity, and revision intensity.

## What I was trying to solve

AI-assisted academic writing often sounds generic, over-polished, or
structurally weak — even when the underlying argument is solid. I built this
tool to fix the surface problems without touching the substance: the citations
stay, the argument stays, the voice stays. Only the AI texture goes.

## Structure

- `SKILL.md` — core logic: priority order, integrity rules, claim discipline,
  output format
- `patterns.md` — 29 AI-tell patterns with before/after examples
  (based on Siqi Chen's rewrite playbook, MIT License)
- `supplemental-ai-tells.md` — 8 supplemental patterns for scaffolding,
  citation leakage, and register discontinuity

## Status

Runs inside Claude as a custom skill. Iteratively tested and refined based
on output quality across thesis chapters, literature reviews, and methodology
sections.
