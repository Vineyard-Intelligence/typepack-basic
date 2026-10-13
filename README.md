# typepack-basic

The **basic Type Pack collection** for Vineyard — schema-only definitions of entity types and
their properties. No code runs; a Type Pack is data.

| Type Pack | Identifier | Types |
| --- | --- | --- |
| Infrastructure | `run.vineyard.typepacks.infrastructure` | 15 |
| Threat | `run.vineyard.typepacks.threat` | 10 |
| Identity | `run.vineyard.typepacks.identity` | 7 |
| Financial | `run.vineyard.typepacks.financial` | 4 |
| Endpoint | `run.vineyard.typepacks.endpoint` | 6 |
| Geospatial | `run.vineyard.typepacks.geo` | 3 |

Each pack lives at `typepacks/<name>.json`. Clients fetch a pack from this repo at the commit
the registry pins, e.g.
`https://cdn.jsdelivr.net/gh/Vineyard-Intelligence/typepack-basic@<commit-sha>/typepacks/infrastructure.json`.

## Listing / installing

These packs are listed in the [registry](https://github.com/Vineyard-Intelligence/registry) and
browsable at [docs.vineyard.run](https://docs.vineyard.run/). Install one from the in-app
marketplace.

## Contributing

Open a pull request changing a `typepacks/*.json` file. CI validates every pack against the
canonical Type Pack schema. To add a *new* pack to the catalog, also open a PR against the
registry.

## License

MIT
