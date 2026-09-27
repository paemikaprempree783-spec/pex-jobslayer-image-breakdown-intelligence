# Pex JobSlayer Visual Evidence Schema

Use one row per asset region or material finding. Keep unknown values as `unknown`, `not_visible`, or `not_measurable`; never use zero to mean missing.

| Field | Allowed values / notes |
|---|---|
| asset_id | Filename or stable identifier |
| source | Local path, URL, or user-provided reference |
| access_date | ISO date |
| region | background, subject, product, text, logo, offer, proof, CTA, negative_space, whole_image, unknown |
| observation | Neutral description of what is visible |
| transcription | Faithful text or `not_legible` |
| label | FACT, SIGNAL, BET, GAP |
| confidence | high, medium, low |
| visual_role | attention, comprehension, desire, trust, action, brand_memory, unknown |
| situation | pain, aspiration, event, comparison, education, identity, entertainment, unknown |
| promise | functional, emotional, identity, price, proof_led, unknown |
| proof | demo, testimonial, authority, numbers, guarantee, UGC, packaging, none_visible, unknown |
| offer | product_service, consultation, lead_magnet, discount, event, content, unknown |
| action | visible_cta, implied_next_step, no_cta_visible, unknown |
| risk | unreadable, clutter, low_contrast, ambiguity, unsupported_claim, distortion, crop, none_observed |
| evidence_note | Exact visual basis or measurement method |
| implication | Cautious creative/marketing implication |
| next_test | One practical test or `not_needed` |
