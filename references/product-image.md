# Product Image Workflow

## Establish Product Truth

Create a product fidelity brief from user-confirmed facts or supplied references:

```text
Product ID / variant:
Category and use:
Silhouette and dimensions:
Materials and surface finish:
Colors:
Controls, ports, seams, closures:
Logo and label placement:
Packaging and included items:
Must-not-change features:
Unknown facts:
```

Never infer hidden sides, ingredients, certifications, compatible devices, scale, or included accessories. If multiple references disagree, ask which is authoritative.

## Select The Image Type

| Type | Primary job | Composition default |
| --- | --- | --- |
| Packshot | accurate listing/catalog view | isolated, neutral, complete silhouette |
| Hero | campaign attention | dominant product, controlled drama, copy space |
| Lifestyle | show context and use | believable interaction, product still legible |
| Detail | prove material or feature | macro/close crop, one feature per frame |
| Scale | communicate size | familiar comparison with truthful proportions |
| Carousel | tell a sequence | consistent angle, light, crop, and variant identity |
| Conceptual | communicate brand idea | metaphor must not distort product truth |

For marketplaces, prioritize platform requirements over artistic styling. Do not add props, badges, text, reflections, or shadows that violate the specified listing policy.

## Design The Shot

Specify observable controls:

- Camera: viewpoint, framing, focal-length feel, distance, depth of field.
- Product pose: orientation, tilt, visible faces, cap/door/screen state.
- Composition: product occupancy, negative space, crop safety, prop hierarchy.
- Lighting: key size/direction, fill ratio, rim, reflection cards, shadow softness.
- Surface and set: material, horizon, background color, environmental context.
- Fidelity: unchanged geometry, finish, label location, ports, controls, and item count.

Use a simple studio setup for reflective, translucent, glossy, metallic, or black products unless the user asks for deliberate complexity. Describe reflection shape and edge separation, not only `studio lighting`.

## Compose The English Prompt

Use this order:

```text
[image type and commercial purpose]. [exact product identity and locked attributes].
[pose, viewpoint, framing, product occupancy, copy space].
[surface, background, props, and human interaction if any].
[key/fill/rim lighting, reflections, shadow behavior, lens feel, depth of field].
[material rendering and color requirements].
[fidelity locks and marketplace constraints].
Avoid: [geometry, label, extra-object, reflection, anatomy, text, crop, and claim failures].
```

Do not replace factual control with style adjectives. Use one clear visual hierarchy and one lighting concept per image.

## Text And Logo Safety

Image models may corrupt small typography and logos. When exact text matters:

1. Generate a clean product/scene while protecting the label area.
2. Preserve or mask the original label when the tool supports controlled editing.
3. Composite approved text and logos afterward from the brand source file.
4. Verify spelling, placement, contrast, and trademark proportions at 100% zoom.

Never fabricate packaging copy. Do not describe an output as logo-perfect unless it was compared with the authoritative asset.

## Product Claim Safety

Separate visual mood from factual claims. Avoid visualizing unverified superiority, medical outcomes, environmental claims, awards, endorsements, or performance numbers. Put required disclaimers and copy in the production notes for later typesetting, not inside the generative prompt.

## Delivery

For a single image, return the fidelity brief, composition plan, prompt, negative constraints, and QA checklist. For a series, add a consistency matrix covering product variant, camera angle, background, light direction, crop, and intended message for every frame.

