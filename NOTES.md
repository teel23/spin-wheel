# Spin to Decide — Project Notes
> Reference for jumping back into this project.
> Last updated: March 9, 2026

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
