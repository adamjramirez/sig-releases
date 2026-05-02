# Sig v0.1.0-beta

First public beta. Welcome.

## What works

- **Capture** — talk through a meeting, get a structured private note
- **Synthesis** — facts separated from your personal layer, stored on your machine
- **Share** — review the exact text before anything leaves your machine; nothing is sent without your explicit approval
- **Skills** — reusable workflows like 1:1 prep, weekly updates, and call debriefs
- Works alongside Claude, ChatGPT, and Gemini. GitHub Copilot support is coming soon.

## Install

**macOS** (13 Ventura or later)

1. Download `Sig-0.1.0-beta.1-universal.dmg` from the assets below.
2. Open the DMG and drag Sig to Applications.
3. Open Sig from Applications. The build is signed and notarized by Apple, so it opens without security warnings.

**Linux**

1. Download `Sig-0.1.0-beta.1.AppImage` from the assets below.
2. Make it executable: `chmod +x Sig-0.1.0-beta.1.AppImage`
3. Run it: `./Sig-0.1.0-beta.1.AppImage`

Captures and notes are stored as plain markdown in the folder you choose during first-run setup.

## Uninstall

Drag Sig from Applications to the Trash (macOS), or remove the package via your package manager (Linux). Your captures stay on your computer as plain markdown in the folder you picked during setup. Delete that folder if you want them gone.

## Privacy

- Your memory stays on your computer as plain markdown in the folder you pick.
- Messages go directly to your chosen AI provider — Sig doesn't proxy, log, or intercept them.
- Optional connections (Slack, team knowledge base, voice) only run when you turn them on.
- Sig sends a small set of anonymous events for crash diagnostics and product improvement.

Full policy: https://sig-ai.app/privacy. In-app: Settings → Privacy. Questions: privacy@sig-ai.app.

## Telemetry

Sig sends anonymous event counts so we can catch crashes and prioritize fixes — things like which skill ran, app version, OS, and scrubbed crash details. Events go to PostHog Cloud EU.

**Never sent:** message content, file contents, file paths, your name, your email, prompt text, or conversation text.

The full list of allowed events ships with the app and lives in `docs/analytics.md`.

## Reporting bugs

Open an issue: https://github.com/sig-ai-app/sig-releases/issues/new/choose

For anything sensitive: hello@sig-ai.app.

## What's next

This is a beta. The fastest way to make Sig better is to tell us where it gets in your way — small frictions count.
