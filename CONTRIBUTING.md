# Contributing a connector

- One API (or one endpoint family) per file, in `connectors/`.
- Never put keys, tokens or personal addresses in a file. Use `{{key}}` and the user's own base URL.
- Fill `_help` so people know what to install or enable first.
- Test it in AiChat ("Check" and a real request) before opening a pull request.
- Keep the file under 1 MB (the app refuses larger files).
