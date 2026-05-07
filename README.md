# VAN — Managed Buyer Ticket Form

Static HTML prototype of the MB ticket intake form. Source-of-truth for the Netlify deploy at `heartfelt-granita-3dba2e.netlify.app`.

This is a **prototype**. The production form will be a HubSpot-native form wired to ticket pipeline `768309544` — built from this spec.

## Versions

- **v4** (2026-05-06) — current. Adds `Dealer vs Managed Buyer` selector at the top per Tom/Mary request (junta 2026-05-06). Aligned with `wiki/projects/mb-ticket-system/form-structure-v3.md`.
- **v3** (2026-05-05) — finalized in junta with Mary: dedupe gate, removed "VAN is slow", flat issue type, Active FB count drives priority, Kameleo as textarea, vAuto rename to "Push output error".

## Deploy

Push to `master` → Netlify auto-deploys (once connected in Netlify dashboard).

To connect Netlify:
1. Netlify → Add new site → Import from Git → GitHub
2. Pick `mfahmel/van-mb-ticket-form`
3. Branch: `master` · Build: none · Publish dir: `/`
4. Set custom domain to point at `heartfelt-granita-3dba2e.netlify.app`
