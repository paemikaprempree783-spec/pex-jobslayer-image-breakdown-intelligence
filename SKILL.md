---
name: pex-jobslayer-image-breakdown-intelligence
description: Pex JobSlayer Outcome-First Creative Lab for turning static ads and product images into original, testable creative directions. Use when the user wants better ad results without copying a reference, including visual diagnosis, creative strategy, variant concepts, audience hypotheses, and AI image prompts.
---

# Pex JobSlayer — Outcome-First Creative Lab

## Purpose
Use a reference image as **research input, never as a blueprint**. Recover the job the creative is trying to do, identify the friction that may prevent that job, then invent distinct executions and test them. The goal is equivalent or better business learning and performance—not visual duplication.

## Originality firewall

- Do not reproduce the source's exact composition, copy, headline rhythm, object placement, color treatment, layout, distinctive prop combination, logo treatment, or recognizable art direction.
- Abstract the source into transferable levers such as `contrast`, `proof`, `urgency`, `demonstration`, `social context`, `price salience`, or `category education`.
- Change at least **three major dimensions** in every new direction: composition, visual metaphor/scene, copy angle, color system, subject action, proof device, or information architecture.
- Never use a competitor's name to request an exact style. Describe an independent art direction instead.
- If the user asks to “copy exactly”, explain that the useful alternative is a **principle transfer**: retain the communication job, create a distinct execution, and validate it with a test.

## Evidence discipline

Use four tags throughout the work:

- `OBSERVED`: directly visible or transcribed.
- `INTERPRETED`: a reasonable reading of the visible evidence.
- `HYPOTHESIS`: a claim about audience behavior or performance that requires a test.
- `UNKNOWN`: not readable, not present, or not inferable from the image.

Never invent hidden copy, product benefits, brand intent, audience demographics, funnel stage, CTR, CPA, ROAS, or winner status. Mark uncertain text as `[ไม่ชัดเจน]`. Do not infer protected or sensitive traits from appearance.

## Input and route selection

Accept local/uploaded images, screenshots, public image URLs, product visuals, logos, brand references, and image sets.

1. Establish the desired business outcome: attention, qualified click, lead, purchase, trust, education, retargeting, or brand memory.
2. Establish constraints: product truth, prohibited claims, brand assets, platform/placement, aspect ratio, audience context, and available performance data.
3. Inspect the whole image with native image understanding. Use deterministic tools only for measurable properties such as dimensions, aspect ratio, or color sampling.
4. For URLs, verify public access and obtain a viewable image. If unavailable or restricted, report the limitation and do not infer from the URL alone.
5. For multiple images, create separate observations first; compare only after each image has its own decision record.

## The Outcome-First workflow

### 1. Write the job statement
Complete: “This creative appears intended to help [audience/context] believe or do [action] because it uses [visible mechanism].” Tag each part `OBSERVED`, `INTERPRETED`, or `HYPOTHESIS`.

### 2. Build a signal ledger
Record only high-value signals, not an exhaustive art-school description:

| Signal | Evidence in image | Possible job | Confidence | Unknown |
|---|---|---|---|---|
| | | | | |

Look for attention trigger, promise, proof, offer, action cue, brand memory, and friction. Transcribe only legible text.

### 3. Diagnose the bottleneck
Choose the first likely break in the path:

`notice → understand → believe → want → know what to do → remember brand`

State whether the break is visible (`OBSERVED`) or predicted (`HYPOTHESIS`). Prioritize one bottleneck; do not produce a long list of cosmetic opinions.

### 4. Convert the source into principles
Write 3–5 abstract principles using verbs, for example:

- “Make the before/after contrast instantly legible.”
- “Use proof before adding decorative detail.”
- “Give the offer a single visual home.”

Then explicitly list what **not** to carry over: composition, wording, palette, prop arrangement, or distinctive styling.

### 5. Create a divergence board
Generate three independent directions:

- **Direction A — Demonstration:** show the mechanism or transformation through a new scene.
- **Direction B — Decision shortcut:** simplify the choice with a new information structure or comparison.
- **Direction C — Human consequence:** show the lived outcome, ritual, or context rather than the product pose.

Adapt these names when the category requires it, but keep the directions materially different. Each direction must state its changed dimensions and its risk.

### 6. Design the test
For each selected direction, define one variable to learn, the control, the expected behavior, the primary metric, a guardrail, minimum observation window, and the decision rule. Do not call a creative a winner without supplied performance data.

### 7. Produce the asset brief and prompt
Generate a production brief before an AI prompt. Preserve product truth and brand constraints; invent only the visual execution. Reserve space for final typesetting instead of asking the image model for dense copy.

### 8. Quality and originality gate
Reject the direction if a viewer could place it side-by-side with the reference and identify it as the same layout, wording, palette, or distinctive scene. Rework it by changing the communication device, not by adding random decoration.

## Output modes

- **Decision Sprint:** job statement, bottleneck, three principles, three original directions, one recommended test.
- **Creative Lab Report:** use `templates/creative-lab-report.md`.
- **Variant Board:** output three to six directions with changed dimensions, risk, and test setup.
- **Prompt Studio:** use `templates/prompt-pack.md`; create original prompts only—no faithful recreation prompt.
- **Set comparison:** compare principles, bottlenecks, and learning opportunities; do not rank by aesthetics alone.
- **Copy/legibility pass:** return only confirmed transcription, hierarchy, uncertainty, and new copy angles.

## Recommended report sequence

1. Decision and constraints
2. Job statement
3. Signal ledger
4. Bottleneck diagnosis
5. Principle transfer / do-not-copy list
6. Divergence board
7. Recommended direction and production brief
8. Test design and measurement
9. AI prompt pack, if requested
10. Unknowns and next evidence needed

## Prompt Studio rules

Every prompt must include: outcome, product truth, audience context, one learning hypothesis, three or more changed dimensions, composition, scene/action, lighting/color, platform ratio, clean text area, negative constraints, and post-generation checks.

Use English for image tools when helpful:

```text
Create an original [platform/aspect ratio] advertising visual for [truthful product/context].
Business job: [attention, understanding, trust, desire, or action].
Learning hypothesis: [one testable hypothesis].
Preserve only: [verified product/brand facts].
Do not copy: [reference layout, wording, palette, prop arrangement, or distinctive style].
New execution: [new scene, visual metaphor, subject action, and information structure].
Composition: [new focal point, scan path, crop, and safe area].
Lighting and color: [independent direction].
Text handling: reserve clean space for later typesetting; do not render dense copy.
Avoid: unsupported claims, distorted packaging, extra products, competitor imitation, clutter, and illegible text.
Output: [ratio, number of variants, realism/style level].
```

## Final response checks

- Is the desired business outcome explicit?
- Are observation, interpretation, hypothesis, and unknown separated?
- Is the main bottleneck prioritized?
- Are transferable principles abstract rather than copied details?
- Does every new direction differ in at least three major dimensions?
- Is product truth preserved without invented claims?
- Does the test specify control, metric, guardrail, window, and read rule?
- Does the prompt reserve text for a later design step?
