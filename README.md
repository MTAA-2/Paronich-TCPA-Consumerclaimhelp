# Robocall Help Landing Page — GitHub Pages (static) version

A static (HTML + CSS only, no PHP) wrong-number robocall (TCPA) landing page for **Paronich Law, P.C.**, built on the framework of your uploaded BioZorb page (`index-5.html` / `style-5.css`) and filled with content from **robocallhelp.com**. Per your standing instruction, all branding and firm-information areas were converted to the sample site's firm.

## Kept from your framework, unchanged

- Page structure, classes, the MTAA CIPA block script, and your Meta Pixel (`1665132690448359`).
- Your form embed: `forms.mtaa.ai/f/nf_441462e043274be8bab32ea3e44ac34c`, in the overflow form card — the container hangs past the hero over the section below it, the frame scrolls internally with `overflow: auto` if the embed runs tall, and your mobile values from the framework are preserved.
- The call/text consent paragraph in the footer disclaimer.
- Footer legal links still point to your `privacy-policy.html` and `disclaimer.html` on justicehelpnow.com (your hosted legal pages from the framework). Say the word if you want them pointed elsewhere for this page.

## Two framework items converted

- **Logo images removed.** The framework's header and footer Bernheim Kelley logo images (personaljusticeclaim.com) were replaced with a Paronich Law text logo in the header slot and the firm name/address in the footer contact block. Your `.logo-size` CSS rules remain in the stylesheet, unused, so the CSS stays faithful to your upload — if you host a Paronich logo on your image CDN, it can drop back into the same slots.
- **Hero video removed.** The framework's hero slot held the BioZorb Wistia video; it was replaced with text hero copy from the sample site. If you have a robocall video ID, send it and it can go back into that same slot.

## Firm information — converted to the sample site (Paronich Law)

- Title/meta and header: Paronich Law, P.C.
- Footer contact: Paronich Law, P.C., 350 Lincoln St #2400, Hingham, MA 02043.
- Disclaimer: the sample's sponsorship line — "THIS IS ATTORNEY ADVERTISING sponsored by Paronich Law, P.C., located at 350 Lincoln St #2400, Hingham, MA 02043."
- Copyright: © 2026 Paronich Law, P.C.
- All prior-firm traces verified at zero: no Bernheim Kelley, Lerner & Rowe, Goldwater, or Weltchek names, numbers, addresses, image hosts, or content, and no BioZorb content or video.

### A note on the phone number — please read

The page includes **(833) 965-2070** ("Questions? We are here to help") in the header, review section, and footer. That number and wording appear at the top of the sample site's extracted page content. However, a separate live inspection of the *rendered* page on 2026-10-30 did not find any phone number visibly displayed in the header, body, or footer screenshots — contact there is presented through the form. The number may live in a hidden or mobile-only element of the sample. It is the sample's own number (nothing was invented), and it has been kept on that basis — say the word if you want it stripped like the stroke page, and it will come out of all three spots.

## Colors

`css/style.css` is your uploaded `style-5.css` with **color values only** changed (diff-verified — every layout, spacing, and overflow rule untouched), matched to the live robocallhelp.com palette, sampled from the rendered site on 2026-10-30:

- Deep navy `#13294b` (their footer) for the top bar, dark section, and footer; indigo `#1e1a5e` (their logo panel) through the hero gradient to charcoal `#262626` (their darkened skyline hero)
- Gold/bronze `#c9a86a` for kickers, headline accents, checkmarks, and the CTA buttons with white text, like their "Reach Out Now" (hover `#d8bc7a`)
- Yellow-gold `#e8c87a` highlights on dark backgrounds (hero eyebrow, footer phone) — the sample's color for its compensation eyebrow and amounts
- Light gray-blue `#eef1f5` for the compensation band

Colors were sampled visually from the rendered page (which uses gradients and a photograph), so they are close approximations rather than values read from that site's stylesheet. The sample also uses a small red accent for "100% Confidential" in its form; the framework has no equivalent element, so red was not mapped.

## Content (from robocallhelp.com)

- Hero: their headline — "Getting Robocalls Meant for Someone Else?" — with their supporting copy: prerecorded calls or messages to your cell phone while a company tries to reach someone else may violate your rights; federal law restricts artificial or prerecorded calls to cell phones without the required consent; $500 to $1,500 may be available for each qualifying violation, depending on the facts.
- Why Paronich Law? — the TCPA explainer and "Don't assume a wrong-number robocall is simply an annoying mistake," followed by their five points: free case review; no upfront costs; focused on unwanted-call and TCPA class actions; experience litigating TCPA cases in federal courts across the country; no fee unless we obtain a recovery.
- Why Do Companies Keep Calling the Wrong Person? — their explanation: a new number that previously belonged to a company's customer, or the wrong number associated with a customer; even a mistaken first call doesn't mean enduring repeated prerecorded calls intended for somebody else.
- Who Is Calling You? — nine cards from their list: banks and financial institutions, debt collectors, creditors, insurance companies, telemarketers, loan servicers, healthcare-related companies, retailers, and other businesses.
- Compensation — their line: a wrong-number robocall could be worth $500–$1,500 per violation; no obligation, confidential case review, compensation may be available.
- What We Look At — their four qualification statements: an artificial, prerecorded, or AI-generated voice call/message on your cell phone; intended for another person; you did not give the company permission; you still have voicemails, screenshots, call logs, or other records. Plus "Don't Delete Those Voicemails" — their evidence list: voicemails, screenshots, call history, dates/times, numbers used, texts, the company's name, notes on the message, and records that you asked them to stop.

## Files

```
github-robocall-help-landing-page/
├── index.html
├── css/style.css   (your framework CSS, colors only changed)
└── README.md
```

Publish the same way as the other GitHub pages: upload to a repo keeping the structure, Settings → Pages → deploy from branch (root).
