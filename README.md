# The Forge Protocol
**Toward a Digital Society of Wealthy Creative Sovereigns**

The Forge Protocol is an attempt ~ still being stress-tested and revised ~ to build an open, composable culture and commerce protocol for creator communities in emerging markets. The core question driving it: what would it actually look like if creators owned their infrastructure instead of renting algorithmic feeds? We think the answer might involve something we're calling Take-Home Efficiency (THE), alongside other indicators of creative wealth we haven't fully defined yet. We're building new ways for creative commerce and experimentation across various emerging market communities, and we don't yet know which of those will hold.

This repository contains the smart contracts, compliance dashboards, and commerce pipelines we're experimenting with to run a **D.A.M.N.** (Digital Alternative Media Network).

***

## 🏗 System Architecture

We're designing the protocol around an ecology of clusters, operating on three primary media organs. These structures are provisional, they reflect our best current thinking.

### Network Evolution
Creators move through the protocol along a suggested functional progression. Whether this progression holds in practice is something we're actively trying to learn:
1. **Seed Cluster:** 3 to 15 creators. An opt-in forming stage where initial commitments are posted to the ledger.
2. **D.A.M.N. (Digital Alternative Media Network):** Clusters that have crossed into producing tangible media artifacts and returning data/value back to the commons.
3. **D/DAMN (Decentralized Autonomous Media Network):** Long-running, steward-led clusters that we hope will become portable enough to coordinate beyond our immediate rails ~ though this stage is largely theoretical at this point.

### The Three Organs
*   **Music (Live & Production):** Event ticketing pipelines, venue check-ins, and royalty collection routing, aimed at recovering streaming leakage that we're still measuring.
*   **Merch (Curated Drops):** An asset-light seasonal drops framework designed to protect creators from upfront inventory risk. We're still validating whether the margins hold.
*   **Media (AI Tooling):** A localized AI tooling suite (audio, video, transcription) accessed via an internal credit rail (Seeds), intended to lower production costs below standalone global SaaS subscriptions. The actual cost delta is something we're working to quantify.

***

## 🧮 Telemetry & Mathematical Specification (v1.0)

We want to prioritize falsifiability over optimism ~ which means being honest that these metrics are first drafts. The protocol is intended to be governed by a live telemetry spec with deterministic queries, but the queries themselves are still being refined. We track six top-line metrics that we *think* tell us whether the infrastructure is extracting undue value from the creator.

**1. Take-Home Efficiency (THE)**
*   **Definition:** The ratio of net earnings received by the creator versus the gross amount paid by the buyer.
*   **Formula:** `THE = Σ(Net Creator Earnings) / Σ(Gross Transaction Value)`
*   **Suggested Target:** `≥ 0.70` on the primary corridor.
*   **Variables Being Tracked:** Gateway fees, foreign exchange (FX) spreads, last-mile processing stacks.

**2. Sovereign Cash Latency (SCL)**
*   **Definition:** The median number of hours from when funds are cleared to when they are spendable by the creator.
*   **Formula:** `SCL = Median(T_spendable - T_cleared)`
*   **Suggested Target:** `≤ 24 hours` (Q1) $\to$ `≤ 4 hours` (End of Year 1). We're not certain this is achievable on all corridors.

**3. Commitment Fulfillment Rate (CFR)**
*   **Definition:** The percentage of posted peer-to-peer commitments (e.g., studio time, design work) fulfilled on time within a cluster.
*   **Formula:** `CFR = (Fulfilled Commitments) / (Total Posted Commitments)`
*   **Suggested Target:** `≥ 0.70` at the cell level. What counts as "on time" is still being negotiated with early clusters.

**4. Direct-Reach Share (DRS)**
*   **Definition:** The portion of the audience reachable without interference from an algorithmic gatekeeper.
*   **Formula:** `DRS = (Direct Audience Contacts) / (Total Aggregated Audience)`
*   **Suggested Target:** Scaling from `0.10` to `0.30`. We don't yet know if 0.30 is a ceiling or a floor.

