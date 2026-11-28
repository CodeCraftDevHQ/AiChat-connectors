# AiChat connectors

Ready-made connector files for [AiChat](https://github.com/CodeCraftDevHQ/AiChat). A connector is a small JSON file that
describes how to talk to an API (chat, image, video, audio, 3D, ...). One connector can contain several **modes**
(for example text to image, upscale, inpaint), and it can load models and voices from the server by itself.

## Use a connector

1. In AiChat open **Settings → APIs → Add → Custom connector (JSON)**.
2. Press **Add from URL / catalog**, load the list (or paste the link of any connector file) and press **View → Add**.
3. Fill in the API key (if the service needs one), press **Fetch models**, and choose the **Mode** in the API settings.

Before a connector is added, AiChat shows every server it will contact. A connector can send your messages, files and API key
to those addresses, so only use files you trust.

## Available connectors

| Connector | File | Notes |
|---|---|---|
| ElevenLabs | `connectors/elevenlabs.json` | Text to speech, sound effects, music; models and voices from your account |
| Fooocus-API (local) | `connectors/fooocus-api.json` | Modes: text to image, upscale / vary, image prompt / face swap, inpaint, outpaint, describe |
| Viggle | `connectors/viggle.json` | Modes for image, video and 3D |
| Ollama (native chat API) | `connectors/ollama-chat.json` | Local chat |
| Reasoning chat (DeepSeek-style) | `connectors/reasoning-chat.json` | Shows streamed reasoning |
| OpenAI Images | `connectors/openai-images.json` | Needs an API key |
| OpenAI Text-to-Speech | `connectors/openai-tts.json` | Needs an API key |
| AUTOMATIC1111 / Forge | `connectors/automatic1111-forge.json` | Local, start with `--api` |
| ComfyUI (default workflow) | `connectors/comfyui-default-workflow.json` | Local |
| ComfyUI: Wan 2.2 (video) | `connectors/comfyui-wan22-video.json` | Local |
| Send a file to an API | `connectors/send-file-template.json` | Template |
| Generic async job | `connectors/generic-async-job.json` | Template for submit / poll / download APIs |

## File format

Optional top-level keys: `_name` (display name), `_baseUrl` (default Base URL), `_help` (what to prepare).
The full format is described in `docs/CONNECTORS.md` of the AiChat repository, and the **Help and AI prompt** button in the
connector editor gives a prompt that lets any AI assistant write a connector for your API.

See [CONTRIBUTING.md](CONTRIBUTING.md) to add your own.
