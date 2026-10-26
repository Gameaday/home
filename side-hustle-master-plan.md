# Side Hustle Master Plan — Nov 2026 → Oct 2027

One year, four products, one audience: people who want to own their digital tools.
This file is the source of truth. Each product repo carries its own ROADMAP.md with phase detail.

## The bet

Build with AI, never serve AI. Sell ownership, not subscriptions. Keep marginal cost at zero.
Pick underserved niches where the incumbent overcharges or simply does not exist.

## The rules (apply to every product, no exceptions)

1. **AI builds it; the product never bills AI.** AI is the construction crew, not a metered runtime feature. If an AI feature is ever demanded, it ships as an offline batch job or a hard-capped quota.
2. **One-time pricing.** Lifetime / per-license purchases. No subscriptions unless a feature has real per-user costs (and then think twice).
3. **Zero marginal cost per user.** Local-first desktop/mobile apps. The only shared cost is a static landing page.
4. **Free tiers are marketing, not crippleware.** Nobody is locked out of the core job; people pay because they work harder in the tool.
5. **Maintenance budget: ≤ 2 hrs/week per shipped product.** If a product exceeds it, cut scope, not sleep.
6. **A new phase only starts if the previous gate is green.** The calendar is the default, not a contract.

## Sanctioned rule-2 exception

**Stream-Doctor: three-tier model approved (2026-10-24, Carl).** Principle: *own what is permanent, rent only what needs constant feeding.*

- **Free** — static local checks, forever.
- **Pro (one-time)** — permanent local features: USB Sentinel, Frame Pacing Doctor, OBS Link, Snapshot & Restore.
- **Live-Data (subscription)** — only features that hit current, maintained driver/device knowledge; the hardware landscape keeps shifting, so this has genuine per-user ongoing cost. Possible later addition: opt-in secure cloud backups (real storage cost → subscription tier only).

This is the only sanctioned subscription; all other products remain one-time. Tier detail: Stream-Doctor/ROADMAP.md.

## Year at a glance

| Phase | Months | Product | Detailed plan | Gate (go / no-go) |
|---|---|---|---|---|
| 1 | Nov 2026 – Jan 2027 | IA Helper Pro | ia-helper/ROADMAP.md | ≥ 30 Pro sales |
| 2 | Feb – Apr 2027 | MediaMaid standalone app | Elagato-Media-Maid/ROADMAP.md | ≥ 25 lifetime sales |
| 3 | May – Jul 2027 | FrictionPoint Pro | FrictionPoint/ROADMAP.md | ≥ 25 Pro sales |
| 4 | Aug – Oct 2027 | TShock server suite + Havoc | TShock_Metatron/ROADMAP.md | ≥ 15 server licenses (bonus phase) |

## Cross-cutting infrastructure (build during Phase 1–2, reuse all year)

- **One storefront** (historylabs.dev/shop): all products, lifetime keys, founding pricing visible on day one.
- **One email list**: every app's About screen links to it. This list — not any single app — is the actual asset.
- **One merchant-of-record account** (Lemon Squeezy-class: ~5% + 50¢, handles global VAT) plus the Play Console account (15% fee on first $1M/yr).
- **Quarterly review ritual**: at each gate, write three lines in the log below — installs, sales, decision.

## Gate policy

- **Green** → next phase starts on schedule.
- **Yellow** (50–100% of target) → one month deepening the current product, then re-check.
- **Red** → no new product starts. Diagnose first: wrong niche, wrong price, or not enough distribution.

## Review log

