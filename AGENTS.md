# lebie — static site for lebie.eu (Google OAuth branding)

```text
CONSTRAINT: Do NOT invent requirements. Every rule below must trace to a source
in the Source Map / this ruleset / the human dump. If a question is not covered,
say so and point to the source. Never soften written thresholds or formats.
```

Pattern #2 — see root `AGENTS.md`.

Public homepage + privacy policy for the invoice Google OAuth app (domain **lebie.eu**). Hosted on **GitHub Pages** from this folder’s git repo.

## Operating rules (pattern #2)

1. Do NOT invent requirements. Every rule you state must trace to this file or a linked source. If something isn't covered, say so and point to the source.
2. Treat this file as authoritative over prior knowledge of the domain.
3. When checking against thresholds or fixed formats, apply them strictly.
4. Be accurate to the rules; never soften them against the guidelines' intent.
5. If sources change, update this ruleset in the same turn.
6. Never invent URLs, DNS, or account facts from memory — re-read this file.
7. If something is ambiguous, stop and ask.

## Facts

| Item | Value |
|------|--------|
| Domain | `lebie.eu` (bought at GoDaddy, Francisco 2026-10-27) |
| Purpose | OAuth consent-screen Application home page + Privacy policy URL |
| Site paths | `/` (hello + Lebie brand), `/privacy/` (short English privacy policy) |
| Host | GitHub Pages (chosen 2026-11-07; no GoDaddy web hosting) |
| GitHub | `s1ashz/lebie` (pushed 2026-11-07); remote `git@github.com-s1ashz:s1ashz/lebie.git` |
| Contact on privacy page | `faturas.investimento@gmail.com` |

## Publish

1. This folder is its own git root (not the parent workspace).
2. Push `main` to `s1ashz/lebie` (or the repo name Francisco creates).
3. GitHub → Settings → Pages → Deploy from branch `main` / root.
4. Custom domain `lebie.eu` (repo has `CNAME`). Enable DNS HTTPS when GitHub offers it.
5. GoDaddy DNS (replace parking/DPS):
   - Apex `lebie.eu`: A records → GitHub Pages IPs `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Optional `www`: CNAME → `s1ashz.github.io`
6. Google Cloud OAuth branding URLs: `https://lebie.eu/` and `https://lebie.eu/privacy/`

## Files

| Path | Role |
|------|------|
| `index.html` | Homepage |
| `privacy/index.html` | Privacy policy (`/privacy/`) |
| `styles.css` | Shared styles |
| `CNAME` | Custom domain for GitHub Pages |
| `.nojekyll` | Serve static files as-is |
| `README.md` | Human publish notes |
