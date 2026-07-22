# Prior Art And Security Record

Reviewed as text-only references on 2026-07-22. MIT licensing permits reuse with license notice, but this skill uses independently written rules and does not bundle third-party executable code.

## Adopted Concepts

- [jnMetaCode/ai-shortfilm-prompts](https://github.com/jnMetaCode/ai-shortfilm-prompts), commit `601d98476fa62709c1e7b78dc1e9783584451263`: staged video prompt construction, genre routing, model-ready output, and targeted negative constraints.
- [YvonneMovingon/short-drama-skills](https://github.com/YvonneMovingon/short-drama-skills), commit `6d632fd7d790cfa45ccf81916bf0e26efd7744c7`: narrative beats, emotion/action decomposition, pacing, and continuity-oriented short-drama production.
- [TateZhouSiu/create-storyboard-skill](https://github.com/TateZhouSiu/create-storyboard-skill), commit `4b8662e2fee51b37488c77952bbfa302bfeaf36c`: continuity bibles, shot cards, reference matrices, and transition handoffs.
- [veryCoolTimo/imagegen-skills](https://github.com/veryCoolTimo/imagegen-skills), commit `b135eda638093f9ce070b4d265afbfd488349ed2`: structured image-prompt anatomy, product-ad routing, model adaptation, editing, and IP checks.
- [inference-sh/skills](https://github.com/inference-sh/skills), commit `fbe0aa4ac8f4be13cbcff551bbbc80554e8eb31f`: product-shot taxonomy, lighting vocabulary, marketplace framing, and detail/scale views.
- [higgsfield-ai/skills](https://github.com/higgsfield-ai/skills), commit `9ab6483d45ebead2c0cf7597ae96ab3eb605fa34`: studio, lifestyle, hero, carousel, conceptual, and virtual-model routing.

## Excluded Components

- All `curl | sh`, automatic installers, external CLIs, MCP setup, and vendor authentication.
- All API-calling generation scripts and automatic uploads of prompts or reference assets.
- The image preset shell import/export examples because untrusted paths or payloads can become command-injection inputs.
- The storyboard package Python scaffold because an unvalidated slug can escape the intended output directory and `--force` can overwrite files.
- Evaluation scripts that invoke external model CLIs or read provider API keys.

## Operational Boundary

This skill contains Markdown and UI metadata only. It has no executable scripts, dependencies, network endpoints, telemetry, credential handling, or automatic generation. Re-audit upstream sources before adopting later changes; commit hashes above define the reviewed snapshots.
