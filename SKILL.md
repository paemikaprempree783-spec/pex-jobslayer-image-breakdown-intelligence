---
name: pex-jobslayer-image-breakdown-intelligence
description: Pex JobSlayer evidence-first static image and ad creative intelligence. Use when analyzing ad images, product visuals, screenshots, image URLs, visual hierarchy, copy, offers, audience hypotheses, creative strategy, or AI recreation/improvement prompts; separate visible facts from interpretation and tests.
---

# Pex JobSlayer — Static Image & Ad Creative Intelligence

## Mission
Turn an image into a defensible creative decision: what is visibly present, what marketing job it appears to perform, what may be blocking comprehension or action, and what should be tested next. Do not treat visual quality, longevity, or aesthetic preference as proof of performance.

## Non-negotiable rules

1. **Observe before interpreting.** Separate `FACT` (visible or directly transcribed), `SIGNAL` (pattern supported by visible evidence), `BET` (hypothesis to test), and `GAP` (not observable).
2. **Never invent text, product claims, brand intent, demographics, targeting, conversion rate, CTR, CPA, ROAS, or winner status.** An image alone cannot prove these.
3. If text is unreadable, say `อ่านข้อความไม่ชัดเจน` and quote only the legible portion. Do not silently repair or translate uncertain copy.
4. Describe people and audiences only through observable context and a cautious audience hypothesis. Do not infer sensitive traits or protected attributes.
5. Do not identify fonts, exact HEX values, camera settings, or dimensions as certain unless provided or measured. Use `ประมาณการ` and confidence labels.
6. Do not recommend copying a competitor's protected creative. Extract transferable principles and propose distinct executions.
7. Analyze every image separately before comparing a set. Do not average away important differences.
8. Prompt sections may be in English for image-tool compatibility; the analysis and recommendations should be in Thai unless the user requests another language.
9. A prompt must not ask an image model to render dense final copy unless the chosen tool reliably supports text. Put copy in a separate design step when needed.
10. If the source is private, restricted, geo-blocked, broken, or unavailable, state the limitation and continue only with the material actually available.

## Input routing

Accept: local image files, uploaded images, screenshots, public image URLs, product visuals, logos, brand references, and one or more ad creatives.

Choose the route:

- **Local/uploaded image:** inspect with the native image-reading capability first; use deterministic tools only for measurable properties such as dimensions, aspect ratio, color sampling, or cropping.
- **Public URL:** verify that it is accessible and public, then obtain a viewable image. If access fails, do not fabricate an analysis from the URL or page title.
- **Multiple images:** create one record per image, then a comparison table with matched fields.
- **Prompt-only request:** ask for the target, product, audience/context, platform, aspect ratio, desired fidelity, and what must change; do not pretend an unseen reference was inspected.

## Core workflow

1. **Capture the decision.** Identify whether the user wants diagnosis, recreation, improvement, competitive learning, a creative brief, prompt generation, or comparison. If absent, state a reasonable default.
2. **Record source scope.** Log source/file name or URL, access date, image count, visible platform/context, and any missing or cropped areas.
3. **Inspect the whole image.** First form a one-sentence neutral description without marketing interpretation. Then inspect regions: background, subject/product, text blocks, logo, offer, CTA, proof, and negative space.
4. **Transcribe visible copy.** Preserve line breaks where they affect hierarchy. Mark uncertain words with `[ไม่ชัดเจน]`; distinguish text on-image from text supplied by the user.
5. **Build the evidence map.** For every important conclusion, attach the visible evidence, label, confidence (`สูง/กลาง/ต่ำ`), and what would change it.
6. **Decode the creative system.** Analyze attention, comprehension, desire, trust, action, and brand memory as separate jobs. Do not force every image to have a CTA or direct-response role.
7. **Diagnose friction.** Identify the first likely comprehension break, visual competition, weak proof, unclear offer, unreadable copy, low contrast, or mismatch between promise and action. Label the diagnosis as a `BET` unless directly observable.
8. **Recommend changes.** Prioritize up to three changes by expected learning value and implementation effort. Keep the product truth, brand constraints, and legal/claim boundaries visible.
9. **Create test cards.** Each test should change one major variable when possible and specify a bet, evidence, change, hold, audience/context hypothesis, primary metric, guardrail, and read rule.
10. **Generate prompts only after the strategy is clear.** Provide a faithful recreation prompt only when requested, plus an improvement prompt that preserves essential brand/product facts while changing the chosen variable.
11. **Run a final quality gate.** Check that facts, signals, bets, and gaps are distinguishable; no hidden performance claims were added; prompts are actionable; and uncertain details are marked.

