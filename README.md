# linkstash-api-v2

Learning project: clean Express API structure

Started as a weekend hack, grew on me.

## Highlights

- REST endpoints: list / create / delete / search
- Request validation helpers, no framework magic
- Morgan logging and centralized error handler
- env-driven port, runs anywhere Node does
- In-memory store with optional JSON persistence

## Install

```bash
npm install
npm run dev
```

## Usage

```bash
curl -X POST localhost:3000/api/bookmarks \
  -H 'content-type: application/json' \
  -d '{"url": "https://example.com", "tags": ["reading"]}'
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   ├── config.js
│   ├── index.js
│   └── store.js
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
└── package.json
```

## Development

```bash
npm install
```

## Notes

- mostly stable, edge cases remain

## License

MIT - see [LICENSE](LICENSE).
