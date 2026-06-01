# StreamSheets

**Live site: https://streamsheets.dev**

Cheatsheets for data streaming.

Compact, hoverable references for distributed data systems:

- **Apache Flink** - stream processing concepts, time and windows, state, fault tolerance, architecture, SQL & Table API
- **Apache Kafka** - core concepts, producers, consumers, storage and durability, ecosystem, security and ops
- **Apache Iceberg** - core concepts, schema and layout, write operations, time travel and branching, maintenance, catalogs, performance

Each cheatsheet has a release-history page and a project-info panel (links, recent versions, headline stats).

## Learn more

Hovering a concept reveals a popup with a **Learn more** button. These link out to [Confluent Developer](https://developer.confluent.io) courses - free (as in free beer) video lessons that explain the concept in depth. No signup, no paywall.

> **Disclosure:** I work at Confluent. The linked courses are Confluent's free educational content, chosen because they happen to be high-quality explanations of these concepts - but this is an independent side project and is not an official Confluent product.

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
