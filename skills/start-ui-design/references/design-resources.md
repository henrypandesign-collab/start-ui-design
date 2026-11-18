# Design Resource Guide

Use this guide only for the research and synthesis stages that apply to the current request.

## Source routing

| Source | Best for | Avoid using it as |
|---|---|---|
| Refero | Visual direction, hierarchy, layout, density, typography, navigation, color, and product personality | Evidence that a full workflow is usable |
| Mobbin | Real product flows, information architecture, interaction patterns, onboarding, search, filtering, settings, tables, and system states | A component library or a reason to copy a branded flow wholesale |
| 21st.dev | Implementation-ready React, Tailwind, and shadcn-style components or interaction building blocks | A substitute for product architecture or accessibility review |
| Beautiful UI | Presentation of AI activity, progress, uncertainty, approvals, results, and failures | The source of truth for the product's state model |
| Transitions.dev | State transitions, progressive disclosure, enter/exit behavior, streaming feedback, and microinteractions | A reason to add motion before behavior is understood |

Search the source that answers the current question. A typical sequence is Refero for visual language, Mobbin for behavior, 21st.dev for components, Beautiful UI for AI states, and Transitions.dev for motion, but omit or reorder sources when the brief calls for it.

## Reference record

For each shortlisted reference, capture enough detail to support a decision:

- source and identifiable item or URL;
- the user goal or design question it informs;
- the specific characteristic or pattern that works;
- why it transfers to this product;
- what to borrow or adapt;
- what conflicts with the brief and should not be copied.

Do not present a screenshot or link without interpretation. Prefer contrasting references when the user is choosing between materially different directions.

## Flow analysis

When studying a product flow, inspect the sequence rather than only the hero screen. Note:

- entry point and user intent;
- information architecture and progressive disclosure;
- primary and secondary actions;
- feedback, waiting, empty, error, and recovery states;
- points where the user's context or trust could be lost;
- the parts that depend on the reference product's business model or ecosystem.

## Component evaluation

For each component candidate, assess:

- semantic and interaction fit;
- keyboard and screen-reader behavior;
- responsive behavior and density;
- visual adaptability to the chosen direction;
- dependency and stack compatibility;
- engineering effort or hidden complexity.

Label candidates as adopt, adapt, or inspiration-only when that distinction helps implementation.

## AI state matrix

A compact state matrix can use these columns:

| State | System activity | User-visible feedback | Available action | Intervention | Progress / uncertainty |
|---|---|---|---|---|---|

Use only states the product can actually enter. Define transitions and recovery paths for failures, cancellations, and partial outcomes.

## Motion specification

Describe motion at the transition level:

| Transition | Trigger | Start | End | Timing | Purpose | Reduced motion |
|---|---|---|---|---|---|---|

Timing should be concrete enough to prototype, but it can remain a range until the visual design is tested. Reduced-motion behavior should preserve state feedback without relying on movement.

## Final synthesis

Organize the final output around decisions rather than source websites. A useful structure is:

1. Confirmed brief and success criteria.
2. Recommended visual and interaction direction.
3. Annotated evidence supporting that direction.
4. Information architecture or flow.
5. Component plan and implementation notes.
6. AI state model, when applicable.
7. Motion behavior, when applicable.
8. The requested production artifact and open questions.

Keep a visible chain from each recommendation back to the brief or evidence. Call out assumptions that still need validation.
