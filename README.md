# Credential Sentinel — website

Four static pages for App Store Connect. No build step, no dependencies, no
external requests — just HTML and one stylesheet.

| File | Used in App Store Connect as | Live URL |
|---|---|---|
| `index.html` | Marketing URL | https://luissummit.github.io/credential-sentinel/ |
| `privacy.html` | **Privacy Policy URL** (required) | https://luissummit.github.io/credential-sentinel/privacy.html |
| `support.html` | **Support URL** (required) | https://luissummit.github.io/credential-sentinel/support.html |
| `terms.html` | Custom EULA (optional) | https://luissummit.github.io/credential-sentinel/terms.html |

Served by GitHub Pages from the `main` branch, root folder. This repository must
stay **public**, and Apple's reviewer must be able to open the privacy URL
without logging in.

## Editing

Edit the files and commit; Pages redeploys in about a minute. The master copies
live on the iMac in `Expire Reminder Business/website/`.

- `support@summituspro.com` is the contact address on every page.
- **Summit** is the publisher name throughout.
- `terms.html` names Florida law and Lake County as venue.
- `privacy.html` and `terms.html` carry the effective date **7 October 2026**.
  Bump it whenever the text changes materially.

## Keeping it accurate

The privacy policy states that the app collects nothing, makes no network
requests of its own, and contains no analytics or third-party SDKs. That is
true of the current code — verified against the source on 7 October 2026.

**If an SDK, a crash reporter, a backend, an account system, or document
attachments that upload anywhere are ever added, this page has to change before
that version ships.** An inaccurate privacy policy is grounds for rejection at
review, and for removal afterwards.
