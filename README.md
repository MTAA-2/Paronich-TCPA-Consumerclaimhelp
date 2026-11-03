# Consumer Claim Help (Wrong-Number Robocalls) — Rebuilt GitHub Pages version

A static (HTML + CSS only, no PHP) rebuild of **consumerclaimhelp.com** — the Paronich Law, P.C. wrong-number robocall (TCPA) page — on the current framework (your uploaded `index-6.html` / `style-6.css`), adding the newer framework elements: **lawyer picture areas** and **parallax background placeholders in the sections**. Content, firm, palette, and typeface are the live site's own.

## Kept from the framework, unchanged

- Page structure, classes, the MTAA CIPA block script, and your Meta Pixel (`1665132690448359`).
- Your form embed: `forms.mtaa.ai/f/nf_441462e043274be8bab32ea3e44ac34c`, in the overflow form card — the container hangs past the hero over the section below it, the frame scrolls internally with `overflow: auto` if the embed runs tall, and your mobile values from the framework are preserved.
- The commented-out site header block (converted inside the comment to Paronich Law, so it is correct if you uncomment it), with the firm name carried in the hero, as in your current framework. Note: the live site's old visible header is therefore not reproduced — the header phone went with it; the number still appears in the review section and footer, as below.
- The call/text consent paragraph in the footer disclaimer, and the footer legal links to your `privacy-policy.html` / `disclaimer.html` on justicehelpnow.com.

## New elements added in this redo

- **Lawyer picture areas** — a "Meet the Attorneys at Paronich Law" block at the end of the review section, in the framework's team-block format, with two photo slots. The site names no individual attorneys, so the slots are placeholders: image files `images/lawyer-photo-1.jpg` and `images/lawyer-photo-2.jpg` (create an `images/` folder next to `index.html` and drop the photos in with those names, or swap in hosted URLs) and `[Attorney Name]` captions to replace with each lawyer's name and title.
- **Parallax placeholders in the sections** — the hero keeps your `.section-parallax` block with its image line as a placeholder (`YOUR-IMAGE-URL-HERE`), and the dark "Who Is Calling You?" section now carries it too, via one added CSS rule, `.section-parallax-2`, which reuses the same navy overlay (rgb 19, 41, 75 at 0.75 — already this site's navy) with its own placeholder (`YOUR-IMAGE-URL-HERE-2`), so the two section images can be set independently when you provide the URLs. Until then those sections render as the solid navy tint over their backgrounds. As in the Taco Bell build, the mobile fallback's misspelled `.section--parallax` selector was fixed to `.section-parallax` so the iOS fallback applies.

## Firm, content, and the phone number

- Everything is Paronich Law, P.C., 350 Lincoln St #2400, Hingham, MA 02043 — title/meta, hero firm line, sponsorship line in the disclaimer, © 2026 Paronich Law, P.C. Content is the live site's: the TCPA explainer and "Don't assume it was just an annoying mistake," the firm's five points, why companies keep calling the wrong person, the nine-card "Who Is Calling You?" grid, $500–$1,500 per qualifying violation "depending on the facts," the four qualification statements, and "Don't Delete Those Voicemails."
- **Phone:** (833) 965-2070 is kept in the review section and footer. On the earlier robocall build this number was flagged because robocallhelp.com's rendered page didn't visibly show it — but your published consumerclaimhelp.com does display it (header, mid-page, and footer), so the question is settled in favor of keeping it.
- All prior-framework traces verified at zero: no Lerner and Rowe names or image hosts (familyjusticenow.com is gone from both files, including the commented header), and no birth-injury or Taco Bell content anywhere.

## Colors and typeface

`css/style.css` is your uploaded `style-6.css` with **color values only** changed (diff-verified), plus the one added `.section-parallax-2` rule described above and the parallax placeholder/fix. The palette is the live consumerclaimhelp.com design, re-sampled from the rendered page on 2026-11-03 (identical to the October robocall build's):

- Deep navy `#13294b` for the top bar, dark section, and footer; indigo `#1e1a5e` through the hero gradient to charcoal `#262626`
- Muted gold `#c9a86a` for kickers, headline accents, and checkmark circles (white checks), and for the CTA buttons with white text (hover `#d8bc7a`); yellow-gold `#e8c87a` highlights on dark backgrounds
- Light gray-blue `#eef1f5` compensation band, light gray `#f2f2f2` section background

Typeface is unchanged from your framework — Fraunces headings with Inter body — because that is the pairing the live site itself runs.

## Files

```
github-consumer-claim-help-landing-page/
├── index.html
├── css/style.css   (your framework CSS, colors only changed + .section-parallax-2)
└── README.md
```

Publish the same way as the other GitHub pages: upload to a repo keeping the structure, Settings → Pages → deploy from branch (root). Add the `images/` folder with the lawyer photos when you have them.
