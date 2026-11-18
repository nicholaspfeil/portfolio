# Portfolio site: working rules

Static personal portfolio for Nicholas Pfeil, deployed to Vercel from GitHub.

## Stack
- Plain HTML (`index.html`) and CSS (`style.css`) only. No frameworks, no build step, no JavaScript.
- Fonts (Google Fonts): Newsreader (serif) for name, section and entry headings; Schibsted Grotesk (sans) for body. One accent color (Pacific teal) used for link underlines, automatic dark mode via `prefers-color-scheme`.
- Look: professional document style, high-contrast ink on near-white, no boxed cards, no all-caps labels, no gradients or shadows. Sentence-case serif section headings with a hairline rule below.
- All colors are CSS variables in `:root`; dark values are in the `prefers-color-scheme: dark` block.

## Content rules
- Never include Nicholas's phone number anywhere (site or `resume.pdf`).
- Use only content Nicholas provides. Ask before inventing or rewording claims, metrics, dates, or links.
- Never ship placeholder links (e.g. `[LIVE SITE URL]`). Leave a link out until the real URL exists.
- Keep links relative (`resume.pdf`, not `/resume.pdf`) so the site works when opened from disk.
- Section order: About, Projects, Experience, Education, Skills, Leadership & Activities.

## Working style
- Nicholas wants the site built for him, not a tutorial. Make changes directly and keep explanations short.
- Do not run git commands or deploy without his approval.
- After changes, check the page at phone width (~375px) and laptop width, in light and dark mode.
