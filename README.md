# Cheatsheets for Data Streaming

Compact, hoverable references for distributed data systems:

- **Apache Flink** - stream processing concepts, time and windows, state, fault tolerance, architecture, SQL & Table API
- **Apache Kafka** - core concepts, producers, consumers, storage and durability, ecosystem, security and ops
- **Apache Iceberg** - core concepts, schema and layout, write operations, time travel and branching, maintenance, catalogs, performance

Each cheatsheet has a release-history page and a project-info panel (links, recent versions, headline stats).

## Running locally

These are static HTML files with no build step. Open `index.html` directly, or serve the directory with any static server:

```sh
# Python
python3 -m http.server 8000

# Node (npx)
npx serve .
```

Then visit http://localhost:8000.

## Stack

Vanilla HTML, CSS and JavaScript. No bundler, no framework, no runtime dependencies. Fonts come from Google Fonts (`Inter`, `JetBrains Mono`). Project logos are stored locally under `shared/logos/`.

## Layout

```
.
├── index.html              # landing page
├── flink/
│   ├── index.html          # Flink cheatsheet
│   └── releases.html       # Flink release history
├── kafka/
│   ├── index.html
│   └── releases.html
├── iceberg/
│   ├── index.html
│   └── releases.html
└── shared/
    └── logos/              # SVG logos
```

## Trademarks

Apache®, Apache Flink®, Flink®, Apache Kafka®, Kafka®, Apache Iceberg™, Iceberg™ and the Apache feather logo are either registered trademarks or trademarks of The Apache Software Foundation in the United States and other countries. Project logos are used in accordance with the ASF's trademark and branding policies. This project is independent and is not affiliated with, endorsed, or sponsored by the ASF.

## License

MIT - see [LICENSE](./LICENSE).
