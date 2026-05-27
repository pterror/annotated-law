# annotated-law

Plain-language summaries of legislation with citations to primary sources. Phase 0 targets UK tenancy law — ingesting statutes from legislation.gov.uk, structuring them through an intermediate representation, and serving searchable, annotated summaries via an Astro frontend.

## Dev setup

```sh
nix develop        # enter the dev shell (provides bun)
bun install        # install dependencies
bun run dev        # start the Astro dev server
```

## Project layout

| Path | Purpose |
|------|---------|
| `src/ingest/` | Fetch and parse legislation from primary sources |
| `src/ir/` | Intermediate representation for normalised legislative structure |
| `src/ontology/` | Domain concepts and relationships for UK tenancy law |
| `src/summary/` | Generate plain-language summaries with citations |
| `web/` | Astro frontend |
