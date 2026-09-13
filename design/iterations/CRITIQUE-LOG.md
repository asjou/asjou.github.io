# Design critique log: front-guide-B-darkhybrid

Procedure per iteration: full-page screenshot at 1440px, fresh Fable critic with the screenshot only
(no code, no prior critiques), same prompt each time. Target: an independent critic score of 9/10.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v0 (original) | 5/10 | Display face reused on every title; meta row flat; glow underline and three stacked textures; half-hearted lead item; no accent |
| v1 | 5/10 | Sans summaries break the serif premise; hero item unearned; header split into three bands; chip UI generic; section heads at wrong scale |
| v2 | 6/10 | Header still four bands; no lead entry; mono used in too many roles; constant FCC tag carries no information; gutter column underused |
| v3 | 5/10 | Owner direction applied: cool ink, cobalt accent, mono for dates only, serif small caps, deco folio and footer, dinkus, printer's mark, lead entry. Critic: Limelight wordmark, floating date column, lead ratio, ornament count |
| v4 | 5/10 | Dateline moved right, date column top-aligned, lead ratio 1.4:1, double rule under masthead, tinted newsletter panel. Critic: Limelight wordmark, kickers too dim, no strong lead, dinkus and monogram read as filler |

Owner overrides in force since v3: keep Limelight, keep the dinkus and printer's mark, keep the deco face on folio and footer, cool ink not warm, cobalt accent not gold, dockets not in mono.

## Round 3: Shanghai deco palette, new wordmark face

Owner direction: warmer palette from the Shanghai deco study (lacquer, ivory, gold, jade, vermilion), a deco face with more authority at a smaller size, drop the dinkus and printer's mark, folio and footer in serif small caps. Five wordmark candidates were rendered side by side in wordmark-candidates.png. Bodoni Moda in tracked caps was chosen.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v5 | 5.5/10 | Two type scales (lead vs rest); wordmark too light and loosely tracked; single rule under masthead; teal kickers read as dashboard labels; folio-to-newsletter gap |
| v6 | 6/10 | Six equal entries; green button; three rule systems in masthead; mono dates; headline and deck on different measures |
| v7 | 6/10 | Green button; masthead too tight; dateline in nav; mono date beside serif docket; headline orphans; kickers in gold |

v7 as committed carries one unscored tweak after the critique: headline measure widened and balanced to remove the orphan.

Owner rules in force: mono for dates, dockets not in mono, green accent kept, no gold on interactive elements.

## Round 4: owner answers to the grilling

Poiret One ivory wordmark; docket in the kicker line; mono date alone in the margin; vertical rule stopped short of horizontal rules; summaries cut to two lines; new tagline; "Updated" date beside Subscribe; grain 8 percent and stronger vignette.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v8 | 6/10 | Nav weakest element (mixed weights, divider, duplicate Subscribe); horizontal rules between entries fight the vertical rule; lead headline still larger (owner asked for equal, fixed after scoring); mono date vs serif docket; tagline too small; teal button; Bad Labs tag under-marked; footer hierarchy; deck measure too wide |

## Round 5: critic 9 applied in full, jade accent replaces gold

Owner overruled own rules. Applied: one nav weight with a 2px accent underline and no divider, Subscribe removed from nav, row rules removed with space as separator, docket back beside the date in mono, tagline larger, square marker on Bad Labs, accent rule above the folio, footer room and smaller colophon type, summary measure capped, jade accent on every rule and state. No ornaments.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v9 | 6/10 | Right 40 percent of page empty; entries need hairlines back (reverses critic 9); masthead needs a dateline back (reverses owner); headlines too small; kicker glyph inconsistent; mono too cold; newsletter generic; nav underline is a web tab (reverses critic 9); footer thin |

Ten fresh critics over nine iterations: scores 5, 5, 6, 5, 5, 5.5, 6, 6, 6, 6. Critics 9 and 10 reverse each other on row rules, nav underline, dateline, and ornament.

## Round 6: centred column

Page narrowed to an 830px centred column. Headlines 34px. One kicker system: type muted, tag in ink, Bad Labs red. Courier Prime replaces IBM Plex Mono. Non-breaking hyphen in CopyPaste-2 fixed after scoring.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v10 | 6/10 | Six identical entries, wants a lead (reverses owner); 90px gaps, wants hairlines back (reverses critic 9); masthead needs a dateline (reverses owner and critic 9); mono too grey; kicker colours; hyphen break in CopyPaste-2 (fixed); nav underline (reverses critic 9); texture; newsletter coupon; colophon |

