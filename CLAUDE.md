# CLAUDE.md — Enes Media Portfolio

## Project Overview
This is Adrian "Enes" (Enes Media)'s freelance video editing portfolio website. It is a single-page conversion funnel. The page speaks as Adrian under the Enes Media brand — "Enes" is Adrian's nickname (testimonials refer to him as Enes).

Files:
- `index.html` — the whole site (inline CSS + JS)
- `assets/` — headshot and creator avatars (webp)
- `CNAME` — custom domain for GitHub Pages (`enesvfx.com`); don't delete
- `.nojekyll` — tells GitHub Pages to serve files as-is
- `.github/workflows/pages.yml` — Pages deploy workflow (push to `main` + manual "Run workflow")

## Hosting
- **Repo**: https://github.com/DryChester/editportfolio (public), branch `main`
- **Host**: GitHub Pages, Source = **GitHub Actions**, workflow `.github/workflows/pages.yml` ("Deploy to GitHub Pages")
- **Deploying**: pushes made from Claude Code sessions do NOT trigger GitHub Actions or the legacy Pages build. After pushing a change, tell Adrian to open https://github.com/DryChester/editportfolio/actions/workflows/pages.yml and click **Run workflow → Run workflow** (on `main`). Commits Adrian makes himself on github.com deploy automatically.
- **Domain**: `enesvfx.com`, registered at Porkbun. DNS: four A records on the apex → 185.199.108.153 / .109.153 / .110.153 / .111.153, and `www` CNAME → `drychester.github.io`

## Editor Config
- **Name / Brand**: Adrian "Enes" — Enes Media
- **Location / Languages**: Poland (CET) — edits in English and Polish
- **Experience**: 3 years
- **Specialty**: Storytelling and high-quality visuals; script to final cut
- **Niche**: IRL / sports, gaming, documentary — page kept deliberately niche-neutral and professional so it doesn't put off clients from other niches
- **Style / Vibe**: Clean & cinematic
- **Reference sites**: rgedits.com (Ryan Gee) and alexlangworthy.com — aesthetic cues only (geometric tracked uppercase labels, quiet centred-style captions, thin accent hairlines, editorial About with tall portrait, icon footer). Their grid-wall layout was NOT used.

## Brand Colours
- **Dominant (60%)**: `#3A0610` — rich maroon (background). Darker shade `--maroon-deep` (maroon mixed with black) used for the creator strip and footer.
- **Secondary (30%)**: `#FFF3DC` — light cream (text, hairlines, borders; opacity variants for muted text)
- **Accent (10%)**: `#F2A93B` — amber gold (CTAs, view counts, key numbers, italic headline accents)

Palette was derived from the old enesvfx.com (oxblood `#42040B` / cream `#FFECC7` / crimson `#C81627`) and moved to gold so CTAs stand out against maroon.

Typography ("film-title caps", option B — chosen by the editor after rejecting the original Instrument Serif + Jost pairing):
- **Jost** (`--display`, Futura-like) — UPPERCASE, wide tracking for headlines, section titles, CTA bands, step titles, labels, buttons, client names; weight 500 for numbers (stats, view counts, 1.9M). Highlight words in headlines are gold, never italic.
- **Inter** (`--sans`) — body copy, video titles, testimonial quotes (light 300, sentence case).
- No serif and no italics anywhere on the page.

