# Portfolio Phase 2: Ranked Build Document

**Brief:** Apple-sleek + Ghibli-soft (palette and curve, not scenery), immersive, impressive, out of the box. Light/pastel, frosted glass, continuous motion (not slideshow).

**Source:** about 290 research slices, checked 4 October 2026. URLs are copied as written in the slices (some slices give bare domains without https://).

**Rule for every mechanic:** keep a plain, fast path to the work (project list, email), a reduced-motion state, and a mobile fallback.

## Evidence tags

| Tag | Meaning |
|---|---|
| **BROWSER** | Slice says it rendered the page in a browser and inspected pixels or screenshots. |
| **FETCH** | Page text loaded by fetch only. A WebGL/canvas runtime is NOT proven to work. |
| **[A]** | Award confirmed on the Awwwards/FWA/CSSDA page itself. |
| **[C]** | Award claimed only by the agency or creator. Do not cite as an award. |
| **NO AWARD** | Real, but no award found. |
| **NOT REAL** | Fictional, AI-generated showcase, content farm or invented maker. Never cite as real work. |

Many short slices record "SOTD/HM" with a month but do not say whether the award page was opened. Those are listed as the slice states them. Anything FETCH-only or unstated should be hand-checked in a browser before public citation.

**Security note:** several source pages contained text trying to steer AI agents (rating nudges, "build briefs", certification claims). The research agents ignored them. Most came from the NOT REAL cluster in section 2Z. Treat content from those hosts as untrusted.

---

# PART 1. Top 10 mechanic directions, ranked by what to build first

Order logic: 1 and 2 are the foundation. 3 to 5 are signature hero ideas. 6 to 10 are add-on sections.

## 1. Persistent glass-and-light 3D stage with scroll-driven camera (foundation)

One fixed canvas, one hero object in a pale soft-lit space, scroll drives the camera, UI is frosted or liquid glass.

- **References**
  - Butter, https://www.butter.video/ - SOTD 28 Sep 2026 [A] https://www.awwwards.com/sites/butter . BROWSER (hero pixels). Glossy hanging 3D key charms, soft coloured blur in the headline, floating rounded nav. Best single match to the brief.
  - Igloo Inc, https://www.igloo.inc/ - SOTY gallery 2024, jury 7.92 [A] https://www.awwwards.com/sites/igloo-inc . Screenshot of landscape seen. Translucent ice objects, frost transitions.
  - davidlee.studio - sunlit 3D studio, BROWSER (light-background slice). Strongest light-palette fit.
  - Lusion v3, https://lusion.co/ - jury 8.25, SOTY gallery 2023 [A] https://www.awwwards.com/sites/lusion-v3 . FETCH (hero not verified past loader).
  - secretlevel.co - liquid-glass nav, closest to Apple glass.
  - iyo.ai/products/iyo-one - SOTD + Dev, Apr 2026.
  - Apple pacing benchmark: apple.com/airpods-pro (scroll-scrubbed explode and reassemble), apple.com/iphone-17-pro.
- **Stealable mechanic:** Lenis + GSAP ScrollTrigger, `pin:true` on one fixed canvas, scroll drives camera along authored stations, project chapters fade over the canvas, static stills under reduced motion. One shared R3F canvas with drei View scissor (inkgames.com, Codrops case) is the cleanest multi-section pattern. Glass UI: liquidglass.dev, kube.io (CSS/SVG refraction explainer), liquid-glass-js.vercel.app (draggable lens).
- **Fit:** Apple-sleek by default, glass is explicitly in the taste, and the light variant is nearly unclaimed (most references are dark).
- **Difficulty:** Medium. Main risk is mobile performance. Use quality tiers (ZERO Codrops case: under 10MB, 60fps budget on Android).

## 2. Spatial project world: curved wall or miniature diorama as navigation

- **References**
  - Jesper Landberg, http://jesperlandberg.com - SOTD 29 Sep 2026, Dev 8.17 [A] https://www.awwwards.com/sites/jesper-landberg-4 . Curved room-like carousel above a perspective grid. Strongest portfolio reference in the corpus. Animation not browser-verified.
  - Colonia Zacamil, https://coloniazacamil.com/ - SOTD 1 Oct 2026 [A] https://www.awwwards.com/sites/colonia-zacamil . BROWSER. Navigable miniature neighbourhood with routes and day/night states.
  - Messenger (Abeto), https://messenger.abeto.co/ - Developer Site of the Year, jury 7.92 [A] https://www.awwwards.com/sites/messenger . BROWSER (planet seen). Tiny hand-drawn spherical world as project map.
  - duroc.ma - SOTD + CSSDA + FWA 2025, aerial miniature amusement park, attractions are navigation.
  - water-scene.unseen.co - Unseen Labs pool diorama, soft rounded 3D, BROWSER. No award verified.
  - aimees-papercraft-world.com - folded-paper world, open source: github andrewwoan/aimees-hand-drawn-papercraft-folio.
- **Mechanic:** projects are places in one small world. Camera glides between them, home is a readable overview. Day/night toggle (Zacamil) doubles as light/dark mode.
- **Fit:** closest thing to Ghibli form without painting scenery. Keep soft rounded geometry, cream and sage.
- **Difficulty:** Medium-High (authored assets). Cheaper variant: curved wall of project frames (Landberg).

## 3. Rain-on-glass and water-and-light as the hero material

- **References**
  - DISANTINO Water, https://disantinowater.com/ - Awwwards HM, not SOTD [A] https://www.awwwards.com/sites/disantino-water ; case https://www.byfugu.com/work/disantinowater ; element https://www.awwwards.com/inspiration/water-drop-on-glass-effect-disantino-water . BROWSER shows a light grey editorial site. The glass-drop section itself was not isolated.
  - Codrops RainEffect (Lucas Bebber, 2015), https://tympanus.net/Development/RainEffect/ - NO AWARD. BROWSER (renders). Only documented bead, merge, fall, trail logic. Source https://github.com/codrops/RainEffect (building on it allowed, no redistribution as-is).
  - Anderson Mancini water, https://water-simulation.vercel.app/ - HM 25 Jun 2025 [A] https://www.awwwards.com/sites/3d-realistic-water-experiment . BROWSER (Dive transition, caustics, droplets).
  - Canvas UI droplets, https://canvasui.dev/docs/components/droplets - NO AWARD, BROWSER. Pointer wipe radius and strength exposed. Uses an experimental HTML-in-canvas API, so needs a fallback.
  - CrazyGL rainy glass typography, https://crazygl.com/hero/rainy-glass-typography - NO AWARD. Young low-provenance library (GitHub org created 20 Jun 2026). Audit licence and package first.
  - Gentle Rain (Zajno), https://gentlerain.ai/ - SOTD [A] https://www.awwwards.com/sites/gentlerain-ai . Soft caustic light plus dithering, warm earth tones. Case https://tympanus.net/codrops/2025/01/16/case-study-gentle-rain/ . Some graphics are AI-assisted by the case study's own account. Not literal rain.
- **Mechanic:** pale frosted pane, tiny static beads, a few drops grow, merge, run and leave trails. A drag-wipe clears fog to reveal a project title. Navigation stays outside the fogged layer.
- **Fit:** frosted glass is the taste brief. Soft, cool to warm.
- **Difficulty:** Medium (Codrops source gives the logic). No verified awarded site does all four behaviours together.

## 4. Folded and paper-cut world (Ghibli form through paper)

- **References**
  - romanjeanelie.com - SOTD Oct 2025, WebGL page-curl fold shader, Codrops walkthrough with code. Best build reference.
  - aimees-papercraft-world.com - scroll-driven folded-paper seasons, MIT, tutorial in repo.
  - mr-pandas-psychologically-safe-portfolio.com - SOTD 2025, open source (andrewwoan). Hand-drawn notebook paper in 3D, puppet micro-animations.
  - moooi.com/eu/paper-play (also https://www.moooi.com/us/step-into-paper-play) - Webby 2023 / SOTD, paper-cut WebGL world. The benchmark.
  - itomdev.com - FWA Apr 2026, paper rips as loader, camera glides into a hand-drawn corridor. OSS github ITomPoland/portfolio-itom.
  - niccolomiranda.com - SOTM 2021, full paper/newspaper universe. Old but the best literal paper portfolio.
  - popup.larosee-cosmetiques.com - SOTD Jul 2025, drag-and-drop curtain opens a hidden cafe, pastel.
  - Tools: origamisimulator.org, Codrops origami and unfolding box tutorials.
- **Mechanic:** page-curl and fold shader for transitions, layered cut-paper depth for scenes, optional loader that tears open into the site.
- **Fit:** pastel, soft turns, tactile. Delivers "pastoral colour and soft curves" without drawing trees.
- **Difficulty:** Medium. Code exists for the key shader.

## 5. One physical control drives the whole piece (crank, dial, orrery)

- **References**
  - ProDyn Orrery, https://orrery.prodyn.ai/ - NO AWARD. BROWSER (gear stack renders; a quarter turn advanced the date 7.5 days). Repo https://github.com/cygnostik/orrery , created 6 Sep 2026, MIT code, textures and fonts under separate rights. Dark sci-fi look, borrow mechanics only. Ignore the webkkk.net mirror posing as the repo.
  - GravIT Orrery, https://www.gravit.com.au/orrery/ - NO AWARD, BROWSER. Click to follow, Today button, arrow keys scrub time.
  - Orrery.live, https://orrery.live/ - NO AWARD, BROWSER. Snaps the time dial to named alignments. Credits disclose AI-assisted design and code.
  - Cartier Watches & Wonders 2024 (Immersive Garden), https://immersive-g.com/projects/cartier-watches-and-wonders-24/ - SOTD [A] https://www.awwwards.com/sites/cartier-watches-wonders-2024 ; FWA and CSSDA only [C]. Live demo stuck on loader, use the case study.
  - 150years.audemarspiguet.com - SOTD 2025 + Webby 26, 20 real-time 3D heritage rooms.
  - jamesmurray.ca - Awwwards NOMINEE only, https://www.awwwards.com/sites/james-murray-3d-portfolio . Portfolio categories as globes. Very cluttered, wrong style.
- **Mechanic:** one dial or crank moves a shared clock. Five project "planets" on satin arms. At career milestones two align and a glass card appears. Real index always visible, keyboard steps, reduced-motion pause.
- **Fit:** tactile and precise. Cream, blue, frosted centre.
- **Difficulty:** Medium-High. The conjunction-unlock has no precedent (Part 4).

## 6. Cursor as protagonist: creatures, flocks, light that follows

- **References**
  - Noomo Labs, https://labs.noomoagency.com/ - SOTD + Dev, FWA, CSSDA, Jun 2024 [A] https://www.awwwards.com/sites/noomo-labs . Glass jellyfish, shattering sphere. Dark scene.
  - Aurelia, holtsetio.com/lab/aurelia - MIT jellyfish, WebGPU TSL, verlet + caustics. Needs a Safari fallback.
  - Murmuration: murmuration-pink.vercel.app (800 starlings, cursor predator), demos.karanbansal.in/murmuration (8000 birds, hawk cursor), github swarmphony (4096 GPU birds, 7-nearest-neighbour model).
  - Zichen Yuan "A cursor is a kite", https://a-cursor-is-a-kite.yuanzichen.com/ - BROWSER, coverage https://waxy.org/2025/04/a-cursor-is-a-kite/ . Cursor as tether, lagged follow, weather gusts. No award.
  - cynx.io (HM 26, liquid WebGL cursor), dashcreative.co (HM 26), itsmarga.me (SOTD, mask-reveal trails), victor-sin.com (HM 26).
  - cuberto.com cursor: public code (cuberto.com/blog/cursor-magnetic-js-component, mouse-follower lib).
  - Do not copy Lusion Labs code (its devs object publicly).
- **Mechanic:** GPU boids with the pointer as attractor or repulsor. The flock settles onto project positions. Frosted-glass creatures on a light background are the differentiator.
- **Fit:** alive, continuous motion, not a slideshow.
- **Difficulty:** Medium (boids) to High (WebGPU, Safari fallback).

## 7. A short playable hero that reveals a project (not a whole game)

- **References**
  - The Tie-break, https://thetiebreak.merci-michel.com/ - SOTD 25 Sep 2026 [A] https://www.awwwards.com/sites/the-tie-break . Playable tennis hero into shoe reveal.
  - Cinnamon, cinnamon.co.uk - HM Apr 2026, claw machine as project nav. Best portfolio model for gacha.
  - gacha-liard-seven.vercel.app - May 2026, portfolio as 3D gacha machine, OSS repo. Closest match, not awarded.
  - bfcm.shopify.com - SOTD 7.56, playable pinball with live data globe.
  - martin-laxenaire.fr - HM 25, portfolio-as-game, compute-shader physics, OSS.
  - OUIGO Let's Play, https://letsplay.ouigo.es/ - jury 8.40 [A] https://www.awwwards.com/sites/ouigo-let-s-play . BROWSER (pinball seen). Live Spanish edition, not the original 2017 build.
  - Don't Board Me, https://dontboardme.com/ - tennis-ball intro [A] https://www.awwwards.com/sites/dont-board-me . BROWSER.
  - Bruno Simon was rejected earlier as too gamified. Keep this to one short interaction.
- **Mechanic:** Matter.js or Rapier. A ball or capsule drop picks a project, and the visitor can skip.
- **Difficulty:** Medium.

## 8. Exploded and cutaway object story

- **References:** iyo.ai/products/iyo-one (SOTD + Dev Apr 2026, Z-axis teardown, hover pulls a component forward; https://www.awwwards.com/inspiration/interactive-webgl-exploded-view-iyo), solutions.alphanelabs.com (HM 25, orthographic blueprint peeled layer by layer), yomy.care (robot assembles on scroll), neoconda.com (HM 26), apple.com/airpods-pro (benchmark), vision.avatr.com (FWA, frame-by-frame orbit), audemarspiguet.com code-1159-universelle.
- **Mechanic:** scroll pulls a hero object apart along Z with thin-type labels, then reassembles. Use it for the "about me" (skills as layers).
- **Difficulty:** Medium (needs a modelled object; frame-scrub is the cheaper route).

## 9. Light and shadow reveal

- **References:** moooi.com/us/step-into-paper-play (Webby 23, visitor spotlight), killianherzer.com (HM 26, flashlight hero), matcha-cartel.com (HM Jun 26), artprize-shadows.com (SOTD 2025), alanwake.fun (Sep 26, unawarded, exact beam reveal). Parts: Codrops relighting images with depth maps (Aug 26, github DGFX/codrops-relightning-images), crucibleui.com lantern component.
- **Mechanic:** a soft beam (pointer or slow auto sweep) reveals content. Lighthouse version: one `beamAngle` state, atan2 angle difference per card, CSS-variable brightness (see Part 4 for the source caution).
- **Fit:** make it warm daylight or dusk pastel, not noir.
- **Difficulty:** Low-Medium.

## 10. Persistent state: something that grows or remembers the visitor

- **References:** bruno-simon.com (SOTM Jan 2026, 8.11; the "whispers" are visitor-written messages, not audio), play.garance.com (CSSDA WOTD + SOTD 25, forest grows as visitors plant), edwson.com/project-ma.html (2026, zen sand garden with season and sun sliders, shareable state), ihaveagarden.com (real-time plant), nature-beyond.tech (HM [A] https://www.awwwards.com/sites/nature-beyond-technology ; Codrops https://tympanus.net/codrops/2025/12/04/crafting-nature-beyond-technology-a-project-from-roots-to-leaves/ ), utopiatokyo.com (SOTD Mar 26, skill points generate a 3D mask).
- **Mechanic:** localStorage state. Return visits show change (a tree has grown, a tide has moved). Optional shareable keepsake image.
- **Difficulty:** Low-Medium for state, High for a quality asset.

---

# PART 2. Verified live references, grouped by category

Status per line: BROWSER = pixels inspected, FETCH = text only, [A] = award page checked, [C] = award claimed only. NOT REAL items are collected in 2Z, not mixed in here.

## 2A. Current award winners (21 Sep to 4 Oct 2026)

All fetched. Hero pixels seen for Colonia Zacamil, Butter, Moto Finance, Milledollars.

| Site | URL | Award | Note |
|---|---|---|---|
| Jesper Landberg | http://jesperlandberg.com | SOTD 29 Sep [A] https://www.awwwards.com/sites/jesper-landberg-4 | curved spatial wall |
| Colonia Zacamil | https://coloniazacamil.com/ | SOTD 1 Oct [A] https://www.awwwards.com/sites/colonia-zacamil | BROWSER |
| CoMinVi | https://www.cominvi.com.mx/ | SOTD 30 Sep [A] https://www.awwwards.com/sites/cominvi | sculptural rock + type |
| Butter | https://www.butter.video/ | SOTD 28 Sep [A] https://www.awwwards.com/sites/butter | BROWSER, best fit |
| MEER MOHSIN | https://www.meermohsin.me/ | SOTD 26 Sep [A] https://www.awwwards.com/sites/meer-mohsin | red grain, cinematic |
| Moto Finance | https://www.moto-card.com/ | SOTD 24 Sep [A] https://www.awwwards.com/sites/moto-finance | BROWSER. One slice excludes it over a "destination concern"; check before citing. |
| Milledollars | https://milledollars.fr/ | SOTD 2 Oct [A] https://www.awwwards.com/sites/milledollars | BROWSER |
| The Tie-break | https://thetiebreak.merci-michel.com/ | SOTD 25 Sep [A] https://www.awwwards.com/sites/the-tie-break | playable hero |
| Gil Huybrecht | https://gilhuybrecht.com/ | SOTD 21 Sep [A] https://www.awwwards.com/sites/gil-huybrecht | contact-sheet index |
| Realevate | https://realevate.agency/ | SOTD 27 Sep [A] https://www.awwwards.com/sites/realevate | |
| Tengile MalaMala | https://tengilemalamala.com/ | SOTD 3 Oct [A] https://www.awwwards.com/sites/tengile-malamala-collection | luxury editorial |
| EDOLUS | https://edolus.com/ | SOTD 4 Oct [A] https://www.awwwards.com/sites/edolus | **UNVERIFIED**: fetch empty, browser reached loader only |

## 2B. All-time and annual award references

All 10 fetched. BROWSER screenshots confirm Igloo, KPR, Messenger, OUIGO, Noomo and Don't Board Me.

| Site | URL | Award |
|---|---|---|
| Lusion v3 | https://lusion.co/ | jury 8.25, SOTY gallery 2023 |
| Igloo Inc | https://www.igloo.inc/ | jury 7.92, SOTY gallery 2024 |
| KPR | https://kprverse.com/ | jury 7.98, SOTY gallery 2022, https://www.awwwards.com/sites/kpr |
| Bruno Simon 2019 | https://2019.bruno-simon.com/ | jury 8.04, SOTY 2019 (only reached START) |
| Messenger | https://messenger.abeto.co/ | Dev SOTY, jury 7.92 |
| Lando Norris | https://landonorris.com/ | jury 8.18, official 2025 SOTY + Users' Choice |
| OUIGO Let's Play | https://letsplay.ouigo.es/ | jury 8.40 |
| Mana Yerba Mate | https://en.manayerbamate.com/ | jury 8.03, gallery 2023, https://www.awwwards.com/sites/mana-yerba-mate |
| Noomo Agency | https://noomoagency.com/ | jury 7.72, Users' Choice 2023 |
| Don't Board Me | https://dontboardme.com/ | jury 7.83, gallery 2024 |

Bruno Simon current, https://bruno-simon.com (SOTM Jan 2026, FWA Site of the Year 2025, CSSDA 8.84 Best Portfolio): real and strong, but the user rejected it earlier as too gamified. The 2025 build is vanilla three + Rapier + WebGPU, not R3F.

## 2C. Studio and agency self-sites

- Orage https://orage.studio/ (SOTD 29 Oct 2025, draggable video masks)
- LEOLEO https://www.leoleo.studio/en-gb (SOTD 20 Jun 2025)
- Ribbit https://ribbit.dk/ (SOTD 24 Nov 2025)
- Sileent https://www.sileent.com/ (SOTD 10 Feb 2026)
- Flabbergast https://flabbergast.agency/ (SOTD 19 Oct 2025)
- 2xA https://2xa.studio/ (SOTD 31 Jul 2026)
- HOBRO https://hobro.digital/ (SOTD 29 Aug 2026)
- Revelatio https://revelatio.studio/ (SOTD 12 Aug 2026)
- MIUX https://madeinuxstudio.com/ (designer-documented SOTD/FWA)
- FUTURE THREE https://www.futurethree.studio/ (HM only)
- Nine to Five https://www.9to5studio.it/ (SOTD 2026, architecture studio)

All fetched. Screenshot review partial (heavy sites stalled at loaders). Excluded by the slice: Swell (creator claims SOTD, official page says HM) and Phantom (dated 2024).

Others from stubs (mostly text-fetch): labs.lusion.co (SOTD 7.58), wrapped-party.activetheory.dev (SOTD 7.31), resn.co.nz (8.57), immersive-g.com, makemepulse.com, dogstudio.co, unseen.co, activetheory.net, locomotive.ca, basement.studio, 14islands.com. BROWSER: obys.agency, mouthwash.studio, bureauborsche.com, pentagram.com, xx.studio, dia.studio, gt-mechanik.com.

## 2D. Personal portfolios

jordan-breton.com (FWA SOTD Oct 25) | joseph-san.com (Apr 26, single camera take, github JosephASG) | itomdev.com (FWA Apr 26) | cynx.io (HM, strongest portfolio ref per its slice) | stabondar.com (SOTD 25) | aurelienvigne.com (SOTD May 25, raccoon + theatre, Codrops breakdown) | gnrm.se (SOTD 7.53) | corentinbernadou.com | minhpham.design | artemshcherban.com | mersi-architecture.com (SOTD, split-screen, Codrops making-of) | pacomepertant.com (7.76) | cydstumpel.nl | arnaudrocca.fr | stefanvitasovic.dev | edoardolunardi.dev (/lab) | henryheffernan.com (3D CRT bedroom; MIT source os.henryheffernan.com) | sooahs-room-folio.com (HM Feb 25, OSS github.com/andrewwoan/sooahs-room-folio) | rleonardi.com/interactive-resume (FWA + Awwwards + CSSDA) | jesse-zhou.com (isometric ramen shop) | office.graffico.it (WASD studio) | jaredwalte.rs (signal-tuner portfolio, BROWSER, not awarded). Mostly text-fetch grounded.

## 2E. Material and effect references

- **Water, rain, glass:** see Part 1 item 3. Also xe.works (CSSDA WOTD Apr 25, glass ring refracts live DOM), dorianlods.fr (HM Aug 25), mesh3d.gallery/the-state-of-the-gallery (SOTD + Dev Aug 26, oil-slick bulge), vgpu.sh (Codrops 26, prism), dasprinzip.com/tinker/day42.
- **Gooey and liquid transitions:** anima.ai (HM Jan 26), springs.house (SOTD + Dev), fromanother.love (SOTD May 26), aerleum.com, madeinmay.studio, victor-sin.com.
- **Gradient and aurora:** velizardelyanov.com, contemporarytype.com, studiohazey.com, myhealthprac.com, beatfic.jp. Code: grainient.supply.
- **Holographic:** mesh3d.gallery/the-state-of-the-gallery, glossy.wannathis.one, dorianlods.fr, atolldigital.com, crucibleui.com/backgrounds/iris.
- **Grain and dither:** partial. estacionvenenta.com, mattrothenberg.com, aidandombrowski.com/work/dither-dog. Weak category.
- **Paper, clay, tactile:** clayboan.com (SOTD Aug 25), clay.com (Rube Goldberg hero, no award), ponpon-mania.com (SOTD Oct/Nov 25), tearthepaperceiling.org (HM May 25), seated.com (HM Dec 25).

## 2F. Motion, type and interaction components

- **Cursor and hover:** cuberto.com (code public), dennissnellenberg.com (SOTD, https://www.awwwards.com/sites/dennis-snellenberg), lusion.co, itsmarga.me, magnetism.fr.
- **Kinetic type:** matvoyce.tv (use this domain only, see 2H), exat.hottype.co (SOTD, Codrops Apr 26), squeezy.overnice.com (HM, github overnice), fontgauntlet.com, magnettype.com.
- **Page transitions:** dennissnellenberg.com (curved SVG wipe, most copyable), fromanother.love, flim.ai, aristidebenoist.com, daveholloway.uk (GSAP Flip).
- **Loaders (recordings inspected, BROWSER):** 3dhouse.schumacher.com (loader is a doorway), kprverse.com, quechua-lookbook.com/ss25, ph.demiladehq.com.
- **Footers** (all fetched; ranking is editorial, not an interaction test): https://labs.noomoagency.com/ (SOTD) | https://0110studio.ca/ (HM) | https://makhnostudio.com/ (SOTD) | https://inkwell.tech/ (SOTD, contact as final scene) | http://www.mansellmade.com/ (HM, click-to-copy email) | https://nographism.com/en/ (HM) | https://dtampe.com/ (HM) | https://dennissnellenberg.com/ (SOTD). Bonus https://www.studiobo.io/ (nominee only, Rive lion).
- **Contact pages:** immersive-g.com/the-studio/contact-us, toyfight.co/connect, dversostudio.io, rabenrifaie.com/#contact.
- **About pages (browser-inspected):** stabondar.com, glenncatteeuw.com/about, seanhalpin.xyz/about, alinbuda.com/timeline.
- **Scroll video and frame scrub:** apple.com/airpods-pro (standard), qorion.net/work/vesna, dappasol.com/streetsofpunk, makoai.studio/work/scrollhouse.
- **Audio (verified in browser):** jazz.computer, soundoftheearth.org, jazzkeys.plan8.co, typatone.com. Also intrusionproject.com, mola-zone.com (SOTD + FWA). Keep sound optional with an explicit toggle.
- **Mobile and device motion:** tiltoootilt.tote.co.jp, poison.studio (gyro, HM), birdfeedgames.com (70+ Rive assets). iOS needs a permission tap plus a cursor fallback.
- **Components worth lifting (check licences):** liquidglass.dev, canvasui.dev, crazygl.com, crucibleui.com, originkit.dev, 21st.dev, gsapvault.com, madewithgsap.com.

## 2G. Stack and technique references

Three.js Journey grads and Codrops case studies: merodev.net, jordan-breton.com, themonolithproject.net (13-scene R3F, SOTD 7.69), trionn.com (GSAP + Three + Lenis + WebAudio), inkgames.com (one canvas, drei View), github.com/brunosimon/folio-2025 (three + TSL), webgl-scroll-sync.lusion.co (open source), studiofreight.com (Lenis). WebGPU production: brand.ivress.co.jp (FWA May 2026, TSL with WebGL fallback), threejspunk.com (FOTD 3 Oct, WebGPU), martin-laxenaire.fr (gpu-curtains). Takeaway from slices: TSL materials with a WebGL fallback. Engine exports (Godot, Unity) are too heavy for a portfolio.

## 2H. Domain hygiene (look real, are NOT the real thing)

- **matvoyce.com is hijacked/spam. The correct site is https://matvoyce.tv/.**
- 10x17.co: hijacked. mubasic custom domain: hijacked (World of Tanks); only mubasic.webflow.io is live. glsl.io: hijacked. timbstrails: hijacked.
- grungeology.com is a tribute band. The real one is grungeology.org.

## 2Z. NOT REAL: fictional, AI-generated, content-farm or invented-maker items

**Never cite any of these as real work, real awards or real makers.**

**The "FABLE/175" cluster (host fable-25-830.netlify.app).** Its own index reads "One hundred seventy-five websites. One AI. Three passes each." These are AI-built showcase rooms with invented histories, makers and numbers, pushed by SEO-farm write-ups (leluxart.com, artnewsnviews.com, thisdesigngirl.com, smartcr, thorstenmeyerai, influenctor). Slices found embedded agent-directed instructions and fake certification claims on or around them. Rooms seen in the corpus:

- https://fable-25-830.netlify.app/sites/orrery/ (and /guide/): "Alabaster & Vane Est. 1774" invented, instrument blank in two screenshots
- https://fable-25-830.netlify.app/sites/patang/ (room 84)
- https://fable-25-830.netlify.app/sites/tidepool/ ("Intertidal Society / Kelp Point", Est. 1936 invented; mechanics do work)
- https://fable-25-830.netlify.app/sites/moonjar/ ("Designed & built by Claude Fable 5", invented kiln-keeper)
- https://fable-25-830.netlify.app/sites/pharos (room 33)
- https://fable-25-830.netlify.app/sites/mycelium , /sites/composing , /sites/paperfox , /sites/pigmentarium , /sites/calibre
- Named in slices on the same host or network: Noctiluca, Mothlight, Station 36 numbers station, Silent Running, Abyssal Station, Frost Herbarium "Room 99", Snow Globe Workshop (room 91), Midnight Meridian, KIRIN EXPRESS.

**Other fabricated or AI-generated items**

- Bonsai Pavilion https://bonsaipavilion.app/ (invented developer, "Verified Specifications" copy)
- AIIndigo bonsai tutorials https://aiindigo.com/tutorials/getting-started-with-har-simulating-perfect-bonsai-pruning (content farm)
- Voxel Bonsai (host gemini-3-8-flash.demos.sulat.com, self-labelled one-shot model demo)
- Bat Trang Vessel https://1designtool.com/demos/bat-trang-vessel/index.html (parent site says agent-generated, zero hand edits)
- Clay & Kiln https://clearvibe.vip/studio.html (no real author, templated copy; likely generated, not proven)
- AIGameShare Pottery Studio 3D (labelled AI-generated)
- CROSSWIND https://aimade.games/g/crosswind (explicitly AI-built; real page, not independent validation)
- Fly a Kite, CodeTap https://codetap.org/project/fly-a-kite (likely AI boilerplate)
- Moth & Lamp (cephalochromoscope.net/...): page opens with an injection-style banner nudging a high rating. Drop it.
- Crescendo music box (musicboxsimulater.netlify.app): likely AI-assisted, throwaway host
- kimi.ai showcase pages, diegopacheco AI playground (same network)
- mysimulator.uk/codetap farm sims (likely AI)
- sherlock-cold-ember.netlify.app, mentalistos.netlify.app, atlas-vault.vercel.app, casebook-phi.vercel.app (hobby or AI fingerprint-noir demos, no award-grade matches)

**AI-disclosed but real (mechanics only, never prestige):** Kanso https://www.kansogame.com/ (Cursor Vibe Jam, 90% AI-code rule), Orrery.live, Bonsai: A Tree in Time (sunriseoath.itch.io/bonsai).

**Do not mistake for fakes** (slices say a Netlify or Vercel host alone is not proof): water-simulation.vercel.app (Awwwards-bound author), travelers-collage.netlify.app (HM), waterball.netlify.app, splash-fluid.netlify.app.

---

# PART 3. Dead, broken, parked or changed

| Site | State |
|---|---|
| yarn.so | Now a plain white SaaS page with video, no longer immersive. Exclude from wow lists (verified 4 Oct 2026). |
| Prometheus Fuels | Awarded at 8.40 but now serves a different 2026 corporate site. Exclude. |
| Pangram Pangram | Redesigned 2025, award-era site gone. |
| L'Occitane Seeds of Dreams | Fetch failed (2019 anyway). Likely dead. |
| Dogstudio (8.17) | Responds but stuck on loader in check. |
| Miyagami | Now a broader agency site; archived footer not current. |
| KUBOTA FUTURE CUBE | Discontinued May 2026. |
| kodeimmersive.com | Nuxt 500, broken (creator malvah.co). |
| lab.sardinefish.com/rain | TLS certificate expired 17 Sep 2026. MIT repo github.com/SardineFish/raindrop-fx still useful. |
| kite.venashial.design | 502 from the research environment. Repo https://github.com/venashial/kite-cursor loads. Not proven dead. |
| The Sea We Breathe, https://www.bluemarinefoundation.com/the-sea-we-breathe/ | Awarded (2021 project), but canvas stuck on loader in two checks. Not confirmed working. |
| Cartier W&W 2024 live (cartier-waw-dev-0224.dev.60fps.fr) | Stuck on loader. Use the case study only. |
| Reach the Moon (2015) | Live campaign fetch failed. |
| Cool Club x FWA | Domain parked. |
| endlessletter.com | Maintenance. isolation.is is parked. |
| retrominder.tv | Domain for sale. |
| creative-nights.com | "Coming soon". |
| Sephora Pinball, Cdiscount Jumping Max | Live-broken. |
| ZERO (gesture-locked landing) | No live URL. |
| gpomp.com (502), vfreman.com (parked), pierrenottin.com (fetch failed) | Unreachable. |
| demilie.ru (original) | Dead. |
| aengel.io | Cloudflare Access wall. Leo Parpeix: empty fetch. |
| 10x17.co, matvoyce.com, mubasic custom domain, glsl.io, timbstrails | Hijacked (see 2H). |
| Kasama (closing), deadshot (broken), dash.creative (domain dead) | Dead or dying. |
| Loader stall only (not proved dead) | shoya-kajita.com, hirotos.com, heycusp.com/gallery, patatap. |
| Black or blank render | TRACK (502), ROME restored (black film), Studio Dumbar, Kiln, Feixen, MOUTHWASH (blank in one slice, though mouthwash.studio rendered in another; re-check). |
| Unresolved URLs | Springs (7.36), AIR (7.54), Josephsm.com (did not load), Palmer in the horizontal-scroll slice (not the Dinnerware site). |

Note: palmer-dinnerware.com is live and fetched fine (SOTD + Dev, https://www.awwwards.com/sites/palmer).

---

# PART 4. Original-mechanic opportunities (no awarded precedent = differentiator)

For each: the closest real parts, and what is new. Where the only "exact match" is a NOT REAL page, it is flagged so it is not cited.

| Mechanic | What exists | What is original | Build from |
|---|---|---|---|
| **Kite flight through project chapters** (altitude unlocks content) | No awarded steer + wind + tension + reel site. Yuan's kite is a visual tether only (string length does not limit reach). | Reel payout as navigation; altitude flags as chapters | Yuan https://a-cursor-is-a-kite.yuanzichen.com/ + WebGamePlus https://webgameplus.com/games/kite-flight/ (one-button payout, real, BROWSER, unknown maker) + CargoKite https://cargokite.com/ (SOTD 7.44 [A] https://www.awwwards.com/sites/cargokite) |
| **Conjunction-unlock orrery** | Real orrery demos, none with content triggered by alignment | Projects as planets; alignments reveal glass cards | ProDyn + GravIT + Orrery.live (item 5) |
| **Bonsai: prune, season dial, regrowth** | No awarded prune + wire + regrow. Nature Beyond Technology is presentation only. ZenBonsai https://daankogelmans.itch.io/zenbonsai is patience-growth (old). | Prune-to-reveal; per-visitor tree state | Navas GPGPU wind (Codrops 2025/12/04) + ZenBonsai persistence. Ian Nacke postmortem https://tsai-ian.itch.io/bonsai-simulator/devlog/830612/procjam-2024-postmortem for topology (his pruning and wiring are admitted absent). |
| **Pottery wheel: shape, glaze, fire, shelf** | VaseFX https://killedbyapixel.github.io/VaseFX/ (GPL-3.0, no award, canvas not hand-tested). Keramos https://keramos.vercel.app (all rights reserved: principles only). | Whole shape-glaze-kiln flow as portfolio intro | VaseFX core + Keramos feel + Palmer https://palmer-dinnerware.com gallery |
| **Rock pool: disturb, react, tide hides projects** | Jill Hindenach exhibit https://www.jillhindenach.com/work/rocky-shore-tide-pool (2019 installation, not web) | Tide level gates which project is reachable | Mancini water + water-scene.unseen.co + species-specific reactions |
| **Rain and fog wipe over a project card** | Parts only (item 3) | Merge + wipe + reveal in one | Codrops RainEffect + Canvas UI droplets |
| **Beam / lighthouse reveal** | None real. The only exact match is the NOT REAL PHAROS room (its `beamAngle` + atan2 + CSS-variable maths was read in code). | Cards lit by a sweeping beam | Re-derive the maths yourself. Do not cite PHAROS. |
| **Marble run / ball down the page** | Netlify 5 Million Devs (FWA SOTD + HM Oct 2024), Trunk.io (nominee; GSAP MotionPath, most buildable), clay.com hero | Scroll-bound ball with checkpoint props | Trunk recipe + Rapier ball-pit finale |
| **Dandelion: blow, carry, plant** | Wilde Weide (SOTD Mar 2024), Navas GPGPU | Seeds carry text and images to new sections | Navas wind + sprites + scroll bloom |
| **Cairn: stack stones as projects** | stackrocks.com (best physics HUD), Sai no Kawara (write-up only) | Projects as stones in a queue | stackrocks + progress meta |
| **Breath-to-clear frost** | Igloo (material), Frozen github takuma-hmng8 (R3F), CrazyGL wipe logic | Warm breath clears frost, regrows | Frozen + CrazyGL |
| **Signal decoder: scroll as tuning knob** | jaredwalte.rs (closest, not awarded), Infinite Field (HM Apr 2026) | Static snaps into a headline | jaredwalte.rs + Interference Archive (github zazieproductions, MIT) |
| **Moth to flame / fireflies** | CrazyGL Fireflies component, Medusae (webgpu.com/showcase/medusae) | Lamp as input, physical inward spiral | Medusae physics; firekeeper.cloud fuel model for fire variants |
| **Music-box crank + pinned drum** | quaxio.com/music_box (disclosed Claude-coded experiment, closest), bilal.show (scroll turns drum) | Pin = project | quaxio + Molazone motion polish |
| **Train carriage journey** | iampoonno.com Night-Train Story (one scroll value, hold zones), toeeshnetwork.vercel.app (route map as nav) | Cel-shaded window, frosted glass panels | Daniel John Morris Ghibli shader how-to (Apr 2026) + hold zones |
| **Snow globe per project** | taylormichaelhall.com/games/snowglobe (50 globes, solo hobby), xmas.forged.build (WebGPU, Dec 2025) | One globe per project | taylormichaelhall + forged |
| **Garden: snip to uncover** | edwson.com/project-ma.html (rake); prune only in itch games | Snip reveals content | edwson + bonsai pattern |
| **Honey drip / viscous reveal** | Buzzworthy (2024), Liquid Drip FX Framer component | Wand-reforming text | Liquid Drip FX + SideFX motion docs |
| **Switchboard / patchbay nav** | 42penguins.com/switchboard, corbet.ch/patchbay (link fallback), design.helpmarq.com | Cord drag opens a project | corbet fallback + helpmarq pulse |
| **Tiny workers assemble the layout** | kody-w.github.io ant colony (10k ants), Ants Coffee identity (Sep 26) | Instanced agents carry DOM blocks | instanced agents + GSAP |
| **Chat as front door** | blackbook.dk (nominee Jun 26), judeworks.app/product/unknown-contact | Near-empty category | github goyal-nandini/chatfolio |
| **Zoetrope / optical-toy navigation** | dimsum002.resn.global (Muzli Pick), siena.film (SOTD 7.9) | Spinning disc is the index | danielcwilson.com zoetrope blog |
| **Soundscape map of projects** | soundingfuture.com/build, radio.garden | Spatial audio per project | Three.js + Web Audio PannerNode |
| **User-controlled gravity flip nav** | tiltoootilt.tote.co.jp (nominee 26) | True user-rotated gravity | Matter.js/Rapier + DeviceOrientation |
| **Creature schools on a light ground** | Item 6 references (all dark) | Frosted-glass creatures | GPU boids, 7 nearest neighbours |
| **Shadow as interface** | experiments.withgoogle.com/shadow-art (2019), mingyongcheng.com | Cast shadows as nav | Codrops relighting (Aug 26) |

Weak or empty categories (no strong precedent): chalkboard (only The Blackboard Artist nominee), inventory/loadout, puzzle grid, single-glyph hero (0 verified), zero-budget award sites (0 strict matches), grain and dither, X-ray lens (draggability unverified).

---

# Build order

1. Foundation: item 1 (stage, scroll camera, glass UI, quality tiers). Everything mounts in it.
2. Navigation model: item 2 (curved wall first, diorama later).
3. Signature hero: one of items 3, 4 or 5.
4. Secondary: 6 (creatures) and 7 (one short playable) as sections.
5. Polish: 8, 9, 10, plus footer and contact from 2F.
6. Differentiator: one Part 4 row that matches the hero. Kite, orrery conjunction and pottery fit the glass-and-cream direction best.

# Caveats

- Most slices are text-fetch. Only BROWSER entries had pixels checked. A loading WebGL page is not proof the interaction works.
- Stub slices do not state how each award was verified. Re-check before public citation.
- Licences: VaseFX is GPL-3.0, Keramos is all rights reserved, Codrops RainEffect forbids redistribution as-is, KITESIM is GPL-3.0, Lusion devs object to code copying. Reference the idea, reimplement it.
- Do not copy brand assets, portraits or code from any reference.
