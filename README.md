# 🐾 colorpaws

> **A mobile-first dog walk tracker that turns every walk into a colorful map — and connects you with other dog parents nearby.**

🔗 **[Try the live prototype →](https://YOUR-USERNAME.github.io/colorpaws-demo/)**

*(Replace `YOUR-USERNAME` with your GitHub handle once deployed.)*

---

## The problem

Dog owners want to know: *Where have I actually walked my dog this week?* Existing fitness trackers (Strava, Apple Fitness) treat walks as anonymous workout data — they don't recognize that **the walk is for the dog**, not the human. There's no way to:

- Visualize a pet's territory the way the pet experiences it
- Track separate maps for different pets in the same household
- Discover other dog owners whose dogs frequent the same parks
- Coordinate playdates with neighborhood dog friends

colorpaws fills that gap with a playful, social-first take on walk tracking.

---

## The solution

A mobile-first app where each walk paints a colored trail across a personal map, grouped by pet, and shareable with friends.

**Core experience in 30 seconds:** open the app → pick which dog(s) you're walking → tap *Start walk* → the map lights up as you go. Stop the walk and it's saved automatically. Browse all your dog's adventures. See where your friends' dogs hang out. Schedule a playdate when your maps overlap.

---

## Key features

🗺️ **Personal walk map** — Each walk paints a glowing trail in the dog's color. Multiple pets get distinct colors so the map stays readable at a glance.

👯 **Multi-pet support** — Select one or more dogs before starting. Walks are filed under the right pet automatically. Edit assignments later if needed.

🌐 **Friends map with overlap zones** — Toggle which friends' walk routes appear on the same map. Shared "hotspot" zones surface where playdates would feel natural.

📅 **Playdate scheduling** — Send/receive playdate requests with accept-or-decline flow. Manage upcoming dates with reschedule and cancel.

🐕 **Pet profiles** — Add dogs with name + breed (the identity used for friending). Per-pet stats: walks logged, total distance, recent activity.

✏️ **Walk management** — Every walk is editable. Reassign to a different dog, change the date, or delete entirely.

---

## Process & decisions

**Why mobile-first?** Walks happen in motion, one-handed, often in poor light. Every interaction had to be tappable with a thumb without breaking stride.

**Why a stylized map instead of real geography?** For a prototype, an illustrated map communicates the *concept* of "lighting up explored territory" far more clearly than a gray Google Maps tile would. In a production build, this would layer onto a real map provider (Mapbox or Apple Maps).

**Why not let the user pick *every* color?** Pets get auto-assigned colors from a palette curated for legibility against the map background. Letting users free-pick risked clashes that would make the friends-map view unreadable.

**Why divs instead of buttons in the bottom nav?** The rendering environment kept injecting default `<button>` styling that bled through every CSS reset. Switching to `<div role="button">` solved it cleanly while preserving accessibility semantics.

**What I'd build next:**
- Real GPS + map provider integration
- Push notifications for incoming playdate requests
- "Heatmap" view showing favorite hangout spots over time
- Photo attachments per walk
- Share-to-Instagram of a walk's colored trail

---

## Tech & tools

- Designed and prototyped end-to-end as a single self-contained HTML file
- Vanilla JavaScript, hand-drawn SVG map, custom CSS — no frameworks
- Type system: Fraunces (display) + DM Sans (UI)
- Color palette built around warm earth tones for a cozy, "your dog's world" feeling

---

## About this repo

This is a **clickable prototype**, not a shipping product. Walk data resets on page refresh — there's no backend yet. The goal of this repo is to demonstrate the product thinking, interaction design, and visual direction.

Built as a personal portfolio project. Feedback welcome via the issues tab or [LinkedIn](#).

---

*Made with ❤️ and a lot of imaginary dogs.*
