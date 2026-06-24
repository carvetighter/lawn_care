# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a research and planning project for rebuilding a lawn in Gadsden, Alabama (northeast AL). The goal is a multi-season (2–3 year) restoration focused on natural, soil-first methods — no pesticides.

Key goals from `documents/project_info.md`:
- Build soil health analogous to terra preta (biochar-enriched, biologically active)
- Select grass suited to hot humid summers (can reach ~100°F briefly) and mild winters (rarely below freezing for more than ~30 days)
- Mimic natural ecosystem processes: support beneficial insects, worms, and microbes to crowd out weeds and pests organically
- Achieve deep-rooted, dense, dark-green turf that is winter- and summer-hardy
- Have a repeatable seasonal process to follow for building and maintaining the lawn year over year

Explicit non-goals:
- No pesticides or synthetic pest controls
- No approaches that require the lawn to be reseeded each season

Open questions the owner wants answered (see `documents/project_info.md` for full list): grass variety selection, soil testing methods, regional seasonal care calendar (aeration, seeding, composting, watering), optimal mowing height per grass type, and key nutrients/minerals for turf color and vigor.

## Repository Structure

- `documents/project_info.md` — the owner's raw brief (Situation / What I Want / What I Don't Want / What I Don't Know). This is the source of truth for goals and constraints. It is written in the owner's own words and contains typos; treat it as a verbatim record — don't "correct" or rewrite it.
- `documents/lawn_plan_YYYYMMDD.md` — dated, research-backed plans that answer the brief. `lawn_plan_20260623.md` is the current plan; date-suffix new revisions rather than overwriting, so the planning history is preserved.
- `src/` — reserved for any scripts, tools, or structured data (currently empty).

## Current Plan (decisions already made)

`documents/lawn_plan_20260623.md` is the working plan. Before re-deriving anything, know that it already settled the major forks — extend or revise it rather than starting over:

- **Grass: Zoysia, established by SEED (not plugs or sod).** This is a firm owner decision — do not propose plugging/sodding as the primary method. Seeding forces a **seed-available cultivar (Zenith or Compadre/Companion)**; Meyer/Zeon are vegetative-only and are off the table. Plugging survives only as a contingency to fill gaps if seeding fails. Zoysia was chosen over tall fescue and bermuda because its dense canopy crowds weeds without chemicals and it's a light feeder that fits the soil-first, no-pesticide approach.
- **Timeline: prep in 2026, seed late May–June 2027.** Site is cleared by sheet-mulching (cardboard + 3–4" compost) starting fall 2026 (Option A) or solarize + winter-rye cover crop (Option B, §2b); soil corrected over winter; zoysia **seeded** once soil is consistently ~70°F+. Seeding implications to keep in mind: slow germination (2–3 wks), constant moisture for 3–4 weeks, heavier year-one weeds, no corn-gluten pre-emergent the seeding year, and — if the rye cover crop is used — a 4–6 week buffer after rye termination before sowing (rye allelopathy suppresses seed). A repeatable seasonal cycle (§4) carries it forward.
- **Soil test: Alabama Cooperative Extension / Auburn lab** via the Etowah County Extension office (contact details in §2). Target pH 6.0–6.5. Everything downstream depends on this test.
- **Terra preta method:** charged biochar (charge before applying) + compost delivered via annual core-aeration + ¼–½" topdressing; feed the soil biology, leave clippings. Don't till.
- **Pest/weed control: no pesticides.** Beneficial nematodes (*S. feltiae*) for ants/grubs, dense canopy + hand-weeding for weeds, Bt for armyworms, morning watering against fungus.

## Working in This Repo

There are no build, lint, or test commands — this is a documents-only research project. If scripts are added to `src/`, document their usage here.

When generating research, plans, or schedules, anchor recommendations to the Gadsden / Etowah County, AL climate (USDA zone 7b/8a, warm/cool-season transition zone) and the owner's stated constraints above. Favor concrete, local, actionable specifics (named suppliers, extension contacts, real costs, dated timing) over generic lawn advice — that is the standard the existing plan sets. Today's date is 2026-06-24, so "now" is summer prep before the spring 2027 planting.
