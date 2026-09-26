# voice-todo-prioritizer

Transcribes a spoken brain-dump of tasks and sorts them into a prioritized to-do list, on-device. Built with [Tether's QVAC SDK](https://github.com/tetherto/qvac) — the model runs on-device, so nothing leaves your machine.

## What it does

Transcribes a spoken brain-dump of tasks and sorts them into a prioritized to-do list, on-device.

**QVAC functions used:** `loadModel`, `transcribe` and `completion`.

![voice-todo-prioritizer demo](demo.png)

## Why I built it

My to-do list lives in my head until I say it out loud at 11pm.

## Requirements

- Node.js >= 22
- `@qvac/sdk` `^0.19.0` (installed automatically via `npm install`)

## Install

```bash
git clone https://github.com/YURIIMII-byte/voice-todo-prioritizer.git
cd voice-todo-prioritizer
npm install
```

## Run

```bash
node index.js path/to/brain-dump.wav
```

See the comments at the top of `index.js` for the exact input this app expects. On first run, QVAC downloads the model it needs once and caches it locally; every run after that is fully offline.

## SDK version used

`@qvac/sdk` `0.19.1`

## License

MIT — see [LICENSE](LICENSE).
