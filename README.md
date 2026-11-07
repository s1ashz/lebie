# lebie.eu

Static site for the **Lebie** brand / Google OAuth consent URLs.

- `https://lebie.eu/` — hello + brand
- `https://lebie.eu/privacy/` — privacy policy

Hosted on **GitHub Pages** (no GoDaddy hosting). Details: `AGENTS.md`.

## First publish

On the Mac, in this folder (personal GitHub account `s1ashz`, SSH host `github.com-s1ashz`):

```bash
# Create empty public repo s1ashz/lebie on github.com, then:
git remote add origin git@github.com-s1ashz:s1ashz/lebie.git
git push -u origin main
```

Then: repo **Settings → Pages** → branch `main` / `/` (root). Custom domain: `lebie.eu`. Wait for HTTPS certificate.

### GoDaddy DNS

Remove parking/DPS. Set:

| Type | Name | Value |
|------|------|--------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `s1ashz.github.io` |

### Google Cloud

OAuth consent branding:

- Application home page: `https://lebie.eu/`
- Privacy policy: `https://lebie.eu/privacy/`