Eleven fresh critics, ten iterations. Scores: 5, 5, 6, 5, 5, 5.5, 6, 6, 6, 6, 6. Since v6 every critic states the page shows no AI-generated tells. The remaining top-ranked items reverse from critic to critic.

## Round 7: cool white ink

Ink changed from ivory to cool white, dim grey cooled, ground moved from warm brown-black to neutral near-black.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v11 | 6/10 | Hairlines between entries (reverses critic 9); replace tagline with an edition line (reverses owner); nav undesigned; kicker and tag pairing muddy; pick one accent; newsletter coupon; pagination on one line; titles wrap; texture |

Twelve fresh critics, eleven iterations. Scores: 5, 5, 6, 5, 5, 5.5, 6, 6, 6, 6, 6, 6.

## Round 8: generated plates and lit surfaces

Owner direction: more personality; image generation; shading and 3D effects combined with images; verify frame by frame in the browser. No image-generation model was available, so three plates were drawn as SVG (turbulence, displacement, blur, vignette, grain) and rendered to bitmaps in headless Chromium. Source for all three is in design/img/plates-source.html.

Applied: blinds plate behind the masthead (light through venetian blinds, smoke, fades into the ground); wordmark as cut metal on the wall (lit top edge, four-step extrusion, long soft cast shadow down-right, matching the blinds light); sticky strip as a lacquer bar with a lit top edge and a shadow onto the page; the Bad Labs record carries an inked, worn vermilion seal set 11 degrees off square; newsletter panel under a lamp cone with dust in the beam, bevelled Subscribe key; fog rising from the foot of the page. Type, palette and ledger unchanged from v11.

Verification: viewport frames every 720px of scroll at 1440px and 400px, plus 1024px full page, hover and focus states on the button. Three defects found and fixed before scoring: seal overlapped the kicker on phones (moved beside the date lines), nav wrapped to two lines on phones (one line, scrolls sideways), lamp cone ended in a hard edge at the box bottom (faded into the ground).

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v12 | 7/10 | Dead width at 1440 (reverses owner: centred column); six equal entries, wants a lead (reverses owner); labels, deks and dockets in near-identical greys; newsletter box oversized for its content, green button clashes; footer thin. Imagery: masthead and seal carry the noir conceit; lamp cone on the edge of decoration |

Thirteen fresh critics, twelve iterations. Scores: 5, 5, 6, 5, 5, 5.5, 6, 6, 6, 6, 6, 6, 7. The three top items in v12 are all reversals of standing owner decisions.

## Round 9: critic gaps worked, Limelight wordmark, seal withdrawn

Owner direction: follow the v12 critic on the remaining gaps; a more noir or art deco masthead face; take out the red Bad Labs seal.

Rig defect found and fixed this round: inside the sandbox browser the Google Fonts stylesheet request was reset, so the v12 screenshots, the v12 critic score and the v12.png in this folder were rendered with fallback faces. The rig now fetches the fonts through curl and serves them to the browser. v12.png is regenerated with the real faces; the v12 score of 7 stands as recorded but was given on fallback type.

Wordmark: eighteen faces rendered on the blinds plate with the cut-metal treatment (wordmark-candidates-2.png). Limelight chosen: the one face that is both deco and noir, and the treatment turns it into a marquee. Runner-up Fascinate Inline.

Applied from the v12 critic: right rail at 1100px and up (newsletter card, counts by type and tag, a line from the record) so the page uses its width; a lead record one size up with a three-line summary in ink and a rule beneath; three grey tiers (ink for titles, tags and dates; a brighter dim for summaries; ash for labels, dockets and colophon); nav links in ink so the bar anchors the top; newsletter cut to a rail card with a bone key, no green on any control; footer with a masthead echo, a sections reprise and the colophon. Seal withdrawn and its plate removed.

| Iteration | Score | Main gaps named by the critic |
|---|---|---|
| v13 | 7/10 | Items two to six identical after the lead, wants a second tier; blinds plate inert behind the wordmark and cut hard at the nav; rail runs out of content by mid-page; metadata column and headline block do not share a baseline; newsletter card and Bad Labs red read as tonal outliers. Wordmark: nails deco, tips toward marquee; wants a flatter fill and tighter tracking |

Fourteen fresh critics, thirteen iterations. Scores: 5, 5, 6, 5, 5, 5.5, 6, 6, 6, 6, 6, 6, 7, 7.
