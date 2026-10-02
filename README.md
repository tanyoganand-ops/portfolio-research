# Portfolio research pack

Research date: 2026-10-02. Intended reader: a designer/developer or AI coding assistant building a personal portfolio.

## Recommended direction

Use a normal, easy-to-read portfolio structure with one memorable 3D object and a short scroll-controlled project reveal. Combine Lusion's framed 3D presentation, Blobmixer's soft sculptural form and Fruitful's blurred color layering. Use Dennis Snellenberg as the hierarchy reference. Do not build an entire game unless that is the portfolio's main purpose.

This is a design brief, not finished code. Implementation hints below are proposed ways to recreate patterns, not claims about the reference sites' current source code.

## Taste constraints

- Apple-like clarity: restrained typography, precise spacing, usable controls and obvious navigation.
- Soft curves and a pastel/pastoral color feel. Interpret the Ghibli influence as color, shape and animation, not forests, trees or scenery.
- Layered Gaussian blur, translucent surfaces and selective frosted glass. Keep contrast high and avoid making every surface glass.
- Backgrounds should have depth, texture or controlled color layering. Avoid a generic flat field with plain text boxes stacked over it.
- Animate scroll, hover and click with a consistent motion language. Prefer continuous transitions over a slideshow of disconnected static cards.
- No generic emoji decoration, clip-art or stock chatbot-like layouts.
- References are inspiration for patterns. Do not copy branding, portraits, text, illustrations, models or proprietary code.

## Ranked references

### 1. Lusion: strongest 3D presentation reference

URL: https://lusion.co/

Verified: live official page and desktop pixels inspected. After loading, the hero showed glossy black, white and cobalt sculptural parts inside a large rounded frame. The composition changed between captures. A Page Down moved from the hero toward the next section. This is a limited interaction check, not a complete scroll audit.

What's great: an expressive 3D scene sits inside a disciplined pale page rather than replacing all navigation. Large rounded framing makes the scene feel like a product, not a random canvas experiment.

Patterns to adapt:
- One oversized rounded visual stage with a clear headline outside or above it.
- Contrasting material finishes and a tight accent palette.
- Plain, pill-shaped controls that remain readable over the visual.
- A short transition from the hero into actual project information.

Palette: pale cool/lavender ground, near-black, white and saturated cobalt. For this portfolio, soften the blue and introduce muted peach or sage rather than adopting its whole palette.

Implementation proposal: one Three.js or React Three Fiber canvas; a small number of original meshes; controlled lighting; a scroll timeline that moves the camera or object group. Keep headings and links in normal HTML. Do not infer that this site itself uses React Three Fiber.

Catch: load time was noticeable during this check. Avoid copying a heavy preload experience.

### 2. Blobmixer: strongest soft-shape/material reference

URL: https://blobmixer.14islands.com/

Verified: live and desktop pixels inspected. The Next blob control worked: the view changed from a small purple-blue sculptural form on cyan to a larger orange/pink form on vivid purple.

What's great: one continuous organic shape, reflected light and restrained peripheral controls make a minimal layout feel spatial.

Patterns to adapt:
- A single signature object with smooth curves.
- Material/color transitions tied to project selection.
- Plenty of empty space around the object and unobtrusive navigation.

Palette: multiple colorways; inspected cyan/purple and purple/orange-pink. These examples are vivid, not all pastel. Recolor the pattern to the portfolio's softer palette.

Implementation proposal: an original deformed sphere or authored GLB, a material with controlled roughness and environment lighting, slow rotation, and a short eased transition between states. Keep a static image fallback.

Catch: this is a visual experiment, not a portfolio information architecture. Use its object treatment, not its entire layout. Do not include minting/VR flows in a personal portfolio.

### 3. Dennis Snellenberg: strongest practical portfolio structure

URL: https://dennissnellenberg.com/

Verified: live official page, desktop hero inspected. The large name marquee changed position between captures. Page text confirms Work, About and Contact navigation and a recent-work list. Other hover effects were not tested.

What's great: an immediate identity/role statement, strong scale contrast and very little navigation clutter. The motion does not erase the site's purpose.

Patterns to adapt:
- Oversized type with a concise role statement.
- A short, clearly organized project list.
- One recurring typographic motion motif rather than a different effect on every section.

Palette: grey/black/white in the inspected hero. Borrow hierarchy and restraint, not the monochrome palette or portrait.

Implementation proposal: semantic project links, a CSS transform-based marquee with reduced-motion handling, and a conventional responsive grid. Use a portrait only if supplied and approved; otherwise use an original abstract 3D object.

Catch: do not copy the name, portrait, location badge or client work. Mobile behavior has not been tested in this pass.

### 4. Fruitful: strongest blur-layering reference

URL: https://www.fruitful.com/

Verified: live official page and desktop hero inspected. The current hero uses a pale mint/blue field, soft blurred colored shapes/cards behind crisp text, rounded white controls and green accents. This is a fresh visual check, not a claim based on older palette descriptions.

What's great: the background has depth without making the text hard to read. Rounded controls and soft layering still feel orderly.

Patterns to adapt:
- Keep typography crisp while background layers are blurred.
- Use restrained soft color patches rather than wallpaper art.
- Put a strong action or project selector inside a rounded, high-contrast surface.

Palette: pale mint/blue, white, green accent, with muted color blur behind the hero. Not a verified peach-and-dusty-blue palette in the current hero.

