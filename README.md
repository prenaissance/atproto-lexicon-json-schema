# JSON Schema for Atproto Lexicon definitions

Get autocomplete, linting and documentation for your atproto lexicon files. Built based on the source code of [@atproto/lex-cli](https://github.com/bluesky-social/atproto/tree/main/packages/lex-cli).

For VSCode, add the following to you `settings.json` (adjust the file paths as needed):

```json
{
  "json.schemas": [
    {
      "fileMatch": ["lexicons/**/*.json"],
      "url": "https://prenaissance.github.io/atproto-lexicon-json-schema/v1.json"
    }
  ]
}
```

Sadly, the `@atproto/cli` package does not support adding this per-file using the `$schema` field. Bump this PR if you're interested in that https://github.com/bluesky-social/atproto/pull/3462
