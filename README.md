# Ola Link — mobile prototype

Interactive mobile-app prototype for **Ola Link**, an electric shared-commute network for India's daily 1–5 km trip between home and a metro, bus or rail hub. Built for the Ola Electric 2035 APM assignment.

**The promise on every line: _Next Link in X minutes._**

## Demo scenes

Open the live site on a phone for the full-screen app experience. On a laptop it opens inside a phone frame, with a scene list on the left.

| Scene | Deep link | What it shows |
| --- | --- | --- |
| Morning commute | `/#morning` | Proactive notification → Ola home suggestion → Link Stop with "Next Link in 4 min" → Link + metro + Link journey → boarding → live ride |
| A late Link | `/#delay` | The Link runs 3 min late and a ₹10 credit is added automatically |
| Off-peak: Link Pool | `/#pool` | Low demand, so a pooled ride is offered with a pickup window and a 1.3× trip-time cap |
| Late night: Night Mode | `/#night` | Last Link waits for the last train, women's section, woman-driver option, drop point near home, safe-arrival check |
| Link Pass | `/#pass` | Monthly plan, savings and commute summary |
| Driver-owner view | `/#driver` | A driver running Line L1 on a financed Ola vehicle |

On a phone, tap **Scenes** (top-right) to jump between scenes.

## Notes

- Set in Bengaluru (HSR Layout ⇄ Central Silk Board Metro, Yellow Line). The map is simplified; times, fares (₹25 a ride, ₹799 Pass) and credits are assumptions.
- No real data, bookings, payments or location access. Nothing is sent anywhere.
- Plain static site: one `index.html` with inline CSS and JavaScript, no build step, no dependencies. The only external request is Google Fonts (Manrope), with system-font fallbacks.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy

Import the repository into Vercel with framework preset **Other**, no build command and the default output directory.