## Funnel Type
- **Type**: DM (X / Twitter)
- **CTA text**: Work with me
- **CTA link**: https://x.com/messages/compose?recipient_id=1803682678266306560 (opens a DM to @enesvfx directly; X user ID `1803682678266306560`)
- **CTA microcopy**: "Opens DMs on X · replies within 24h" (under hero CTA and final CTA)
- The footer X icon still links to the profile (https://x.com/enesvfx) — only `.cta` buttons use the DM link.

CTA locations (7): nav (sticky), hero, band after #02, band after #04, band after #06, About, footer closing.

## Structure Choices
- **Navigation**: Nav bar — sticky, translucent maroon, gold hairline, wordmark left + gold CTA right
- **Hero video**: None — uppercase headline "EDITS THAT KEEP PEOPLE WATCHING." ("WATCHING." in gold), subheadline, CTA, stats column (8M+ / 8 / 3 yrs)
- **Case study style**: Minimal — 16:9 thumbnail (click-to-load YouTube facade), index number, title, client (small tracked caps), gold view count
- **Social proof strip**: Scrolling carousel (pauses on hover, static if reduced motion), ordered by subscriber count
- **About Me section**: Separate — portrait, bio, facts (3 yrs / 8M+ / 8 / EN/PL), niche tags, CTA
- **Retention/Analytics section**: No
- **Extra**: "How it works" 3-step strip (Send footage & brief → First cut in 2–3 days → Revise together & deliver) + "Script to final cut" line

Work layout rhythm (varied, not a grid): 01 full-width → 02 right-offset with giant "1.9M" stat → CTA band → 03 + SunRez quote → 04 offset → CTA band → GF quote + 05 (mirrored) → 06 full-width → CTA band → 07 + 08 staggered pair.

## Videos
| # | Title | Client | YouTube URL | Views shown | Notes |
|---|-------|--------|-------------|-------------|-------|
| 1 | SLIP N SLIDE WORLD CUP FINALS FOOTBALL TOURNAMENT! | LDN Movements | https://www.youtube.com/watch?v=ZsWGp0VH3bc | 220K | Opener |
| 2 | Every Call of Duty Game Explained in 30 Minutes | Ghost Explains | https://www.youtube.com/watch?v=UfvM5Whf8XY | 1.9M (as big stat) | Sold on reach, not editing — editor considers the edit "meh"; never move to #1 |
| 3 | Pokemon Has an Inflation Problem | SunRez | https://www.youtube.com/watch?v=Kf2pkeKLcLI | hidden (230, new) | Paired with SunRez testimonial |
| 4 | Whatever The Football Hits, You Get (WORLD CUP) | SnS | https://www.youtube.com/watch?v=28oRNuo5yg0 | 270K | |
| 5 | We Played 100% of Big Walk | Generational Fumble | https://www.youtube.com/watch?v=ip7oGTYklCo | 190K | Paired with GF testimonial |
| 6 | Całe Toy Story w 26 minut | Prezowski | https://www.youtube.com/watch?v=Qh5sqIGQjt8 | 170K | Polish-language |
| 7 | I Challenged The Best Professional Footballers in Malaysia | LDN+ | https://www.youtube.com/watch?v=LlakZ76KAJE | 150K | |
| 8 | NIKE vs MITRE… The RESULTS SHOCKED Us | FFT | https://www.youtube.com/watch?v=IOTJ6-0jBfE | hidden (19K) | |

Thumbnails load from `i.ytimg.com/vi/<id>/maxresdefault.jpg` with automatic fallback to `hqdefault.jpg`.

## Testimonials
| Client | Quote | Format |
|--------|-------|--------|
| SunRez (4.67K subs) | "Enes has been working so hard to learn my style, humor, and skills. I am so proud of his growth, and I can't wait to see what he can do in the future as we keep collaborating!" | Text pull quote, avatar `assets/sunrez.webp`, next to video #3 |
| Generational Fumble (153K subs) | "Enes worked on parts of this video with us, taking a script and building it to a final product, making adjustments when needed and executing amazingly at every level, would definitely recommend for your videos if you're looking for great communication and work!" | Text pull quote, avatar `assets/generational-fumble.webp`, next to video #5 |

Quotes are verbatim — never edit a client's words.

## Numerical Results
- 8M+ total views across all videos Adrian has edited (phrase as "views on edited videos", not as the total of the 8 shown)
- Per-video views as listed in the Videos table (#3 and #8 deliberately hidden)
- 8 channels edited for · 3 years experience

## Social Proof Strip Creators
| Creator | Subscribers | Avatar |
|---------|------------|--------|
| LDN Movements | 1.48M | assets/ldn-movements.webp |
| SnS | 292K | assets/sns.webp |
| Generational Fumble | 153K | assets/generational-fumble.webp |
| FFT | 120K | assets/fft.webp |
| Prezowski | 77K | assets/prezowski.webp |
| LDN+ | 51.4K | assets/ldn-plus.webp |
| Ghost Explains | 18.3K | assets/ghost-explains.webp |
| SunRez | 4.67K (shown as "Gaming", count hidden) | assets/sunrez.webp |

## Social Links
- X / Twitter: https://x.com/enesvfx (also the CTA)
- Email: edit@enesvfx.com (mailto)
- Discord: @drychester (button copies username to clipboard + toast)

## Assets
- `assets/adrian.webp` — headshot (cropped 4:5 from original photo), used in About and as round avatar in footer
- `assets/ldn-movements.webp`, `sns.webp`, `generational-fumble.webp`, `fft.webp`, `prezowski.webp`, `ldn-plus.webp`, `ghost-explains.webp`, `sunrez.webp` — 200×200 creator avatars for carousel and testimonials

---

## Design Rules (Do Not Break)

These rules apply to ALL future edits:

1. **60/30/10**: Only use the three brand colours above. No new colours.
2. **Hierarchy**: Every case study follows Hook → Secondary Detail → Finisher.
3. **Above-the-Fold CTA**: The CTA must always be visible without scrolling.
4. **CTA Repetition**: CTA appears after every 1–2 case studies and at the bottom. Same text and link every time.
5. **Hick's Law**: 4–8 videos only. If adding a new video, remove the weakest one to stay in range.
6. **Social Proof Priority**: Work first, testimonials second, numbers as a bonus. Never add placeholder sections for proof you don't have.
7. **Anti-Cloning**: Do not restructure the page to match other portfolios. Maintain this editor's unique layout and style.
8. **Trust over hype**: Keep text minimal and grounded. No exaggeration, no salesy language.
9. **Single HTML file**: The portfolio is one file with inline CSS and JS. Keep it that way.
10. **Responsive**: All edits must look good on mobile and desktop.

## Common Edit Patterns

When the editor asks to make changes, follow these patterns:

- **"Swap a video"**: Replace the video embed/thumbnail, title, client name, and description. Update the Videos table above. Ensure the replacement is at the same quality standard.
- **"Add a testimonial"**: Place it inline with the related case study (if detailed style) or add to the testimonials section (if minimal style). Update the Testimonials table above.
- **"Change colours"**: Update all three hex codes in the CSS variables. Check that contrast ratios still work for readability. Update the Brand Colours section above.
- **"Change CTA text or link"**: Update every instance of the CTA on the page (there are multiple). Update the Funnel Type section above.
- **"Add/remove a video"**: Ensure total stays between 4–8. Update the Videos table above.
- **"Update stats"**: Only update with real numbers the editor provides. Never invent stats.

After any edit, update this CLAUDE.md file to reflect the change so it stays in sync with the live site.
