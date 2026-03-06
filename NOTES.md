# Spin to Decide — Project Notes
> Your reference for jumping back into this project anytime.
> **Update the Recent Changes section after every session.**

---

## What It Is
A single-page decision-making spin wheel. Add up to 20 custom choices, spin, then keep or remove the result. Pure HTML/CSS/JS — no framework, no backend.

## Live URL
🌐 **https://spin-wheel-one-mu.vercel.app**

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
- `spin()` — animation logic, winner calculation, easing
- `PALETTE` array — segment colors
- Label truncation: `choices[i].name.length > 8`

## Status
✅ Live | 🔶 Beta

---

## Recent Changes (keep updated)
| Date | What Changed |
|---|---|
| Mar 2026 | Initial build and deploy |
| Mar 2026 | Bold black labels (900 weight), pushed toward perimeter (labelR 0.82) |

---

## Next Steps
- [ ] Add custom domain (spin.c2tbuilds.com) once DNS migration to Vercel is done
- [ ] Add to portfolio projects tab ✅ Done
