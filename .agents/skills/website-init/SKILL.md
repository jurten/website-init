---
name: website-init
description: Gather the essential website brief, inspect local inspiration, and build comparable visual concepts before committing to one direction. Use for new websites, landing pages, portfolios, redesigns, or substantial frontend work that should combine impeccable UX craft with gpt-taste art direction and compare multiple styles using the same content, audience, CTA, scope, and technology.
---

# Website Init

Turn the conversation, repository, and available visual references into a
confirmed brief and a small set of comparable website concepts. Ask only for
missing information; never make the user repeat context they already supplied.

## 1. Inspect available context

1. Read the user's initial project context and later clarifications.
2. Inspect the repository, instructions, stack, scripts, content, assets, and
   current product when available.
3. Separate known facts, safe inferences, and unanswered decisions.
4. Prefer the simplest implementation that can compare the requested styles
   fairly.

## First-response contract

In the first response to a new website request:

1. State what is already understood about the business, audience, takeaway, and
   primary action without repeating the user's words unnecessarily.
2. Report whether `website-inspiration` was found. Name the references selected
   when it was; when it was not, ask for reference sites, screenshots, or visual
   keywords.
3. State explicitly that both `impeccable` and `gpt-taste` will be used, with
   one short phrase describing each role.
4. Say that the default comparison will include a brief-aligned concept, a
   brutalist concept, and a reference-led contrasting concept using the same
   content and functionality.
5. Ask one grouped set of missing questions, including the main takeaway,
   primary action, technology direction, and complexity level when unknown.

Do not present the first response as a generic design questionnaire. Connect
every question and proposed concept to the context already known.

## 2. Find visual references first

Search before asking the user for visual direction:

1. Look for a directory named `website-inspiration` or a close plural,
   hyphenation, or casing variant in the project and nearby workspace.
2. Search its metadata, notes, tags, and filenames for the business category,
   audience, desired feeling, layout, typography, color, and interaction ideas.
3. Select one to three relevant references for each proposed style. Extract
   principles; do not reproduce a reference exactly.
4. Prefer real project assets and local references over generic placeholders.

If no usable inspiration directory or match exists, ask the user for reference
sites, screenshots, brands, visual keywords, likes, and dislikes. Do not invent
a claimed reference.

## 3. Gather the minimum brief

Ask one concise batch covering only unknown details:

1. **Business:** What business, organization, product, or person is the site
   for, and what does it offer?
2. **Audience:** Who is the primary audience, and what need or motivation
   brings them here?
3. **Main takeaway:** What single idea should visitors remember?
4. **Primary action:** What should visitors do next? Identify one primary call
   to action and any secondary action.
5. **Success:** What result would make the website successful?
6. **Scope:** What pages, sections, features, forms, integrations, and content
   are required? What is explicitly out of scope?
7. **Content and brand:** What copy, logo, images, brand rules, and references
   already exist? Who supplies anything missing?
8. **Technology:** Is there an existing codebase or required stack? Otherwise,
   offer the simplest suitable recommendation.
9. **Complexity:** Confirm Simple, Production-ready, or Advanced unless the
   preference is already explicit.
10. **Constraints:** Ask about accessibility, devices, languages, SEO,
    analytics, privacy, compliance, hosting, deadline, and browser support only
    when relevant.

Add project-specific questions only when their answers could materially change
the architecture, content, experience, or definition of done.

## 4. Use both design skills

Use both `impeccable` and `gpt-taste` for every visual website build.

1. Verify that both skills are available and read their complete instructions
   before writing UI code.
2. Follow `impeccable` for product truth, surface mode, UX structure,
   accessibility, responsive behavior, craft quality, and browser iteration.
3. Follow `gpt-taste` for divergent art direction, wide editorial typography,
   layout variety, grid integrity, contrast, and purposeful GSAP motion.
4. Run every setup, context, playbook, preflight, and verification step required
   by either skill.
5. Tell the user that both skills are being used and explain their roles in one
   sentence.

Resolve conflicts in this order:

1. the user's brief, factual content, and explicit constraints;
2. usability, accessibility, product behavior, and the selected surface mode;
3. the expressive conventions of the chosen style.

For Persuade and Experience surfaces, apply the AIDA and motion guidance
directly. For Operate and Read surfaces, preserve the task or reading model and
adapt the same art-direction techniques without forcing marketing structure
onto the product. Always provide reduced-motion behavior.

If either skill is unavailable, use the skill installer when its trusted source
is already known. Otherwise, report the missing skill and ask the user for its
source before implementation.

## 5. Define comparable style concepts

Build three concepts by default when the cost is modest:

1. **Brief-aligned:** Interpret the user's requested direction literally. For
   “clean and simple,” make this concept calm, restrained, and direct.
2. **Brutalist counterpoint:** Keep the same product truth while using a
   deliberate brutalist visual language.
3. **Reference-led contrast:** Choose a distinct third direction supported by
   the inspiration library and audience. Suitable directions include editorial,
   warm organic, refined luxury, playful geometric, retro-futurist, or
   technical minimalism.

Follow a user-specified style or concept count instead of these defaults. Make
each concept a coherent visual thesis, not a palette swap.

Keep these factors identical so the comparison is fair:

- audience and user goal;
- information architecture and factual copy;
- main takeaway and calls to action;
- required functionality and data;
- representative page scope;
- technology and responsive breakpoints.

Vary only presentation choices such as typography, composition, color,
materials, imagery treatment, component form, and motion character.

## 6. Keep comparison inexpensive

Treat concepts as high-fidelity representative implementations, not three fully
duplicated production sites.

- Build the primary landing page or most representative route for each concept
  unless the user explicitly requests complete variants.
- Share semantic content, data, and behavior when doing so remains simple.
- Keep style tokens and presentation components distinct enough to avoid a
  lowest-common-denominator design.
- Prefer separate routes such as `/concepts/clean`, `/concepts/brutalist`, and
  `/concepts/<third-style>`, plus a small comparison index when routing is
  already available.
- Use a style switcher or separate entry files when adding routes would create
  unnecessary complexity.
- Do not duplicate backends, integrations, or data layers for visual concepts.
- If comparable implementations would materially expand scope or require major
  dependencies, explain the cost and ask before building all variants.

Create the `gpt-taste` preflight design plan for each concept using a distinct,
deterministic seed. Scale the resulting motion character to the concept:
restrained for clean, sharp and direct for brutalist, and appropriate to the
third direction.

## 7. Build, run, and verify

Implement the concepts, start the app, and perform verification yourself.

Verify each concept at the same content state, viewport sizes, and route depth:

- the main takeaway is immediately understandable;
- the primary action is prominent and works;
- content and functionality match across concepts;
- headings, buttons, grids, and images remain legible and intact;
- keyboard navigation, focus, contrast, and reduced motion work;
- layouts remain responsive without horizontal overflow;
- animations clean up correctly and do not harm task completion;
- no console errors or broken assets remain.

Capture same-size screenshots when browser tooling is available. Present the
concepts together with their reference sources, design thesis, audience fit,
strengths, tradeoffs, and a clear recommendation.

Do not make the user choose a direction before seeing the concepts when building
them is inexpensive. Keep all concepts until the user selects one; ask before
removing unselected work.

## 8. Preserve the working brief

Record and carry forward:

- business and website purpose;
- primary audience;
- single main takeaway;
- primary and secondary actions;
- success criteria;
- scope and exclusions;
- references and visual directions;
- content and assets;
- technology and complexity level;
- constraints, assumptions, and unresolved blockers.

Ask for confirmation only when material ambiguity remains. Otherwise, continue
through implementation and verification without making the user restate the
brief.
