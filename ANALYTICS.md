# Analytics — what's actually sent

**Last updated:** 2026-05-02

Sig sends a small set of anonymous events so we can catch crashes and prioritize what to fix. This document explains what categories of data we send and — more importantly — what we never send. Anything not on the allowlist enforced inside the app is dropped before it leaves your computer.

The destination is PostHog Cloud EU (`eu.i.posthog.com`). Nothing leaves the EU region.

---

## What we send

Four buckets:

- **App, session, and activity totals** — Sig version, OS, session length, and a few aggregate numbers (count of conversations, count of notes, total Sig folder size). No names, no contents, no paths.
- **Feature use, not feature content** — which skill ran, did it succeed, how long did it take. We never see what you typed or what came back.
- **Errors and crashes** — error category (e.g. quota, network, auth), provider family, scrubbed stack traces.
- **Connection state** — whether you've connected a provider, Slack, or a knowledge base. Not the credentials, not the data.

If you click a feedback button or submit a comment from the feedback surfaces, that comment text is sent. Each of those buttons states this directly before you click. Nothing else you type ever leaves your machine via analytics.

---

## What we never send

- Anything from your Sig folder beyond a count.
- Conversation text — what you typed, what Sig replied, system prompts, skill outputs.
- File paths or filenames.
- Your name or email.
- Prompt text. (We see character counts, not contents.)
- Slack content. (We see counts and durations of syncs.)
- Specific model names. (We see provider family — `claude` / `chatgpt` / `gemini` — never specific model IDs, which would reveal subscription tier.)
- Raw error messages. They're sanitized: emails, URLs, and home-directory paths are stripped, and they're truncated.
- Stack traces with real paths. Your home directory becomes `<home>`; your Sig folder becomes `<profile>`.

---

## Your install ID

Every install generates a random anonymous ID on first launch. The analytics backend uses it to group one install's events. It is not joined to any external identity system. You can find it under **Settings → Advanced → Diagnostic** and reset it by deleting the ID files (the next launch generates a new one; events before and after the reset will not be linked).

---

## In-app toggle

There is no in-app toggle to turn analytics off today. We may add one in the future.

---

## Changing this list

Adding a new event or property requires updating the in-app allowlist and this document. Anything not on the list is dropped before it leaves your computer.

Questions: privacy@sig-ai.app
