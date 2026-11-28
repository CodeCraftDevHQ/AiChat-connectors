# Adding a connector

1. Put your file in `connectors/` (English file name, lowercase, words separated by `-`).
2. Start the file with `_name`, `_baseUrl` and `_help`, all in English.
3. Never put API keys or personal data in the file; use `"auth"` and the `{{key}}` placeholder.
4. Add an entry to `index.json`: `name`, `description`, `author` and `url` (relative to `index.json`, e.g. `connectors/my-api.json`).
5. Test it in AiChat (Add from URL / catalog) before opening a pull request.