Implementation proposal: a few absolutely positioned gradient/image layers with CSS blur; separately rendered sharp content; subtle transform motion. Limit large blur layers on mobile.

Catch: this is a financial-service site, not a 3D reference. Borrow visual layering, not its money-related copy, form or claims.

### 5. Alma: restrained editorial/texture reference

URL: https://www.almahospitality.it/

Verified: live official page and desktop hero inspected. The hero uses full-bleed interior photography, a very large light wordmark and a spaced navigation row. Cream and muted sage were visible in the cookie panel and room imagery. The cookie panel partly covered the hero; no complete motion audit was performed.

What's great: scale, imagery and breathing room create atmosphere without a forest motif or clip-art decoration.

Patterns to adapt:
- One carefully art-directed visual instead of many unrelated stock images.
- Warm cream and muted sage as supporting tones.
- A large title balanced by a sparse navigation row.

Implementation proposal: original/licensed imagery or rendered project visuals; responsive aspect ratios; small parallax only where it adds depth. Text must remain readable without the visual.

Catch: not a verified 3D-motion reference. Use for palette, texture and composition, not as evidence of an animation technique.

### 6. Ten Years Away: narrative pacing reference

URL: https://ten.375.studio/en

Verified: live; desktop loading/entry and comic-cover pixels inspected. Enter without sound worked and clicking the cover started a scene transition. Later narrative panels and the full scroll behavior were not verified in this pass.

What's great: oversized year typography, a grainy blue ground and a graphic-novel cover communicate a clear narrative premise before the experience starts.

Patterns to adapt:
- Chapters for project stories: problem, intervention, result.
- Strong transitions between a few meaningful scenes.
- A consistent visual language instead of arbitrary effects.

Palette: textured blue-grey, pale cyan type and colorful comic imagery. It is not a pastel portfolio template.

Implementation proposal: a short pinned project scene with 3-4 timeline states, followed by normal HTML content. Do not require an entry gate or sound to view a portfolio.

Catch: loading/entry is too much friction for a recruiter-facing default. Full narrative motion is unverified here.

## Supplementary reference: Bruno Simon

URL: https://bruno-simon.com/

Verified live page text describes a drivable portfolio world, keyboard/touch controls and a Three.js implementation. The current world did not fully load during this visual check, so it is not ranked above as a freshly tested interactive experience.

Useful idea: spatial navigation can make a portfolio memorable, but provide ordinary project links alongside it. Do not make visitors play a game to find contact details.

Historical implementation source: https://www.awwwards.com/bruno-simon-portfolio-wins-site-of-the-month-november.html . This describes the older portfolio, including Three.js, low-poly models and simplified physics. It does not prove the current site uses the same physics stack.

## Proposed build recipe

These are recommendations, not requirements imposed by the reference sites.

1. Build normal HTML first: hero, selected projects, a short about section and contact. Make project destinations obvious before adding effects.
2. Add one original soft 3D object to the hero. Limit the palette to warm cream, pale blue and a muted accent. Keep readable dark text.
3. Add a short scroll story for one featured project. Change object position/scale and a project panel together. End pinning quickly and return to normal scrolling.
4. Use glass for the navigation or one project surface, with blur behind it and enough opacity for contrast. Avoid stacking translucent cards over translucent cards.
5. Use one animation owner per property. Do not let CSS, React springs and GSAP fight over the same transform.
6. Deliver a mobile layout and a reduced-motion mode that show all content without canvas, pinning or animated scroll.

### Technical starting points

- ScrollTrigger documentation: https://gsap.com/docs/v3/Plugins/ScrollTrigger/ . Supports scrubbed animation, pinning and snapping. A timeline can drive related transitions. Review current licensing before adopting it.
- React Three Fiber introduction: https://r3f.docs.pmnd.rs/getting-started/introduction . A React renderer for Three.js; consider it if the build already uses React. Plain Three.js is also valid.
- Lenis official repository: https://github.com/darkroomengineering/lenis . Optional smooth-scroll layer, not a requirement. Start with native scroll and add only if it improves the tested result. Check the exact version's license.

No reference-site code or assets are included in this pack. Public availability is not a reuse license.

### Starter art direction, not sampled colors

Suggested tokens: cream #F4F0E7, mist blue #DCE8ED, sage #AEC2B4, peach #EFCFC1, ink #202628. These are authored starting values, not measured swatches from the sites above. Check contrast on actual components.

## Builder handoff

Before building, inspect the reference URLs and choose a single direction. Produce one desktop and one mobile hero proof with real motion, not a static mockup. Use placeholder content explicitly labeled as placeholder until real content is supplied. Do not invent personal achievements, clients or project results.

Acceptance checks:
- Navigation and all project/contact links work by keyboard and touch.
- Text is readable over every background state.
- Motion is continuous and purposeful; no abrupt slideshow feel.
- Nothing important requires hover, sound or a game mechanic.
- Reduced-motion users get the same content and a clear static composition.
- Canvas failure still leaves a usable site.
- No horizontal overflow on a narrow phone viewport.
- Loading does not hide the identity or navigation behind a long full-screen counter.

## Evidence limits

All listed sites were reached live on the research date. Desktop visual checks are stated per entry. Mobile, performance benchmarking, exhaustive interaction testing and exact dependency/license audits were not completed. Site designs change. Recheck before copying a pattern into a build.
