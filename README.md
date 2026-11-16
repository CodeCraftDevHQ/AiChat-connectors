# AiChat connectors

Ready-made connector files for [AiChat](https://github.com/CodeCraftDevHQ/AiChat).
A connector is a small JSON file that describes how to talk to an API (chat, image, video, audio, 3D...).

## Use one

In AiChat: **Settings → APIs → Add → Custom connector (JSON) → "Add from URL / catalog"**.

- Press **Load the list** to browse `index.json` of this repository, or
- paste the link of any file here (a normal GitHub page link works), then **Get → Use**.

Before you use a connector the app shows every server it will send requests to. Connectors can send
your messages, files and API key to the addresses inside them, so only use files you trust.

## Add yours

1. Put your file in `connectors/`.
2. Optional keys at the top of the file: `"_name"` (shown in the app), `"_baseUrl"` (filled in for the user), `"_help"` (one or two lines: what it does and what to set up).
3. Add an entry to `index.json`:

```json
{ "name": "My API", "description": "What it does", "author": "you", "url": "connectors/my-api.json" }
```

`url` can be relative to `index.json`. The format of connector files is explained in
[docs/CONNECTORS.md](https://github.com/CodeCraftDevHQ/AiChat/blob/main/docs/CONNECTORS.md).

## Use another catalog

The catalog address can be changed in the same dialog, so any repository with an `index.json` like this one works.
