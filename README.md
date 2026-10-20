# AgentOrch · Assets

What lifehome (the game in [AgentOrch](https://github.com/runsnip/agentorch)) downloads by itself the first time it
runs, kept out of the app so it stays small. One folder and one zip per pack.

| Folder | Pack | What it is |
| --- | --- | --- |
| `people/` | `people` | People in the streets in everyday clothes (28 models, about 13 MB) |

## Development

`python -m agentorch --dev` uses the folders of this checkout (next to the app's) directly.

    python3 tools/pack.py          # dist/<name>.zip + .sha256 for every folder with a manifest.json

The street people are made with the app's `tools/fetch_rocketbox.py --city <name>…` (needs Blender).
A release is a tag `v<version>` matching every pack's `manifest.json`; the workflow attaches the zips.

## License

Apache-2.0 — see [LICENSE](LICENSE) and [NOTICE](NOTICE).
