# Start UI Design

**A reference-first, collaborative Agent Skill for designing better product interfaces.**

Start UI Design guides designers and AI assistants from a clear product brief to a traceable UI design direction. Instead of jumping straight into a polished mockup, it asks focused questions, researches relevant references, and ties recommendations back to user needs and implementation constraints.

> **Core principle:** Design from evidence and explicit decisions — not from a blank-page guess.

## What it does

- **Starts with the product problem.** Understand the user, job-to-be-done, platform, constraints, and intended deliverable.
- **Explores visual directions.** Use [Refero](https://refero.design/) for visual language, hierarchy, density, and layout inspiration.
- **Researches real flows.** Use [Mobbin](https://mobbin.com/) for interaction patterns and product behavior.
- **Finds plausible building blocks.** Evaluate components from [21st.dev](https://21st.dev/) for accessibility and implementation fit.
- **Models AI states when relevant.** Use [Beautiful UI](https://www.beautifului.dev/) as inspiration, while deriving actual states from the product.
- **Adds meaningful motion.** Use [Transitions.dev](https://www.transitions.dev/) to specify purposeful transitions and reduced-motion alternatives.
- **Synthesizes a design direction.** Deliver a brief, annotated references, flows, components, states, motion, or a prototype specification as needed.

The stages are **adaptive, not a mandatory seven-step checklist**. The skill uses only the resources relevant to the current design decision.

## Install

### Option A: Codex skill installer

In a Codex session with the built-in skill installer available, ask:

```text
$skill-installer install https://github.com/henrypandesign-collab/start-ui-design/tree/main/skills/start-ui-design
```

Restart Codex or refresh its skill list if necessary.

### Option B: Manual install

```bash
git clone https://github.com/henrypandesign-collab/start-ui-design.git
mkdir -p ~/.agents/skills
cp -R start-ui-design/skills/start-ui-design ~/.agents/skills/
```

For a project-local skill, place the `start-ui-design` folder under `.agents/skills/` in your project instead. For other compatible tools, follow their native Agent Skills installation path.

## Usage

This skill **only activates when explicitly invoked**. It will not interrupt ordinary UI questions or quick critiques.

Example:

```text
$start-ui-design Help me redesign an enterprise dashboard for operations managers.
The primary goal is to identify blocked work and decide what to do next.
We have an existing React design system. Start with the brief, not a mockup.
```

Other useful examples:

```text
$start-ui-design I'm designing an AI approval workflow. Help me define its user flow and states.
```

```text
$start-ui-design I have three visual directions. Help me compare them against the product brief.
```

The assistant should ask **no more than three questions per round**, work stage by stage, distinguish evidence from interpretation, and make design decisions with the user rather than on the user's behalf.

## The workflow

| Stage | Design question | Typical output |
|---|---|---|
| 1. Brief | Who is this for, and what job must it accomplish? | Confirmed brief and constraints |
| 2. Visual direction | What visual language supports this context? | Annotated visual references |
| 3. Product behavior | Which real-world flows are worth studying? | Transferable interaction patterns |
| 4. Components | What is feasible in the target stack? | Adopt / adapt / inspiration-only candidates |
| 5. AI states | What should users see and do as the system works? | AI state matrix, if applicable |
| 6. Motion | Which transitions provide useful feedback? | Motion and reduced-motion specification |
| 7. Synthesis | What coherent direction should move forward? | Design recommendation or requested artifact |

## Repository contents

```text
skills/start-ui-design/
├── SKILL.md                        # Agent instructions
├── agents/openai.yaml              # Optional OpenAI/Codex metadata
└── references/design-resources.md # Research and synthesis guidance
```

## Requirements and limitations

- This is an **instruction skill**, not a standalone web app, Figma plugin, or component library.
- Web browsing and access to external reference platforms may depend on the host agent, available tools, subscriptions, and permissions.
- References from third-party websites are used for research. This repository does **not** distribute their screenshots, source code, trademarks, or licensed assets.
- Design recommendations are not a substitute for accessibility testing, product validation, or engineering review.
- When a service is unavailable, the skill should say so and use a credible alternative rather than invent evidence.

## Contributing

Issues and pull requests are welcome. Good contributions make the workflow clearer, improve accessibility or evidence quality, or add **optional** research guidance without making the skill depend on any one vendor.

## License

[MIT](LICENSE) for the original instructions and repository materials. Third-party websites, product imagery, and referenced component libraries retain their respective licenses.
