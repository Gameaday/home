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
| 2026-10-24 | pre-launch | — | — | — | Housekeeping sweep: MIT licenses added to 6 repos (Media-Maid, FrictionPoint, Stream-Doctor, Metatron, Herald, Cerberus); Stream-Doctor README written; ia-helper launch issue templates + MANAGE_EXTERNAL_STORAGE audit issue #75; suite roadmap pointers added to Herald/Havoc/Chronical/Cerberus. Open flag: Stream-Doctor design doc assumes a subscription, which breaks rule 2 — revisit before any build work. |

## Related repos

- ia-helper — Phase 1 flagship (Internet Archive companion)
- Elagato-Media-Maid — Phase 2 (media organizer / FileBot alternative)
- FrictionPoint — Phase 3 (system diagnostics, Rust, SBC-first)
- TShock_Metatron / _Herald / _Cerberus / _Chronical / _Havoc — Phase 4 suite
- Gameaday/historylabs.dev — storefront, tutorials, archive site
- Stream-Doctor — unscheduled (Windows streamer diagnostics; design doc exists, pricing conflicts with rule 2)

*Written October 2026 so future-us does not lose the plot.*
