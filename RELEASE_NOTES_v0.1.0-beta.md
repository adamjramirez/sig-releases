# Sig v0.1.0-beta

First public beta. Welcome.

## What works

- Capture: talk through a meeting, get a structured private note
- Synthesis: facts separated from your personal layer, stored on your machine
- Share: review the exact text before anything leaves your machine
- Skills: reusable workflows (1:1 prep, weekly updates, call debriefs)
- Works alongside Claude, ChatGPT, Gemini (Copilot support coming soon)

## Known issues

<!-- Replace with the real list. Examples of the kinds of things that belong here: -->
- [ ] First-launch Gatekeeper warning on macOS — see Install below
- [ ] (list anything you already know is rough — long captures, specific edge cases, etc.)
- [ ] (list anything you've deferred for v0.2)

## Install

**macOS** (13 Ventura or later)

1. Download `Sig-0.1.0-beta.dmg` below.
2. Open the DMG and drag Sig to Applications.
3. Open Sig from Applications. The build is signed and notarized by Apple, so it should open without warnings.

**Linux**

1. Download the Linux build below (`Sig-0.1.0-beta.AppImage` / `.deb` — pick the one for your distro).
2. <!-- AppImage: --> Mark it executable (`chmod +x Sig-*.AppImage`) and run it.
3. <!-- .deb: --> Install with `sudo dpkg -i Sig-*.deb` (or your package manager's equivalent).

## Uninstall

Drag Sig from Applications to the Trash. Your captures stay on your machine as plain markdown in `~/...` (document the actual path). Delete that folder if you want them gone.

## Privacy

- Your memory stays on your computer as plain markdown in the folder you pick.
- Messages go directly to your chosen AI provider — Sig doesn't proxy, log, or intercept them.
- Optional connections (Slack, team KB, voice) only run when you turn them on.
- Anonymous usage counts during beta — see Telemetry below.

Full details in-app: Settings → Privacy. Questions: privacy@sig-ai.app

## Telemetry

Sig sends anonymous event counts so we can catch crashes and prioritize fixes — things like which skill ran, app version, OS, scrubbed crash details. Events go to an EU-hosted instance.

**Never sent:** message content, file contents, file paths, your name, your email, prompt text, or conversation text.

See Settings → Privacy in the app for the full list.

## Reporting bugs

Open an issue: https://github.com/sig-ai-app/sig-releases/issues/new/choose

For anything sensitive: adam@sig-ai.app

## What's next

This is a beta. Expect rough edges. The fastest way to make Sig better is to tell us where it gets in your way.