## Image analysis framework

### A. Neutral inventory — FACT only

- Subject/product and count
- Scene, setting, background, and visible props
- Human action or pose, without sensitive-attribute inference
- Text, logo, offer, price, badge, proof, CTA, and destination cues
- Composition, crop, orientation, and approximate aspect ratio
- Lighting, color family, texture, depth, and visual style

### B. Attention architecture

Map the likely scan path: first fixation → second fixation → supporting detail → action/brand memory. Evaluate focal point, contrast, scale, directionality, salience, clutter, and whether the first read matches the intended hook. Use `SIGNAL` for visible hierarchy and `BET` for predicted attention behavior.

### C. Message and offer architecture

Extract, without rewriting as fact:

- **Situation:** pain, aspiration, event, comparison, education, identity, entertainment, unknown
- **Promise:** functional, emotional, identity, price/promotion, proof-led, unknown
- **Mechanism:** how the product appears to create the promised outcome; always a `BET` unless explicitly shown
- **Proof:** demonstration, testimonial, authority, numbers, guarantee, UGC, packaging, none visible
- **Offer:** product/service, consultation, lead magnet, discount, event, content, unknown
- **Action:** CTA or next step visible, implied, or not present

### D. Design and readability

Assess hierarchy, grouping, alignment, spacing, balance, contrast, type scale, line length, cropping, safe areas, mobile legibility, and text-to-image competition. For exact colors or dimensions, give an estimate and state the measurement method or uncertainty.

### E. Conversion and brand role

Classify the likely role as one or more of: `attention`, `problem education`, `desire`, `trust`, `offer support`, `conversion`, `retargeting`, `brand memory`, or `unknown`. The classification is a hypothesis unless the user supplied funnel context or the image makes the role explicit.

### F. Audience hypothesis

Describe the audience through the situation the image speaks to, desired outcome, sophistication level, and likely objection. Provide no more than three hypotheses and include a confidence note. Never infer protected or sensitive attributes from appearance.

## Output modes

- **Quick diagnosis:** one-line role, three evidence-backed findings, top three changes, one test.
- **Full breakdown:** use `templates/image-analysis-report.md`.
- **Creative brief:** turn findings into a production brief with objective, message, proof, visual direction, copy slots, CTA, constraints, and variants.
- **Prompt pack:** use `templates/prompt-pack.md`; include faithful recreation, strategic improvement, and platform adaptation prompts.
- **Comparison:** analyze each image first, then compare matched fields; identify transferable principles, not a winner unless performance data is supplied.
- **OCR/copy only:** output only legible transcription, uncertainty notes, hierarchy, and suggested copy slots.

## Default full-report order

1. Decision and source scope
2. Neutral visual inventory
3. On-image copy transcription and uncertainty
4. Evidence map
5. Attention and visual hierarchy
6. Message, offer, proof, and funnel-role hypothesis
7. Color, typography, layout, and readability
8. Strengths and friction points
9. Audience/context hypotheses
10. Prioritized improvement plan
11. Test cards and measurement
12. Prompt pack, if requested
13. Gaps and next input needed

## Prompt construction rules

Before writing a prompt, specify: target output, fidelity level, subject/product facts that must remain, variable to change, platform/aspect ratio, intended mood, composition, lighting, camera/viewpoint, color direction, negative constraints, and text handling.

Use this structure in English:

```text
Create a [format/aspect ratio] advertising image for [product/context].
Preserve: [truthful product/brand facts and required visual anchors].
Change: [one strategic variable].
Subject and scene: [observable or supplied details].
Composition: [focal point, hierarchy, crop, negative space, safe area].
Lighting and color: [direction].
Style: [distinct art direction, not a named competitor's exact style].
Text handling: leave clean space for later typesetting; do not generate dense copy.
Avoid: [unwanted claims, clutter, distortions, extra products, illegible text].
Output: [platform, ratio, variants, realism/style level].
```

For a faithful recreation, say what must remain and do not add unsupported claims. For an improvement prompt, list the hypothesis being tested and keep the changed variable isolated.

## Quality gate

Before responding, verify:

- The user's decision and source scope are explicit.
- Visible facts are not mixed with interpretation.
- Every important inference is labeled `SIGNAL` or `BET` with evidence.
- Unreadable or missing details are marked, not guessed.
- No sensitive audience traits or performance data were invented.
- Recommendations are prioritized and actionable.
- Tests include a primary metric, guardrail, and read rule.
- Prompts preserve product truth, brand constraints, and text-handling limits.
- Multi-image work contains per-image analysis before comparison.
