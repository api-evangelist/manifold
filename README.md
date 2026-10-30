# Manifold

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Manifold is an NFT creator tools platform that empowers artists and developers to deploy their own creator-owned smart contracts, mint NFTs, and build custom on-chain experiences without relying on platform-specific custody. Founded in 2021, Manifold provides a no-code studio (Manifold Studio) for ERC721 and ERC1155 contract deployment, open-source Creator Core smart contracts, a Royalty Registry adopted by all major NFT marketplaces, and a Client SDK for building custom minting dApps. The platform supports Ethereum Mainnet, Base, Optimism, Shape, Apechain, and Sepolia testnet. Manifold also exposes server-side authentication APIs (Signature Grant and Authorization Code Grant via oauth2.manifoldxyz.dev), a Studio Apps REST API (apps.api.manifoldxyz.dev) for product and minting data, open-source Solidity extension contracts for custom mint mechanics, and a Marketplace contract powering auction and fixed-price listings. Gas fees are the only cost for creators; Manifold charges no platform fees or royalties on sales.

**Areas:** NFT · Creator Tools · Smart Contracts · Blockchain · Web3 · Ethereum · ERC-721 · ERC-1155 · Royalties · Marketplace · Minting · OpenSea

## Manifold on APIs.io

Everything profiled for Manifold is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/manifold/](https://apis.io/providers/manifold/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Manifold Creator Core Smart Contracts](https://apis.io/apis/manifold/creator-core-contracts/) — Open-source Solidity smart contract framework for deploying ERC721 and ERC1155 creator-owned NFT contracts. Provides minting, metadata modification,…
- [Manifold Studio Apps API](https://apis.io/apis/manifold/studio-apps-api/) — REST API backing Manifold's Client SDK, providing product instance data and purchase preparation information for minting dApps. Used to fetch Edition and…
- [Manifold Royalty Registry](https://apis.io/apis/manifold/royalty-registry/) — On-chain smart contract registry that serves as a single source of truth for NFT royalties across all major marketplaces. Provides setRoyaltyLookupAddress()…
- [Manifold Marketplace Contracts](https://apis.io/apis/manifold/marketplace-contracts/) — Smart contract system powering Manifold Gallery listings and Marketplace Widgets. Supports Auction Listings (single NFT with bidding, configurable floor…
- [Manifold Claim Widgets](https://apis.io/apis/manifold/claim-widgets/) — JavaScript widget library for embedding NFT minting and claim flows into any website or dApp. Served from claims.manifoldxyz.dev, current version 1.16.1.…
- [Manifold Authorization Code Grant API](https://apis.io/apis/manifold/manifold-authorization-code-grant-api/) — Exchange a one-time authorization code for a long-lived access token allowing server-side access to private user data.
- [Manifold Signature Grant API](https://apis.io/apis/manifold/manifold-signature-grant-api/) — Validate a wallet signature session token to confirm a user's wallet address server-side.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Manifold Agentic Access](https://apis.io/agentic-access/manifold/manifold-agentic-access/)

#### JSON Schema (1)

The data models the API reads and writes.

- [Manifold OAuth2 Authentication API Schemas](https://apis.io/schemas/manifold/manifold-oauth2-authentication/)

#### Collections (2)

Postman and Open Collection request collections.

- [Manifold OAuth2 Authentication Authorization Code Grant API](https://apis.io/collections/manifold/open-manifold-authorization-code-grant-api/)
- [Manifold OAuth2 Authentication Authorization Code Grant Signature Grant API](https://apis.io/collections/manifold/open-manifold-signature-grant-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Manifold — jsonschema rules](https://apis.io/rules/manifold/manifold-jsonschema-spectral-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Manifold Domain Security](https://apis.io/security/manifold/manifold-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Manifold Plans Pricing](https://apis.io/plans/manifold/manifold-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Manifold Rate Limits](https://apis.io/rate-limits/manifold/manifold-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Manifold Finops](https://apis.io/finops/manifold/manifold-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://manifold.xyz)
- [Documentation](https://docs.manifold.xyz)
- [Blog](https://manifoldxyz.substack.com)

## API Evangelist rating

**Kin Score 25.2** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 49.6 |
| Contract governance | 9.8 |
| Operational transparency | 13.2 |
| Developer ergonomics | 21.4 |
| Access clarity | 5.3 |

**Agent readiness 26.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 5.9** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/manifold/](https://apis.io/providers/manifold/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Manifold: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/manifold/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
