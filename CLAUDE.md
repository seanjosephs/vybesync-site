# vybesync-site — marketing site (Claude Code orientation)

VybeSync's public-facing marketing landing page. Production: https://vybesync.io. This is brand surface, not product surface.

## Drift-check before any work

1. Read https://vybesync.io live to see current copy and visual design
2. Read Obsidian vault `And Here's My Secret` → `Business Ideas/VybeSync/VybeSync — State of the System.md` (esp. topology + tagline section)
3. If changing copy: read `Business Ideas/VybeSync/VybeSync — Brand Finalization, Pitch Deck, and GitHub Setup.md` for brand voice context
4. Report deltas before working

## End-of-session protocol

If copy or layout changed materially, update `State of the System` (the topology/branding section) and append to `Operational Log`.

## Repo specifics

- **This is the canonical surface for the marketing tagline and framing.** If hub.html, the staff app, the design system docs, or any other surface disagrees on copy, the marketing site wins (Decisions Log #13).
- Current canonical tagline: **"in pilot · five rooms / in sync. present."**
- No login, no auth, no Supabase. Static site. Email capture is the conversion event.
- Brand voice on the live site: anti-extraction, pro-circulation, present over performative. Reference line: *"vybesync doesn't extract value from live music, performance, or theatre ecosystems. It circulates it."*

## Hard rules

- Don't drift the tagline. If it changes, change it here first and propagate to other surfaces.
- Don't add product UI (this is brand, not product).
- Don't add tracking pixels, ads, or anything extractive — it would directly contradict the manifesto on the page.
- Don't use the banned phrases (see Voice contract below).

## Voice contract

Naomi default (Decisions Log #9). See `user_preferences`.

**Banned vocabulary** (Decisions Log #15, full list in `VybeSync — Brand Voice & Vocabulary`): the word **"mark"** is banned in any visual-design context. Substitutes: **wave** (icon), **word only logo** (text), **wave and word combined logo** (full lockup, default when "logo" is used alone). External quotations exempt.

**Author voice (non-app-facing writing):** For any writing where Sean Josephs is the author — founder documents, essays, public statements, LinkedIn posts, thought leadership, pitch materials — apply the brand voice defined in the brand-voice plugin. Canonical settings: `plugin_015ay6vzri9r8cLwi95ZUY9R/settings/brand-voice.local.md`. For long-form drafts, invoke the `seanai` skill. For checking finished drafts, invoke `brand-voice:brand-voice-enforcement`. VybeSync app-facing copy (UI, in-app text, product communications) follows `vybesync-design-system` instead. When ambiguous, ask.

## Design system

If/when `seanjosephs/vybesync-design-system` covers marketing surfaces, consume from it. Until then, the marketing site can have its own visual system separate from the apps — but the logo colors (vybe white + sync orange) and core type choices should match.
