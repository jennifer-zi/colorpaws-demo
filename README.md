# 🐾 ColorPaws

> **A mobile-first dog walk tracker that turns every walk into a colorful map — and connects you with other dog parents nearby.**

🔗 **[Try the live prototype →](https://jennifer-zi.github.io/colorpaws-demo/)**

*(This is a **clickable prototype**, not a shipping product. Walk data resets on page refresh. The goal is to demonstrate the product thinking, interaction design, and visual direction.)*

---

## Problem statement

Sharing life with a dog is one of the most emotionally rich relationships people have, yet the apps built for it treat dogs like assets to track, not companions to share life with. Two unmet needs stand out:

- **Walks are memories, not just data.** Every walk is a small adventure: a new street, a new park, a new smell your dog couldn't get enough of. But existing trackers reduce these moments to distance, pace, and calorie counts. There's no way to see the world you've explored together, or share it with the people who'd appreciate it most

- **Dog social lives are hard to coordinate.** Most dogs thrive on regular play with familiar friends, but setting up playdates today means trading phone numbers with people you barely know, juggling group texts, and guessing who lives or walks nearby. Dog parents want their dogs to have a social circle without having to build their own.

ColorPaws fills that gap by turning walk tracking into sharable memories, and a lightweight social layer that makes setting up playdates hassle-free.

---

## The solution

A mobile-first app with a greyed out map, where a walk in an unexplored area lights up the map or paints a colored trail, shareable with friends.

**Core experience:** open the app → pick which dog(s) you're walking → tap *Start walk* → the map lights up as you go. Stop the walk and it's saved automatically. Browse all your dog's adventures. See where your friends' dogs hang out. Schedule a playdate when your maps overlap.

---

## Key features

🗺️ **Personal walk map** — Each walk illuminates the corresponding area on the map. Multiple pets can get distinct maps so the map stays readable at a glance.

👯 **Multi-pet support** — Select one or more dogs before starting. Walks are filed under the right pet automatically. Edit assignments later if needed.

🌐 **Friends map with overlap zones** — Toggle which friends' walk routes appear on the same map. Shared "hotspot" zones surface where playdates would feel natural.

📅 **Playdate scheduling** — Send/receive playdate requests with a simplistic accept-or-decline flow. Manage upcoming dates with reschedule and cancel.

🐕 **Pet profiles** — Add dogs with name + breed (the identity used for friending). Per-pet stats: walks logged, total distance, recent activity.

✏️ **Walk management** — Every walk is editable. Reassign to a different dog, change the date, or delete entirely.

---

## Key decisions

**Why a grayed-out map setting?** 
A grayed-out map that is illuminated with walks visualizes the shared memories between the user and their dog. This gamefied approach is not only making tracking fun and engaging, but also serves as a strong differentiation between ColorPaws and competitors, leading to higher engagement and long-term user stickiness. 

**Why adding social features?** 
Memories are better when shared. Allowing users to create a network of friends on the ColorPaws provides emotional and social values. In addition, it addresses a core user need: setting up play dates for their dogs easily and ideally without exchanging personal contacts if they do not personally know the other party.   

**Why a stylized map instead of real geography?** 
For a prototype, an illustrated map communicates the concept of "lighting up explored territory" far more clearly than a gray Google Maps tile would. In a production build, this would layer onto a real map provider (Mapbox or Apple Maps).

**Why not let the user pick *every* color?** Pets get auto-assigned colors from a palette curated for legibility against the map background. Letting users free-pick risked clashes that would make the friends-map view unreadable.

**What I'd build next:**
- Real GPS + map provider integration
- Push notifications for incoming playdate requests
- "Heatmap" view showing favorite hangout spots over time
- Photo attachments per walk
- Share-to-Instagram of a walk's colored trail

---

## Tech & tools
- Researched the competitive landscape, brainstormed product positioning, and designed and prototyped with Claude
- Leveraged the "office hour" skill created by Y Combinator's founder for product positioning, and used the frontend design skill on Claude for UI design. 
- Color palette built around warm earth tones for a cozy, "your dog's world" feeling
- The actual product will be built with Lovable, an AI vibe coding tool

---

*Made with ❤️ and a lot of imaginary dogs.*
