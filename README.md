# VAN — Managed Buyer Ticket Form

Static HTML prototype of the MB ticket intake form. Source-of-truth for the Netlify deploy at `heartfelt-granita-3dba2e.netlify.app`.

This is a **prototype**. The production form will be a HubSpot-native form wired to ticket pipeline `768309544` — built from this spec.

## Versions

- **v5** (2026-05-07) — current. Aligned with `wiki/projects/mb-ticket-system/form-structure-v5.md`. Issue description global is now conditional (hidden for Feature/Kameleo/NewFB/BackOffice). vAuto sync option dropped from "Errors after update". vAuto checkbox trimmed to 5 options + "Nothing is being pushed". Feature not working stripped to single textarea. Kameleo "What have you tried" required. New FB account: Reason for request select + dealer-only sub-flow (connect personal vs create new — never collects passwords).
- **v4** (2026-05-06) — Adds `Dealer vs Managed Buyer` selector at the top per Tom/Mary request (junta 2026-05-06). Aligned with `wiki/projects/mb-ticket-system/form-structure-v4.md`.
- **v3** (2026-05-05) — finalized in junta with Mary: dedupe gate, removed "VAN is slow", flat issue type, Active FB count drives priority, Kameleo as textarea, vAuto rename to "Push output error".

## Deploy

Push to `master` → Netlify auto-deploys (once connected in Netlify dashboard).

To connect Netlify:
1. Netlify → Add new site → Import from Git → GitHub
2. Pick `mfahmel/van-mb-ticket-form`
3. Branch: `master` · Build: none · Publish dir: `/`
4. Set custom domain to point at `heartfelt-granita-3dba2e.netlify.app`
