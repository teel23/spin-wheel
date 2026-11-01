# Spin to Decide — Notebook

> **Status:** Live · lives on GitHub (iCloud copy removed)  
> **Notebook updated:** 2026-11-01

| | |
|---|---|
| **What** | Decision spin wheel: up to 20 choices, spin, keep or eliminate the result |
| **Repo** | [teel23/spin-wheel](https://github.com/teel23/spin-wheel) (public) |
| **Live** | https://spin.c2tbuilds.com (Vercel) |
| **Stack** | Single `index.html` (HTML/CSS/JS, Canvas + SVG labels) |
| **Active** | 2026-03-09 → 2026-07-08 |

## Where it stands

Live. Last change (Jul 8): current choices persist across refresh (`spinSession` in localStorage).
NOTES flagged confirming that the `spin.c2tbuilds.com` CNAME resolves.

## Getting back in

```bash
gh repo clone teel23/spin-wheel ~/dev/spin-wheel && open ~/dev/spin-wheel/index.html
```

## Timeline (git history, newest first)

```text
2026-07-08  dd610ee  Persist current choices across refresh (spinSession in localStorage)
2026-06-24  251ac9c  Docs: mark Spin to Decide feature-complete (Done)
2026-03-09  38f1789  restore: full-featured version with sounds, saved wheels, and flick-to-spin
2026-03-09  c3c7ad6  fix: flat wheel, centered labels, remove duplicate animation loop
2026-03-09  2815e19  initial commit
```

## Code layout

```text
NOTES.md
index.html
```

## Original notes

Every doc that existed for this project, verbatim (duplicates removed, secrets redacted). Click to expand.

<details>
<summary><b>NOTES.md</b> · repo · 2.1 KB</summary>

# Spin to Decide — Project Notes
> Reference for jumping back into this project.
> Last updated: July 8, 2026 (session persistence added)

---

## What It Is
A sleek decision-making spin wheel. Add up to 20 custom choices, spin to let fate decide, then keep or eliminate the result. Vivid color-coded segments, smooth eased animation, clean dark UI. No login, no fluff, just spin.

## Live URL
🌐 **https://spin.c2tbuilds.com** *(CNAME set — confirm it's resolving)*

## GitHub
📁 **https://github.com/teel23/spin-wheel**

## Local Path
`/COMPUTER/AI/Projects/spin-wheel/`

## Platform
🚀 **Vercel** — auto-deploys on push to `main`

---

## Tech Stack
HTML · CSS · JavaScript · Canvas API · Vercel

## File Structure
Single-file app: `index.html` contains all HTML, CSS, and JS.

## How It Works
- Canvas draws the wheel at 760×760 internal resolution, fills the container
- SVG overlay (`viewBox="0 0 420 420"`) draws labels inside each slice
- Constants: `SVG_R = 202` (wheel radius), `LABEL_R = SVG_R * 0.65` (labels at 65% radius)
- Single animation loop: `doSpin()` only — old duplicate `spin()` was removed

---

## Status
✅ Live | Done — feature-complete (spin.c2tbuilds.com confirmed resolving Jun 2026)

---

## Portfolio Card
- Buttons: Launch App (blue) + Install App (green)
- Screenshot: `spinwheel.png` (default Pizza/Tacos/Sushi/Burgers choices)

---

## Recent Changes
| Date | What Changed |
|---|---|
| Mar 2026 | Rotated embedded GitHub token in git remote (security fix) |
| Mar 9, 2026 | **Bug fix commit `c3c7ad6`**: removed duplicate `spin()` animation loop |
| Mar 9, 2026 | Canvas CSS: `top:0; left:0; width:100%; height:100%` (was offset 14%/72%) |
| Mar 9, 2026 | Pointer CSS: `top:-14px` (was `calc(14% - 16px)`) |
| Mar 9, 2026 | SVG coords: `SVG_R=202`, `LABEL_R=SVG_R*0.65` — labels now inside slices |
| Mar 9, 2026 | Install App button added to portfolio card |

---

## Open Items
- [x] Save choices to localStorage so they persist on refresh (July 8, 2026 — `spinSession` key)
- [x] Confirm spin.c2tbuilds.com resolves in browser — confirmed live July 8, 2026

</details>


<details>
<summary><b>spin-wheel/NOTES.md</b> · iCloud · 2.1 KB</summary>

# Spin to Decide — Project Notes
> Reference for jumping back into this project.
> Last updated: July 8, 2026 (session persistence added)

---

## What It Is
A sleek decision-making spin wheel. Add up to 20 custom choices, spin to let fate decide, then keep or eliminate the result. Vivid color-coded segments, smooth eased animation, clean dark UI. No login, no fluff, just spin.

## Live URL
🌐 **https://spin.c2tbuilds.com** *(CNAME set — confirm it's resolving)*

## GitHub
📁 **https://github.com/teel23/spin-wheel**

## Local Path
`/COMPUTER/AI/Projects/spin-wheel/`

## Platform
🚀 **Vercel** — auto-deploys on push to `main`

---

## Tech Stack
HTML · CSS · JavaScript · Canvas API · Vercel

## File Structure
Single-file app: `index.html` contains all HTML, CSS, and JS.

## How It Works
- Canvas draws the wheel at 760×760 internal resolution, fills the container
- SVG overlay (`viewBox="0 0 420 420"`) draws labels inside each slice
- Constants: `SVG_R = 202` (wheel radius), `LABEL_R = SVG_R * 0.65` (labels at 65% radius)
- Single animation loop: `doSpin()` only — old duplicate `spin()` was removed

---

## Status
✅ Live | Done — feature-complete (spin.c2tbuilds.com confirmed resolving Jun 2026)

---

## Portfolio Card
- Buttons: Launch App (blue) + Install App (green)
- Screenshot: `spinwheel.png` (default Pizza/Tacos/Sushi/Burgers choices)

---

## Recent Changes
| Date | What Changed |
|---|---|
| Mar 2026 | Rotated embedded GitHub token in git remote (security fix) |
| Mar 9, 2026 | **Bug fix commit `c3c7ad6`**: removed duplicate `spin()` animation loop |
| Mar 9, 2026 | Canvas CSS: `top:0; left:0; width:100%; height:100%` (was offset 14%/72%) |
| Mar 9, 2026 | Pointer CSS: `top:-14px` (was `calc(14% - 16px)`) |
| Mar 9, 2026 | SVG coords: `SVG_R=202`, `LABEL_R=SVG_R*0.65` — labels now inside slices |
| Mar 9, 2026 | Install App button added to portfolio card |

---

## Open Items
- [ ] Future: save choices to localStorage so they persist on refresh
- [ ] Confirm spin.c2tbuilds.com resolves in browser (CNAME `spin` → `cname.vercel-dns.com` set in Namecheap)

</details>


<details>
<summary><b>Archive/misc/SpinWheel/NOTES.md</b> · iCloud · 2.3 KB</summary>

# Spin to Decide — Project Notes
> Your reference for jumping back into this project anytime.
> **Update the Recent Changes section after every session.**

---

## What It Is
A single-page decision-making spin wheel. Save up to 10 named wheels locally. Add up to 20 choices per wheel, spin, then keep or remove the result. Pure HTML/CSS/JS — no framework, no backend.

## Live URL
🌐 **https://spin.c2tbuilds.com** (custom domain — live ✅)
🔗 Also available at: https://spin-the-wheel-puce.vercel.app

## GitHub
📁 **https://github.com/teel23/spin-wheel** ✅ Connected and auto-deploying

## Platform
🚀 **Vercel** — auto-deploys on every push to `main`

---

## How to Deploy Changes
1. Edit `index.html` directly (single file app)
2. `git add index.html`
3. `git commit -m "describe what changed"`
4. `git push`
5. Vercel auto-deploys (~1 min)

---

## Key Code Locations (all in index.html)
- `drawWheel()` — canvas rendering, segment colors, label font/size/position
- `doSpin(minRots)` — animation logic, winner calculation, easing. Accepts min rotation count.
- `getSegmentAtPointer()` — detects which segment is at the top pointer each frame (used for tick sounds)
- `playTick()` — Web Audio API triangle oscillator, fires on every segment crossing during spin
- `touchstart/move/end` on canvas — flick gesture detection, maps speed to rotation count
- `PALETTE` array — segment colors
- `MIN_ROTATIONS = 2` — guaranteed minimum full rotations per spin
- `MAX_WHEELS = 10` — max saved wheels in localStorage
- `spinWheels` localStorage key — array of `{id, name, entries, history, colorScheme}`

## Status
✅ Live | 🔶 Beta

---

## Recent Changes (keep updated)
| Date | What Changed |
|---|---|
| Mar 2026 | Initial build and deploy |
| Mar 2026 | Bold black labels (900 weight), pushed toward perimeter (labelR 0.82) |
| Mar 2026 | Custom domain spin.c2tbuilds.com confirmed live; portfolio card URL updated |
| Mar 2026 | Major feature update: empty start state, saved wheels (10 max, localStorage), tick sounds (Web Audio API), flick-to-spin gesture, min 2 full rotations, spin history per wheel |

---

## Next Steps
- [x] Add custom domain (spin.c2tbuilds.com) — live ✅
- [x] Add to portfolio projects tab
- [x] Update portfolio card URL → spin.c2tbuilds.com

</details>


<details>
<summary><b>Archive/misc/SpinWheel/AUDIT_MARCH_2026.md</b> · iCloud · 2.3 KB</summary>

# SpinWheel (Spin to Decide) — Audit Report
*Generated: March 2026*

## Current State
- Live URL: https://spin-the-wheel-puce.vercel.app (no custom domain yet)
- GitHub Repo: https://github.com/teel23/spin-wheel
- Hosting Platform: Vercel ✅
- Auto-Deploy: Yes (push to main → Vercel builds)
- Status: Live / Beta

## Tech Stack
- Framework: None — Vanilla HTML/CSS/JavaScript (Canvas API)
- Build Tool: None (static single-file site)
- Key Libraries: None (pure Canvas)
- Node Version: N/A
- Deprecated Tech: None

## Deployment Health
- Vercel config: ✅ Not needed — Vercel auto-detects static HTML
- Netlify files removed: ✅ No Netlify files found
- Portfolio links correct: ⚠️ Points to `spin-the-wheel-puce.vercel.app` — custom domain `spin.c2tbuilds.com` planned but not yet set up

## SECURITY FLAG
⚠️ The git remote URL contains an embedded GitHub personal access token (token redacted).
Run `git remote -v` locally to see it.

This token is stored in plain text in `.git/config`. Actions required:
1. **Rotate this token immediately at github.com/settings/tokens** — treat it as compromised
2. After rotating, update the remote with a clean URL: `git remote set-url origin https://github.com/teel23/spin-wheel.git`
3. Use a credential manager or SSH keys instead of embedding tokens in URLs

## Dead Code & Waste
- Unused files: None (single index.html file)
- Unused components: N/A
- Unused assets: None
- Console.logs in prod: Unknown — single-file app; recommend a quick grep
- Other waste: None

## Completion Assessment
**Percent complete: 90%**

### What's done:
- Custom spin wheel with up to 20 entries
- Vivid color-coded segments
- Smooth eased animation
- Keep or eliminate result after spin
- Clean dark UI
- Live on Vercel

### What's missing to call this finished:
- Custom domain: `spin.c2tbuilds.com` (blocked on DNS migration from Netlify to Vercel for c2tbuilds.com)
- Embedded GitHub token must be rotated and removed from git config

## Next Phase Plan
### Phase: Domain + Security
**Goal:** Custom domain and clean git config
**Features:**
- Migrate DNS for c2tbuilds.com to Vercel (Namecheap → cname.vercel-dns.com)
- Add spin.c2tbuilds.com in Vercel dashboard
- Remove embedded token from git remote, rotate token

## Quick Fixes Done This Session
- None (no Netlify files; security issue flagged for manual remediation)

</details>
