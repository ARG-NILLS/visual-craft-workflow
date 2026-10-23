---
name: visual-craft-workflow
description: >-
  Use when asked to design, improve, redesign, audit, or polish a website, app interface, or other visual
  project. Orchestrates a scope-aware workflow for visual direction, product UX, interaction craft, and
  evidence-based review while preserving the user’s brief, project identity, and technical constraints.
  Also use when preparing or presenting a project repository; review its name, description, README, and
  structure against the actual project identity.
---

# Visual Craft Workflow

## Purpose

This project and its adaptive workflow are created and maintained by ARG-NILLS.

Use this as one entry point for visual work. The workflow combines a distinctive visual direction, product UX, interaction craft, and evidence-based review, then activates only the stages that fit the work.

This skill is self-contained. Companion skills and platform-specific tools can deepen a stage, but they are optional. If they are unavailable, continue with this workflow and the tools the host provides. Never claim a tool or review ran when it did not.

## Triage the request

Before acting, identify:

- **Intent:** audit, plan, create, redesign, or refine.
- **Scope:** one detail, component, screen, page, or system.
- **State:** existing experience or genuinely new work.
- **Surface:** public page, working app, reading experience, showcase, or another visual artifact.
- **Constraints:** audience, user goal, brand, stack, content, assets, devices, and deadline.

Read applicable project instructions and inspect the current work when available. Treat audits and plans as read-only unless the user asks for edits. Preserve useful behavior, product facts, and working patterns. Ask only when a missing fact blocks progress; otherwise state a sensible assumption and continue.

## Choose the needed pipeline

Scale the workflow to the request. Use all three lenses for substantial work that spans visual direction, product UX, and interaction craft. Skip stages that cannot improve the requested result.

| Request | Visual direction | Product UX | Interaction craft |
| --- | --- | --- | --- |
| New surface or major redesign | Find a project-specific idea, composition, typography, palette, and imagery. | Define the visitor's goal, content hierarchy, flows, and surface mode. | Apply during implementation to component behavior, states, motion, and finish. |
| App screen or dashboard | Use app-screen thinking; do not apply a marketing-page recipe to a working tool. | Prioritize task completion, scanability, edge states, accessibility, and consistency. | Refine controls, feedback, focus, keyboard, touch, and useful transitions. |
| Small refinement | Preserve the existing direction; do not restart the concept process. | Improve only the affected hierarchy, content, layout, or state. | Use only for the affected component or interaction. |
| Audit or critique | Inspect the rendered page or artifact when possible. | Assess usability and technical interface quality within the requested scope. | Review motion only when it is part of the request. Do not edit. |
| Motion-only work | Skip unless the visual concept changes. | Consider interaction clarity and reduced-motion behavior. | Decide whether motion helps, then assess timing, interruption, frequency, and performance. |
| Non-visual work | Skip. | Skip unless interface behavior or presentation changes. | Skip. |

For a full design pipeline, work in this order: establish the visual idea, shape the experience around the user's goal, then implement interaction and detail. Revisit earlier choices when real output shows a problem.

## 1. Establish visual truth

For existing work, inspect its structure, routes or screens, design tokens, typography, copy, assets, behavior, and rendered appearance. Identify what must stay and what the user asked to change. A missing design document does not mean the product has no established style.

For new work, understand the subject, audience, purpose, evidence, and constraints before choosing a visual direction. Look for distinctive facts, materials, places, language, product behavior, or real assets that belong to this project. Build the concept from those specifics; avoid generic layouts and decoration without a reason.

Choose the ambition that fits the surface:

- **Persuade:** a visitor should understand an offer and act, as on a landing or pricing page.
- **Operate:** a user should complete a task, as in a dashboard, editor, or admin tool.
- **Read:** a person should understand and follow content.
- **Experience:** the work itself should lead, as in a portfolio or gallery.

A product marketing page and the app it depicts are different surfaces. Give each the right structure while keeping their visual system coherent.

## 2. Shape the experience

Make the primary user goal obvious. Organize real content before polishing decoration. Map navigation, important actions, and key states. For interfaces, account for loading, empty, success, and error states when they apply. Give each visible action an honest destination or outcome; do not invent product claims, metrics, or functionality.

For a refinement, keep the existing identity and behavior outside the requested scope. For a redesign, preserve product truth, content, and required functions while making a deliberate replacement direction. Do not split a redesign between the old visual world and a new one without a reason.

## 3. Build with craft

Use the project's current stack, design system, components, and tokens unless the user asks to change them. Keep layouts responsive and content legible. Use real, project-relevant imagery when available; label placeholders and unknowns honestly.

Every interaction should communicate its state. Include relevant hover, pressed, focus, selected, disabled, and validation states. Support keyboard and touch input where applicable. Motion should explain a change, preserve spatial continuity, or give useful feedback. Reduce or remove motion for repeated actions, respect reduced-motion preferences, and avoid effects that hurt readability or performance.

The user's explicit visual direction and the project's established identity take priority over any house-style default. This includes ambitious styles such as liquid glass. When that direction is requested or clearly relevant, use the on-demand [liquid-glass style reference](references/liquid-glass-style.md). Keep contrast, accessibility, usability, and runtime cost in view while honoring the brief.

## 4. Review the result

When implementation is in scope, inspect the actual rendered output at representative sizes and states. Choose checks that match the surface and request: responsive layout, navigation and controls, keyboard flow, touch targets, reduced motion, contrast, accessibility, console or network behavior, and performance. For a static visual artifact, review its composition, legibility, fidelity, and export instead of forcing web checks.

Fix observed issues within scope and review the changed result again. If the runtime, browser, device, or asset is unavailable, report that limitation. Separate source inspection from live verification.

## 5. Report clearly

Summarize the work or prioritized findings, the checks actually performed, and remaining gaps. Keep recommendations concrete and tied to the user's goal. Do not claim a design, route, device, or interaction was reviewed unless evidence supports it.

## Repository identity and presentation

When a request prepares, brands, publishes, or broadly polishes a project repository, review its public-facing identity and presentation:

- Compare the repository slug with the actual project, product, package, or skill name. For this skill’s repository, the slug, skill folder, and `name` frontmatter must all be `visual-craft-workflow`.
- For another repository, compare its slug with that project’s own identity. Never compare it with this skill’s name.
- Check GitHub’s short description, README hierarchy, quick start, repository map, examples, links, visual assets, and license status. Keep every claim consistent with files and verified host behavior.
- Use emojis and visual accents sparingly and consistently. Add badges only when they show a true, maintainable status.
- Fix clear presentation issues when repository setup or polish is in scope. For narrow code or UI work, flag unrelated repository issues without rewriting documentation.
- Do not invent releases, tests, features, compatibility, or a license. Do not rename a remote repository or change its visibility without explicit direction; those changes can break links and access.

Use this check for future repositories without applying this skill’s name or visual brand to them.

## Optional tools

Platform-specific tools and additional skills may deepen individual stages. They remain optional; this workflow continues with the host’s available tools and project context.