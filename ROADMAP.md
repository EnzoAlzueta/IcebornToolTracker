# Roadmap

## First milestone: data feasibility and a narrow tool-timer MVP

Research duration/remaining-time/recharge data for mantles and boosters on the
supported game build before implementing memory reads or promising coverage.
Use shipped/runtime evidence or authoritative source with provenance. The old
meter reader does not establish that these fields are available or stable.

1. Write docs/RESEARCH.md with candidate sources, game hash/profile, units,
   clock semantics, activation/reset/recharge behavior, availability checks and
   a minimal reproducible observation plan. State unknowns plainly.
2. Prove at least a small useful set of actual tools and transitions. If data
   is not viable, deliver the evidence and limit scope; do not invent offsets or
   approximate timers while labeling them authoritative game values.
3. In parallel, create offline states/fixtures for ready, active, cooldown,
   unavailable, equipment change, quest/town transition and loading.
4. After frozen SDK v1 exists, consume a pinned copy and render a compact panel
   through the shared core. No own graphics/input hooks or custom loader.
5. Add visibility/position/scale and supported-tool options. Measure suitable
   data cadence and avoid recalculating/allocating text every frame unnecessarily.

MVP excludes comprehensive skill/build effects unless verified. Do not promise
exact recharge predictions if the game does not expose the modifiers. Actual
in-game tests/installations are coordinated by the Core instance. Prepare your
module package and STATUS.md for handoff; never overwrite shared runtime files
in another project's tree or the real game folder.
