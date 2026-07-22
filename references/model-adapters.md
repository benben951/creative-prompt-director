# Model Adapters

Use current official documentation when exact syntax matters; model capabilities and parameter names change. Do not guess unsupported flags.

## Universal Default

When no model is named, output a provider-independent natural-language prompt plus separate fields for aspect ratio, duration, reference inputs, and negative constraints. Do not embed CLI flags.

## Adaptation Rules

- Preserve the creative contract and fidelity locks across models.
- Move parameters such as duration, aspect ratio, seed, resolution, reference strength, or camera controls into a separate settings block when the target UI exposes them.
- Keep negative constraints separate when the model has a negative-prompt field; otherwise append a concise `Avoid:` sentence.
- For image-to-video, distinguish reference-locked facts from allowed motion.
- For models with weak text rendering, use the compositing workflow rather than adding more spelling instructions.
- For models without audio or lip-sync, deliver dialogue and sound as post-production notes.
- Never add unofficial API endpoints, install commands, environment variables, or credentials.

## Output Settings Block

```text
Target model: [named model or universal]
Mode: [text-to-image / image-to-image / text-to-video / image-to-video]
Aspect ratio:
Duration / image count:
Resolution / quality: [only if confirmed supported]
Reference inputs: [user-provided IDs, not private local paths]
Seed / consistency controls: [only if confirmed supported]
Post-production notes:
```

