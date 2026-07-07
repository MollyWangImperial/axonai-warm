# RehynAI — Warm landing page ("Dawn of Hope")

A redesign of the RehynAI landing page, re-targeted from clinicians to **patients and
families** recovering from a stroke. Warm, hopeful, and emotionally reassuring — while
keeping a quiet entry point for clinicians.

The page is a single self-contained `index.html` (Tailwind + Google Fonts via CDN, no
build step). Open it directly in a browser, or deploy it as a static site.

## Design direction
- **Mood:** Dawn of Hope — warm ivory/peach base, hopeful teal, coral warmth, soft "breathing" dawn gradient.
- **Voice:** plain, dignified, encouraging. Speaks to feelings (uncertainty, motivation, hope), not clinical metrics.
- **Type:** Fraunces (warm serif headlines) + Plus Jakarta Sans (readable body), large 18px base for accessibility.
- **Motion:** gentle scroll-in fades; respects `prefers-reduced-motion`.

## Preview locally
Just open `index.html` in any browser. (Or run a tiny server: `python3 -m http.server` then visit `http://localhost:8000`.)

## Deploy (GitHub Pages)
1. Push this folder to a new GitHub repo.
2. Repo **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Your site goes live at `https://<username>.github.io/<repo>/`.

## Photos to source (replace the placeholders)
Every dashed `[ photo ]` block is a placeholder. Replace each with a real, warm photo
(faces visible, natural light, genuine emotion). Suggested shots:

| Placeholder | Photo to source |
|---|---|
| **Hero** | Older stroke survivor walking, a family member's hand on their arm, soft morning light, hopeful. |
| **How it works — Step 1** | A short movement being recorded on a phone in a bright, homely living room. |
| **How it works — Step 2** | A simple, friendly progress chart on a tablet, held in warm hands. |
| **How it works — Step 3** | Family and therapist looking over a personalised plan together, smiling. |
| **Story** | Candid, close multigenerational family moment at home — patient and carer together. |

Free, license-clear sources: Unsplash, Pexels, or commissioned photography. Avoid cold
stock "doctor + clipboard" imagery — choose home, family, and touch.

To swap a placeholder, replace the `<div class="photo-ph">…</div>` with:
`<img src="assets/your-photo.jpg" alt="describe the scene" class="rounded-3xl w-full h-full object-cover" />`

## Notes
- The "For clinicians" strip and the family testimonial are intentionally marked as illustrative — replace with real quotes/consent before publishing.
- Buttons currently link to `#` / the in-page sections; wire them to your real app routes (`/login`, demo form, etc.) when integrating.

## Photos included (live)
The page now ships with free, commercial-use photos hotlinked from Pexels
([Pexels License](https://www.pexels.com/license/) — free, no attribution required; credited here as good practice):

- Hero — "Multi-generational family walking" by Gustavo Fring (Pexels #4173081)
- Step 1 — "Young woman holding a senior's hand" by ilayda0700 (Pexels #36706838)
- Step 2 — "Walking toward sunset" by Gustavo Fring (Pexels #4173158)
- Step 3 — "Caregiver and senior in a cozy kitchen" by Jsme MILA (Pexels #29372709)
- Story — "Elderly woman and caregiver on the couch" by Jsme MILA (Pexels #29373893)

To use your own photos instead, replace the `src` on the relevant `<img>` in `index.html`
(or drop files into an `assets/` folder and point to them).
