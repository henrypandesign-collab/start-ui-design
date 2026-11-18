---
name: start-ui-design
description: Guide an interactive, reference-first UI design process from product discovery through visual and flow research, component selection, AI state modeling, motion, and a production-ready design direction. Use only when explicitly invoked to start a deliberate UI design workflow; do not use for quick critiques or isolated design questions.
---

# Start UI Design

Help the user shape a UI from evidence and explicit product decisions instead of inventing a polished interface from a blank page.

## Collaboration contract

- Work one stage at a time and ask no more than three questions in a round.
- Ask only for information that materially changes the next decision. Reuse context the user already supplied.
- Explain the current decision and show a small, curated set of options rather than exposing the full workflow at once.
- Do not silently make major product or design decisions. Record the user's choices and carry them forward.
- Let the user skip or reorder stages when they explicitly ask. Otherwise, complete enough discovery to research intelligently before generating a design.
- Distinguish evidence, interpretation, and recommendation. Make clear when a reference is inspiration rather than a pattern to copy.

## Workflow

### 1. Establish the brief

Learn enough to identify:

- the product, feature, or workflow;
- the intended user and their primary job;
- platform and device constraints;
- whether this is new work, a redesign, or an extension;
- existing brand, design-system, content, or technical constraints;
- the current stage and the final artifact the user wants.

Begin with the few unresolved questions that most affect the search. When the brief is sufficiently clear, summarize it in a compact design brief and ask the user to confirm or correct it.

### 2. Research visual direction

Use Refero when broad visual language, layout, hierarchy, density, navigation, typography, color treatment, or product personality is unresolved. Curate multiple references with distinct, relevant characteristics. For each one, explain what works, why it applies, what to borrow, and what not to copy.

Ask the user which direction resonates before treating a visual direction as chosen.

### 3. Research product behavior

Use Mobbin when the design depends on real product flows, information architecture, onboarding, search, filtering, dashboards, tables, settings, empty states, or error handling. Study the behavior across the flow, not just the appearance of one screen.

For each useful example, identify the user goal, flow structure, interaction pattern, transferable lesson, and mismatch with the current product.

### 4. Ground the design in components

Use 21st.dev when implementation-ready React, Tailwind, or shadcn-style building blocks would help translate the direction into a feasible interface. Evaluate candidates for product fit, accessibility, density, adaptability, behavior, and compatibility with the user's stack. Treat them as ingredients, not finished UI.

If the stack is unknown and component feasibility matters, ask before narrowing the search.

### 5. Model AI behavior when applicable

For an AI-enabled experience, define the state model before motion. Use Beautiful UI when useful for reference, but derive the state model from the product's actual behavior.

Include only relevant states, such as idle, input, thinking, searching, tool activity, streaming, approval, partial success, success, empty result, error, retry, and cancellation. For every state, specify:

- what the system is doing;
- what the user sees and can do;
- whether intervention is required;
- how progress, confidence, and uncertainty are communicated.

### 6. Specify motion when it adds meaning

Use Transitions.dev after the state model is clear. Select motion that improves orientation, feedback, continuity, perceived responsiveness, or understanding of system state.

For each meaningful transition, define the trigger, start and end states, duration, easing, delay when relevant, and a reduced-motion behavior. Omit motion that is only decorative unless the user explicitly wants expressive animation.

### 7. Synthesize the direction

Turn the research into one coherent recommendation, not a link dump. Adapt the final artifact to the user's stated goal. It may include:

- a design-direction summary;
- an annotated reference set;
- navigation, information architecture, or user flow;
- component candidates and implementation notes;
- an AI state model;
- motion specifications with reduced-motion behavior;
- wireframes, a UI specification, Figma structure or prompt, prototype specification, React prototype, or design-system recommendations.

Before producing a large final artifact, briefly confirm the proposed direction and deliverable when either remains ambiguous.

## Resource routing

Read [references/design-resources.md](references/design-resources.md) when choosing research sources, documenting references, or structuring the final synthesis. Use only the resources relevant to the current decision; do not search every source by default.

## Quality bar

- Design around the user's actual job and constraints.
- Prefer a few well-explained references over many superficial ones.
- Consider accessibility and implementation feasibility throughout.
- Preserve traceability from the brief to references, design decisions, components, states, and motion.
- If a named resource is unavailable, say so plainly and use the closest credible source without pretending it came from that resource.
