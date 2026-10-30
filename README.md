# Genius

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

Crowdsourced music knowledge — the Genius/Rap Genius platform. The Genius API exposes structured metadata for songs, artists, albums, annotations, referents, and contributors. Raw lyric text is not served by the API; consumers receive the public song page URL and scrape lyrics from there.

**Areas:** Music · Lyrics · Annotation · Crowdsourced · Reference Data · Public APIs

## Genius on APIs.io

Everything profiled for Genius is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/genius/](https://apis.io/providers/genius/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Genius Account API](https://apis.io/apis/genius/genius-account-api/) — Authenticated user account.
- [Genius Albums API](https://apis.io/apis/genius/genius-albums-api/) — Album metadata, tracks, cover art, and leaderboards.
- [Genius Annotations API](https://apis.io/apis/genius/genius-annotations-api/) — Community annotations attached to lyric fragments.
- [Genius Artists API](https://apis.io/apis/genius/genius-artists-api/) — Artist profiles, discography, followers, and leaderboards.
- [Genius Referents API](https://apis.io/apis/genius/genius-referents-api/) — Lyric fragments (referents) and their attached annotations.
- [Genius Search API](https://apis.io/apis/genius/genius-search-api/) — Full-text search across the Genius corpus.
- [Genius Songs API](https://apis.io/apis/genius/genius-songs-api/) — Song metadata, contributors, and activity.
- [Genius Users API](https://apis.io/apis/genius/genius-users-api/) — Genius user profiles and contributions.
- [Genius Web Pages API](https://apis.io/apis/genius/genius-web-pages-api/) — Web page lookup for the annotation network.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Genius Agentic Access](https://apis.io/agentic-access/genius/genius-agentic-access/)

#### JSON Schema (7)

The data models the API reads and writes.

- [GeniusAlbum](https://apis.io/schemas/genius/genius-album/)
- [GeniusAnnotation](https://apis.io/schemas/genius/genius-annotation/)
- [GeniusArtist](https://apis.io/schemas/genius/genius-artist/)
- [GeniusReferent](https://apis.io/schemas/genius/genius-referent/)
- [GeniusSong](https://apis.io/schemas/genius/genius-song/)
- [GeniusUser](https://apis.io/schemas/genius/genius-user/)
- [GeniusWebPage](https://apis.io/schemas/genius/genius-web-page/)

#### JSON Structure (2)

Data models expressed in JSON Structure.

- [Genius Annotation Structure](https://apis.io/json-structure/genius/genius-annotation-structure/)
- [Genius Song Structure](https://apis.io/json-structure/genius/genius-song-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Genius Context](https://apis.io/jsonld/genius/genius-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Genius API Vocabulary](https://apis.io/vocabularies/genius/genius-vocabulary/)

#### Examples (7)

Example requests and responses.

- [Genius Get Annotation Example](https://apis.io/examples/genius/genius-get-annotation-example/)
- [Genius Get Artist Example](https://apis.io/examples/genius/genius-get-artist-example/)
- [Genius Get Referents Example](https://apis.io/examples/genius/genius-get-referents-example/)
- [Genius Get Song Example](https://apis.io/examples/genius/genius-get-song-example/)
- [Genius List Artist Songs Example](https://apis.io/examples/genius/genius-list-artist-songs-example/)
- [Genius Lookup Web Page Example](https://apis.io/examples/genius/genius-lookup-web-page-example/)
- [Genius Search Example](https://apis.io/examples/genius/genius-search-example/)

#### Collections (10)

Postman and Open Collection request collections.

- [Genius API](https://apis.io/collections/genius/open-genius/)
- [Genius Account API](https://apis.io/collections/genius/open-genius-account-api/)
- [Genius Account Albums API](https://apis.io/collections/genius/open-genius-albums-api/)
- [Genius Account Annotations API](https://apis.io/collections/genius/open-genius-annotations-api/)
- [Genius Account Artists API](https://apis.io/collections/genius/open-genius-artists-api/)
- [Genius Account Referents API](https://apis.io/collections/genius/open-genius-referents-api/)
- [Genius Account Search API](https://apis.io/collections/genius/open-genius-search-api/)
- [Genius Account Songs API](https://apis.io/collections/genius/open-genius-songs-api/)
- [Genius Account Users API](https://apis.io/collections/genius/open-genius-users-api/)
- [Genius Account Web Pages API](https://apis.io/collections/genius/open-genius-web-pages-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Genius — jsonschema rules](https://apis.io/rules/genius/genius-jsonschema-spectral-rules/)
- [Genius API Rules](https://apis.io/rules/genius/genius-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Genius Authentication](https://apis.io/security/genius/genius-authentication/)
- [Genius Domain Security](https://apis.io/security/genius/genius-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Genius Scopes](https://apis.io/scopes/genius/genius-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Genius Plans Pricing](https://apis.io/plans/genius/genius-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Genius Rate Limits](https://apis.io/rate-limits/genius/genius-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://genius.com/)
- [Terms of service](https://genius.com/static/terms)
- [GitHub](https://github.com/Genius)

## API Evangelist rating

**Kin Score 34.4** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 28.9 |
| Contract governance | 27.3 |
| Operational transparency | 2.6 |
| Developer ergonomics | 41.7 |
| Access clarity | 28.9 |

**Agent readiness 24.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/genius/](https://apis.io/providers/genius/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Genius: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/genius/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