| Date | Phase | Installs | Sales | Decision | Notes |
|---|---|---|---|---|---|
| 2026-10-24 | pre-launch | — | — | — | Housekeeping sweep: MIT licenses added to 6 repos (Media-Maid, FrictionPoint, Stream-Doctor, Metatron, Herald, Cerberus); Stream-Doctor README written; ia-helper launch issue templates + MANAGE_EXTERNAL_STORAGE audit issue #75; suite roadmap pointers added to Herald/Havoc/Chronical/Cerberus. Resolved same day: Stream-Doctor subscription model approved by Carl — hardware/driver churn means continuous improvements, which justifies recurring pricing. Recorded as the sanctioned rule-2 exception. |
| 2026-10-24 | pre-launch | — | — | — | Round 2: Stream-Doctor refined to three tiers (Free / one-time Pro / Live-Data subscription; cloud backups later, subscription-only); Stream-Doctor ROADMAP.md created; FrictionPoint README expanded from stub. ia-helper audit: PRIVACY_POLICY.md already present — no gap. |
| 2026-10-24 | pre-launch | — | — | — | Round 3 — portfolio audit: PRELAUNCH_AUDIT.md added to all five projects (scope-fit, tier design, polish, as-is vs 1.0, ordered steps). Key findings: ia-helper batch-download free/Pro conflict (recommended split in audit, decide before Pro launch); MediaMaid transcode deferral past 1.0; Stream-Doctor cut to pre-flight + USB Sentinel for v1.0 (highest sprawl risk); Metatron/Cerberus overlap to resolve at Phase 4; FrictionPoint 1.0 bar defined pre-code. November keep-alive plan filed: ia-helper #76 — internal-testing upload satisfies Google's inactive-account policy; closed testing (12 testers/14 days) starts first week of Nov for late-Nov production eligibility. |
| 2026-10-24 | pre-launch | — | — | — | Round 4 — execution: ia-helper tidied for internal testing (scratch files removed, README Play badge fixed to real applicationId, broken headers repaired, internal-testing-readiness.md added); MediaMaid marketplace pass (Node.js debug disabled in manifest, versions aligned, CHANGELOG + CI + Elgato submission checklist per the official plugin guidelines); TShock suite audit landed in Metatron — Metatron confirmed as the original monolith, split into Cerberus (Gate) / Herald (Voice) / Chronical (Memory, never built), Havoc the later flagship; recommendations: keep one Gate (re-scope Metatron to the Scribe or fold into Cerberus), build-or-archive Chronical at the Phase 3 gate; Chronicle README rewritten from raw AI chat into a proper design doc. |
| 2026-10-24 | pre-launch | — | — | — | Round 5 — package identity: applicationId switched to **com.gameaday.iahelper** (Carl's preference, applied pre-publication while the choice was still free; permanent once the Play entry exists). Consistent with com.gameaday.mediamaid; code namespace deliberately unchanged. Docs, README badge, and manifest metadata aligned. |
| 2026-10-24 | pre-launch | — | — | — | Round 6 — Terrawinia vision parked: deterministic bot platform (no LLM in runtime), modes as configs over one core (backfill bots → Idle Terraria → Dynasty → Terrawinia faction wars, since renamed Faction Wars). Validated gap: no shippable Terraria bot plugin exists despite public demand. Support contracts + sponsored-feature early-access windows documented as the second sanctioned rule-2 exception (metered labor). Phase 4 gate unchanged; ceiling revised from ~$1.5k/yr to ~$15k/yr done-well. Full plan: choir-suite-plan.md (renamed in Round 7). |
| 2026-10-24 | pre-launch | — | — | — | Round 7 — ecosystem rename: **Terrawinia → Choir** (Carl's pick). Names the system property — many deterministic agents, one score — and matches the angelic block lineage (Metatron, Cerberus, Herald, Havoc, Chronical are already voices; the suite is the choir). Core engine → Choir Core; mode 4 → Faction Wars. Collision check clean: no TShock/Terraria plugin or gaming-brand conflicts in the niche. Plan doc renamed to choir-suite-plan.md. Open question #4 now reads: brand the show "Choir" or run it under the Gameaday umbrella? |
| 2026-10-24 | pre-launch | — | — | — | Round 8 — full-time roadmap: goal reframed from $50k/yr to a real path off a $200k job (~$215k total comp). 4th step = mode shift, not new product: Choir Managed fleet + premium commissions ("Choir Live"), with the no-hour-without-an-asset productization rule. Quit gates F1–F3 defined (fleet scale Apr 2028 at ≥15 servers; quit evaluation from Apr 2029 at trailing 12mo ≥ $100k, ≥50% recurring, 18–24mo runway). Anti-race-to-zero pricing rules added. Doc: road-to-full-time.md. |
| 2026-10-25 | pre-launch | — | — | — | Round 9 — pipeline & UI priority: ia-helper CI green again (analyze/test/APK all pass; all 16 audit bugs #12–#27 fixed; `dart analyze --fatal-warnings` clean). Support contact corrected repo-wide to admin@historylabs.dev (gameaday.project@gmail.com was never owned by the project); privacy policy to be hosted at a public URL (historylabs.dev recommended). Merges: Elagato-Media-Maid #17 (reliability & performance hardening) and historylabs #2 (foundation pass: house style, site validator, CI) merged; historylabs CI activated (`0eb10dc`); stale Metatron sentinel PRs #67/#68 closed — a stronger ping-injection fix was already on main. Priority set by Carl: Material Design UI pass (ia-helper #79) before the Play push — theme phase 1 landed (`ddce204`: unified light/dark theme builder, full M3 component coverage); then closed testing per ia-helper #76 (12 testers / 14 days) with late-Nov production eligibility. |
| 2026-10-26 | pre-launch | — | — | — | Round 10 — latest-Zensical canaries & dead-link purge: historylabs and atlasofpelvicsurgery CI both now gate on pinned Zensical 0.0.62 and run a weekly canary job against the latest PyPI release (0.0.72) with full failure logs posted to the PR; atlas is green on 0.0.72. All 39 historylabs 0.0.72 dead-link warnings fixed (PR #6): Zensical reserves `docs_dir/templates`, so the five template pages never rendered — moved to `artifacts-templates/` with every inbound link, nav entry, validator glob, and pathfinder URL updated; one more 0.0.72 regression fixed (`.env.example` → `env.example`, since 0.0.72 stops copying dotfiles into the site). historylabs verify + canary both green; live site needs a redeploy (Pi rsync) to serve the fixes. |

## Related repos

- ia-helper — Phase 1 flagship (Internet Archive companion)
- Elagato-Media-Maid — Phase 2 (media organizer / FileBot alternative)
- FrictionPoint — Phase 3 (system diagnostics, Rust, SBC-first)
- TShock_Metatron / _Herald / _Cerberus / _Chronical / _Havoc — Phase 4 suite
- Gameaday/historylabs.dev — storefront, tutorials, archive site
- Stream-Doctor — unscheduled (Windows streamer diagnostics; Free + one-time Pro + Live-Data subscription, the sanctioned rule-2 exception)
- Choir (formerly Terrawinia) — Terraria bot platform & mode suite (choir-suite-plan.md, this repo) — Phase 4+ vision, parked Oct 2026. Support contracts recorded as the second sanctioned rule-2 exception.
- Road to full time — Year 2+ quit plan (road-to-full-time.md, this repo)

*Written October 2026 so future-us does not lose the plot.*
