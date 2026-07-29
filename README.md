# field-hygiene.isogunlabs.com

The public marketing/docs/privacy/security site for Field Hygiene for Jira — plain static
HTML/CSS/JS, no build step, deployed to GitHub Pages directly from this repo's `main` branch
(classic Pages pipeline, same as `recap-privacy`).

This is a **nested Git repo**, living inside `products/field-hygiene/` but tracked separately —
see that project's own `README.md`/`CLAUDE.md` for how the two relate. `git status` in
`products/field-hygiene` will not show changes made here.

## Layout

| Path | What's there |
| --- | --- |
| `index.html` | Homepage — hero, how it works, what it catches, principles, FAQ, CTA |
| `docs.html` | Full documentation, sidebar-navigated |
| `privacy.html` | Privacy policy |
| `security.html` | Security policy |
| `assets/css/site.css` | Shared styles — teal/amber palette, drawn from the app's own logo |
| `assets/img/` | Logo, favicon, and OG/social share image |
| `assets/fonts/` | DM Sans, shared with the rest of the Isogun Labs family |
| `.github/workflows/indexnow.yml` | Notifies Bing/Yandex of URL changes on every push to `main` |

## Deploy

Pages source is set to **Deploy from a branch** (`main`, root) — plain static files, nothing to
build. Push to `main` and it's live within a minute or two.

## Notes

- No screenshot showcase yet — Field Hygiene's Marketplace screenshots aren't ready, so the
  hero is text/icon-led. Swap in a real showcase once screenshots exist (see the parent
  project's `CLAUDE.md` definition of done).
- No analytics wired in yet (deliberately skipped when this site was built — see
  `prompts/marketing-site.md` in the parent project for the reasoning). Add GA4 as its own
  small decision if wanted later, matching the rest of the Isogun Labs family.
- Marketplace links are placeholders (`mailto:` "get notified" CTAs) until the app is actually
  submitted and published — don't add a real Marketplace link before that's true.
