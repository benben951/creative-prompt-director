# Prompt Evaluation

Score each dimension from 0 to 2:

| Dimension | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Goal clarity | unclear | inferable | explicit purpose and audience |
| Visual observability | abstract | mixed | actions and appearance are renderable |
| Constraint completeness | missing | partial | format, timing/composition, and exclusions present |
| Continuity or fidelity | drift likely | some locks | identities and state are explicitly locked |
| Model feasibility | overloaded | risky | scoped to likely model capability |
| Safety and truth | unsupported/private | ambiguous | consent, IP, privacy, and claims are handled |

Target at least 10/12 with no zero. A zero in continuity/fidelity or safety/truth is a hard failure regardless of total.

## Review Procedure

1. Extract every claim and must-preserve fact from the prompt.
2. Compare them against the user brief and references; flag unsupported additions.
3. Simulate the first and last frame or the final product image. Confirm they are unambiguous.
4. Count major actions, camera moves, subjects, props, and text demands. Reduce overload.
5. Check that negative constraints name likely failures without contradicting positive instructions.
6. Verify no secret, local path, private metadata, or upload instruction appears.
7. Revise once, then show the score and remaining uncertainty.

## Specialized Checks

For short drama: duration sum, screen direction, eyelines, speaking order, prop hand/state, wardrobe, weather/time, transition receive/send states, and dialogue length.

For product images: silhouette, color, material, ports/controls, label location, item count, scale, reflections, crop, marketplace policy, exact text workflow, and evidence for claims.

