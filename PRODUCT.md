# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

One plain HTML file (`index.html`) with inline CSS and JS. No build step, no framework, no server. Chosen by the user so the file opens by double-clicking, deploys anywhere, and stays readable. Fonts load from Google Fonts; everything else ships in the file.

## Users

**Primary: Zoya, around 10–12, the hamster's owner.** She reads fluently and wants the site to look grown-up rather than babyish. She is the one who shows it to people.

**Secondary: family and visitors** who look at the site out of interest, or who need to know how to feed and handle Kiks when Zoya is not there.

## Product Purpose

A one-page website about Kiks, Zoya's grey dwarf hamster. It exists so Zoya has something of her own that is genuinely hers to show, and so that anyone near the cage knows the real rules — what Kiks can eat, what he must never eat, and how to pick him up. Success is Zoya wanting to show it to someone unprompted, and a visitor getting the care facts right without asking.

## Positioning

Not a generic pet template. Everything on the page is about this one animal: a grey dwarf hamster, nocturnal, named Kiks. The site's organizing idea is his night shift — the day/night state of the page is the hamster's own state, not a theme preference.

## Operating Context

Viewed on family devices, phones and tablets as much as laptops, often handed over screen-first. Shown to visitors while standing next to the cage. Opened as a local file and/or from a shared link. Read in both bright rooms and dim evening light.

## Capabilities and Constraints

- Single self-contained page. No backend, no accounts, no data collection.
- Must work on a phone held one-handed, and hold up when the file is opened directly from disk.
- Google Fonts is the only external dependency; it must degrade to a real fallback stack.
- Currently published as a Claude Artifact: `https://claude.ai/code/artifact/3653e812-e186-460c-becf-c0758142beeb`. Republishing to that URL requires passing it explicitly as `url`. Artifact hosting enforces a CSP — scripts only from cdnjs/jsdelivr/tailwind/jquery, stylesheets only from Google Fonts, no other external fetches. `index.html` is a complete standalone document so it opens from disk; the Artifact host supplies its own skeleton, so publishing uses a copy with the `<!doctype>`/`<html>`/`<head>`/`<body>` wrapper stripped.
- **Undecided:** where the site lives long-term (artifact link only, a static host, or a real domain).

## Brand Commitments

- The names are **Zoya** and **Kiks**, spelled exactly that way.
- Kiks is a **grey dwarf hamster** — grey-brown fur, cream belly, dark stripe down the back. Any illustration or asset must match.
- Voice: warm, playful, plain-spoken, funny about the hamster and never about the reader. Written for a competent 10–12-year-old — no baby talk, no exclamation-mark padding.
- Care instructions are stated as real instructions, not jokes.

## Evidence on Hand

- **No photographs of the real Kiks exist yet.** The current page uses a drawn SVG hamster. If photos arrive, they should replace it.
- **The stat figures on the page (45 g, 8 km a night, 20 seeds per cheek, 6 am bedtime) and the night-shift timetable are typical dwarf-hamster values and affectionate guesses, not measurements of Kiks.** Kiks's real weight, age, birthday, and habits are unknown. Do not invent more specifics, and do not present the existing ones as measured until someone confirms them.
- The food lists (safe foods, and the never-feed list: chocolate, citrus, onion, garlic, almonds, salty snacks) are real dwarf-hamster care facts and must stay accurate.

## Product Principles

1. **This hamster, not hamsters.** Every detail is about Kiks specifically. Generic pet-site content is a failure state.
2. **Never talk down to her.** The reader is eleven, not four. Respect shows in the writing, not in decoration.
3. **The care facts are load-bearing.** Playfulness never blurs what is safe to feed or how to hold him.
4. **One file, no dependencies to babysit.** Anything added must survive being opened straight from disk years from now.
5. **Say what is known.** Where a fact about Kiks is a guess, it stays clearly a friendly guess rather than hardening into a claim.

## Accessibility & Inclusion

No formal standard was set. Product-specific needs: readable at arm's length on a phone, large touch targets for interactive bits, motion that respects `prefers-reduced-motion`, and legible contrast in both the light and dark states since the page is read in dim rooms.
