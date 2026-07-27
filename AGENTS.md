# Website project defaults

These rules apply to every website project unless the user explicitly overrides
one of them.

## Tools and ownership

- Never use the Sites tool.
- Whatever action you can do yourself, do it. This includes starting apps,
  running the project, and completing verification steps.
- Do not hand executable steps back to the user unless they require the user's
  credentials, approval, physical interaction, or a decision that cannot be
  inferred safely.

## Context

- For a new website, redesign, or substantial frontend feature, use the
  `website-init` skill before implementation to gather and confirm the essential
  project brief.
- Treat the general context provided at the start of the conversation as
  persistent project context.
- Carry that context into planning, implementation, verification, and later
  follow-up work. Do not make the user repeat it.
- When new instructions conflict with earlier context, follow the user's latest
  explicit instruction.

## Simplicity and complexity

- Advocate for the simplest solution that fully satisfies the user's goal.
- Avoid unnecessary dependencies, abstractions, infrastructure, and speculative
  features.
- Before implementation, ask the user which level of code complexity they want:
  1. **Simple:** minimal implementation with the fewest moving parts.
  2. **Production-ready:** maintainable structure, robust handling, and
     appropriate tests.
  3. **Advanced:** extensible architecture for known future requirements.
- If the user has already stated the desired complexity or the answer is
  unambiguous from their request, do not ask again.
- Briefly explain when a requested choice adds complexity without clear value,
  and recommend the simpler option.

## Completion

- Continue through implementation and reasonable verification instead of
  stopping after giving instructions.
- Report what was completed, what was verified, and any genuine blocker that
  remains.
