# Genius (genius)

Crowdsourced music knowledge — the Genius/Rap Genius platform. The Genius API
exposes structured metadata for songs, artists, albums, annotations,
referents, and contributors. Raw lyric text is not served by the API;
consumers receive the public song page URL and scrape lyrics from there.

**APIs.yml:** [apis.yml](apis.yml)

## Type

- **x-type:** company
- **x-tier:** 2 — enriched with OpenAPI, Naftiko capabilities, JSON Schemas, vocabulary, plans, and rate limits.
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Music

## API

- **Genius** — [Documentation](https://docs.genius.com/) · base URL `https://api.genius.com`

### Endpoints covered in the OpenAPI

`Account`, `Search`, `Songs` (4 ops), `Artists` (6 ops), `Albums` (5 ops),
`Annotations` (8 ops incl. create/delete/vote), `Referents` (2 ops),
`Web Pages` (1 op), `Users` (2 ops). 29 operations total.

## Authentication

- **OAuth 2.0** (authorization code) — scopes: `me`, `create_annotation`, `manage_annotation`, `vote`
- **Client Access Token** — long-lived bearer token issued at https://genius.com/api-clients; suitable for read-only endpoints
- App registration: [genius.com/api-clients](https://genius.com/api-clients)

## Artifacts

### OpenAPI
- [openapi/genius-openapi.yml](openapi/genius-openapi.yml) — 29 operations, full component schemas.

### Spectral Ruleset
- [rules/genius-rules.yml](rules/genius-rules.yml) — enforces snake_case paths/parameters, OAuth2 scope completeness, meta envelope shape, and Genius-specific pagination conventions.

### Naftiko Capabilities (one per OpenAPI tag)
- [capabilities/genius-account.yaml](capabilities/genius-account.yaml)
- [capabilities/genius-search.yaml](capabilities/genius-search.yaml)
- [capabilities/genius-songs.yaml](capabilities/genius-songs.yaml)
- [capabilities/genius-artists.yaml](capabilities/genius-artists.yaml)
- [capabilities/genius-albums.yaml](capabilities/genius-albums.yaml)
- [capabilities/genius-annotations.yaml](capabilities/genius-annotations.yaml)
- [capabilities/genius-referents.yaml](capabilities/genius-referents.yaml)
- [capabilities/genius-web-pages.yaml](capabilities/genius-web-pages.yaml)
- [capabilities/genius-users.yaml](capabilities/genius-users.yaml)

Every capability file is self-contained — inline `consumes` + `rest` exposer + `mcp` exposer.

### JSON Schema
- [json-schema/genius-song-schema.json](json-schema/genius-song-schema.json)
- [json-schema/genius-artist-schema.json](json-schema/genius-artist-schema.json)
- [json-schema/genius-album-schema.json](json-schema/genius-album-schema.json)
- [json-schema/genius-annotation-schema.json](json-schema/genius-annotation-schema.json)
- [json-schema/genius-referent-schema.json](json-schema/genius-referent-schema.json)
- [json-schema/genius-user-schema.json](json-schema/genius-user-schema.json)
- [json-schema/genius-web-page-schema.json](json-schema/genius-web-page-schema.json)

### JSON Structure
- [json-structure/genius-song-structure.json](json-structure/genius-song-structure.json)
- [json-structure/genius-annotation-structure.json](json-structure/genius-annotation-structure.json)

### JSON-LD
- [json-ld/genius-context.jsonld](json-ld/genius-context.jsonld) — maps Genius entities to schema.org (MusicComposition, MusicGroup, MusicAlbum, Comment) and the Music Ontology.

### Examples
- [examples/genius-search-example.json](examples/genius-search-example.json)
- [examples/genius-get-song-example.json](examples/genius-get-song-example.json)
- [examples/genius-get-artist-example.json](examples/genius-get-artist-example.json)
- [examples/genius-list-artist-songs-example.json](examples/genius-list-artist-songs-example.json)
- [examples/genius-get-referents-example.json](examples/genius-get-referents-example.json)
- [examples/genius-get-annotation-example.json](examples/genius-get-annotation-example.json)
- [examples/genius-lookup-web-page-example.json](examples/genius-lookup-web-page-example.json)

### Vocabulary
- [vocabulary/genius-vocabulary.yml](vocabulary/genius-vocabulary.yml)

### Plans
- [plans/genius-plans-pricing.yml](plans/genius-plans-pricing.yml) — free developer tier only.

### Rate Limits
- [rate-limits/genius-rate-limits.yml](rate-limits/genius-rate-limits.yml) — undocumented; treat as ~1 req/sec per token.

## Community SDKs

Genius does not publish official SDKs. Notable community wrappers:

- Python — [LyricsGenius](https://github.com/johnwmillr/LyricsGenius), [wrap-genius](https://github.com/fedecalendino/wrap-genius)
- Node.js — [genius-api](https://github.com/jahrlin/genius-api), [node-genius](https://github.com/bookercodes/node-genius)
- Ruby — [timrogers/genius](https://github.com/timrogers/genius)
- PHP — [Genius-PHP](https://github.com/simivar/Genius-PHP)
- R — [geniusr](https://cran.r-project.org/web/packages/geniusr/)

## MCP Servers (Community)

- [jchoi2x/genius-mcp](https://github.com/jchoi2x/genius-mcp) — TypeScript / Cloudflare Workers; exposes `genius-search-song`, `genius-song-lyrics`, `genius-list-artist-songs`.
- [federicogarciav/genius-mcp](https://mcpservers.org/servers/federicogarciav/genius-mcp)
- [Sergiolm17/genius-mcp-server](https://mcp.so/server/genius-mcp-server/Sergiolm17)

## Tags

Music, Lyrics, Annotations, Crowdsourced, Reference Data, Public APIs

## Notes

- The Genius GitHub org ([github.com/Genius](https://github.com/Genius)) is almost entirely Ruby infrastructure forks (Heroku buildpacks, Rails internals, deprecated tooling). The only API-relevant repo is [omniauth-genius](https://github.com/Genius/omniauth-genius) (OAuth strategy).
- The API does **not** return raw lyric text. Use `Song.url` to fetch the public song page and scrape lyrics from there. This is a hard product/licensing constraint, not a missing endpoint.
- Genius applies soft fair-use throttling. Treat ~1 request per second per token as a safe upper bound for sustained workloads.

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## Maintainers

- **Kin Lane** — kin@apievangelist.com
