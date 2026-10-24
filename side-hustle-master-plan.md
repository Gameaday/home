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
| 2026-10-24 | pre-launch | — | — | — | Round 6 — Terrawinia vision parked: deterministic bot platform (no LLM in runtime), modes as configs over one core (backfill bots → Idle Terraria → Dynasty → Terrawinia faction wars). Validated gap: no shippable Terraria bot plugin exists despite public demand. Support contracts + sponsored-feature early-access windows documented as the second sanctioned rule-2 exception (metered labor). Phase 4 gate unchanged; ceiling revised from ~$1.5k/yr to ~$15k/yr done-well. Full plan: terrawinia-suite-plan.md. |

## Related repos

- ia-helper — Phase 1 flagship (Internet Archive companion)
- Elagato-Media-Maid — Phase 2 (media organizer / FileBot alternative)
- FrictionPoint — Phase 3 (system diagnostics, Rust, SBC-first)
- TShock_Metatron / _Herald / _Cerberus / _Chronical / _Havoc — Phase 4 suite
- Gameaday/historylabs.dev — storefront, tutorials, archive site
- Stream-Doctor — unscheduled (Windows streamer diagnostics; Free + one-time Pro + Live-Data subscription, the sanctioned rule-2 exception)
- Terrawinia — Terraria bot platform & mode suite (terrawinia-suite-plan.md, this repo) — Phase 4+ vision, parked Oct 2026. Support contracts recorded as the second sanctioned rule-2 exception.

*Written October 2026 so future-us does not lose the plot.*