**5. Functioning DAMNs**
*   **Definition:** The count of Seed Clusters crossing the functional production threshold per quarter.
*   **Suggested Target:** `≥ 2 clusters` by end of Year 1. This is our minimal viable signal that the model converts.

**6. 12-Month Creator Retention**
*   **Definition:** The percentage of creators who remain active and earning across two or more rails after one year.
*   **Formula:** `Retention = (Active Creators at T_12) / (Cohort Creators at T_0)`
*   **Suggested Target:** `≥ 50%`. We chose this threshold because it felt meaningful, but it may shift as we learn more.

### Falsifiability Conditions
We're proposing that the protocol should be considered a failure and restructured if, after 3 years, any of the following hold ~ though we're open to revising what counts as failure as we understand the context better:
1. `THE < 0.70` on the primary corridor (unattributable to sudden regulatory/FX shocks).
2. Seed Clusters fail to convert to DAMNs at a rate visible above standard cohort noise.
3. D/DAMN stage exits exceed entries for four consecutive quarters without external shocks.

***

## 🔗 On-Chain Scope & Tokenomics

We're using on-chain infrastructure only where we believe it genuinely solves a real problem ~ and we're trying to aggressively penalize speculation, though the right mechanisms for that are still being worked out.

**What we're exploring putting on-chain:**
*   **Provenance of Drops:** Cryptographic authenticity for physical merch and secondary-market legibility.
*   **Transparent Commons Accounting:** Inflows, disbursements, and steward votes logged for public audit.
*   **Auditable Commissions:** Immutable records of issued creator commissions.
*   **Reputation Receipts:** Optional, portable verification of a creator's track record.

**What we're keeping off-chain:**
*   **Identity (PII):** Personally identifiable information in secure off-chain identity stores.
*   **Low-effort vanity collectibles** and **speculation-gated access** ~ neither solves a creator problem we can identify.

**The "Seeds" Unit:**
*   Seeds are internal tooling credits earned by contributing (stewardship, content, teaching).
*   They're spent on AI tools and Academy access.
*   *Crucial Constraint We're Holding:* Seeds are intentionally **not cash-convertible** at the protocol level. This is our attempt to prevent the Forge from becoming a spot market ~ but we're watching to see whether this constraint creates unintended friction.

***

## 🛠 Suggested Next Steps

These are working hypotheses about where to focus, not a fixed roadmap. We expect this list to change.

**Immediate Research & Build Questions:**
*   [ ] What compliance integrations are actually feasible on the primary corridors at scale?
*   [ ] Can we build withdrawal pipelines that reliably enforce the SCL `< 24h` discipline ~ and what breaks when we try?
*   [ ] Asset-light Merch Drops pipeline ~ we need a live end-to-end test before we know if this holds.
*   [ ] Commitment ledger for Seed Clusters: can we make it genuinely append-only and offline-tolerant?
*   [ ] Opt-in consent scopes ~ are the configurations we've designed actually usable by creators who aren't technical?
*   [ ] Fee floor logic to protect creator net earnings ~ ensuring 0% take-home never occurs. The edge cases here are still unclear.

**Longer-Horizon Questions (Revisit After Early Stability):**
*   [ ] What would a cross-pollination discovery engine actually look like without recreating algorithmic dependency?
*   [ ] Micro-advances against future sales ~ what's the risk model, and who bears it?
*   [ ] AI training-data royalty rail for opted-in creators ~ we believe this matters, but the infrastructure doesn't exist yet.

***

## 🤝 Contributing

We're building in the open because we think the questions are harder than any single team can answer. We're currently scaling compliance dashboards, story-first product pages, and smart contracts for merch provenance ~ all works in progress.

*   **Developers:** Open issues are tagged `core-infrastructure` and `telemetry`. The commitment ledger and fee floor logic are the most uncertain and most needed.
*   **Data Scientists:** The queries for THE and SCL are early drafts. Review the `telemetry-spec` directory ~ we genuinely don't know if we're measuring the right things yet.
*   **Creators:** Find a Seed Cluster, post your commitments, and start coordinating. Your experience with the system is the most important data we have.
