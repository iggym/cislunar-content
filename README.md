# Cislunar Economy (2025–2040+)

Build a single-file, zero-dependency, mobile-first interactive web application in `index.html` to explore the **Cislunar Economy (2025–2040+)**. The application should deploy as a static site on **GitHub Pages**.

## 1. Research and domain content

Synthesize accurate, verifiable data across three interactive catalogs.

### Key players and infrastructure

- **Commercial pioneers** — SpaceX, Blue Origin, Intuitive Machines, Astrobotic, Firefly Aerospace, ispace, Axiom Space, Lunar Outpost, Venturi Astrolab, GITAI, Redwire, and Orbit Fab.
- **Institutional anchors** — NASA Artemis and Commercial Lunar Payload Services (CLPS), ESA Moonlight, JAXA, and CNSA and the International Lunar Research Station (ILRS).

Include vehicle and payload specifications, mission roles, and funding and contract milestones.

### Economic verticals and strategies

- **Cislunar transportation and logistics** — Heavy-lift launch, orbital transfer vehicles (OTVs), cryogenic propellant depots, and lunar landers.
- **In-situ resource utilization (ISRU)** — Lunar regolith mining, water-ice extraction at Shackleton Crater and the lunar south pole, liquid oxygen and liquid hydrogen (LOX/LH₂) propellant production, and lunar sintering and construction.
- **Communications, positioning, navigation, timing, and power** — Lunar relay constellations, LunaNet positioning, navigation, and timing (PNT), fission surface power, and vertical solar array technology (VSAT).
- **Microgravity manufacturing and robotics** — ZBLAN optical fibers, pharmaceuticals, autonomous surface rovers, and robotic assembly.

### Interactive roadmap and timeline (2025–2040)

Show CLPS deliveries, Artemis crewed landings, Lunar Gateway assembly, commercial propellant depot demonstrations, and permanent surface habitats in chronological order.

## 2. Visual and interactive architecture

### Visual design

Use a high-contrast orbital telemetry theme with a Void Black (`#000000`) canvas, frosted-glass panels using `backdrop-filter: blur(12px)`, and subtle orbital gridlines. Use International Orange (`#FF4F00`), Electric Emerald (`#00FF66`), and Slate Cyan (`#00E5FF`) for data accents.

### Interactive orbital canvas

- Use HTML5 Canvas or SVG to animate the Earth–Moon system. Include low Earth orbit (LEO), geostationary orbit (GEO), Earth–Moon Lagrange points L1 and L2, near-rectilinear halo orbit (NRHO), low lunar orbit, and the lunar south pole.
- Show interactive Hohmann and ballistic lunar transfer paths with animated spacecraft telemetry pulses.
- Let users select orbital zones and nodes to filter or highlight related players, economic verticals, and timeline events.

### Photography, renders, and iconography

- Embed high-resolution public-domain NASA and JPL imagery using reliable Wikimedia Commons or NASA Image Library URLs. Examples include lunar south pole illumination maps, Apollo and Artemis hardware, and Lunar Reconnaissance Orbiter renders. Use `onerror` handlers to substitute procedural SVG or Canvas visuals if an image fails to load.
- Use layered SVG lighting gradients, metallic specular filters (`<feSpecularLighting>`), and Canvas particle shaders to render photorealistic lunar landers, orbital propellant depots, and surface rovers. Include custom geometric brand monograms and technical icons.

### Catalog filtering and comparison

Provide instant client-side search and tag filters for vertical, country or agency, technology readiness level (TRL) or readiness, and target orbit. Show matching entries in a comparison matrix and use a slide-over drawer for details.

## 3. Technical and deployment constraints

- **Single file, zero build** — Keep all HTML5, CSS3, and modern JavaScript (ES6+) in `index.html`. Use vanilla web technologies with no React, Vue, Webpack, Node.js, or npm dependencies.
- **GitHub Pages ready** — Use semantic HTML, relative paths for local assets, and an embedded JSON data store. Keep the core experience offline-capable with no backend calls. Remote photography uses the procedural fallback when unavailable.
- **Mobile-first and touch-optimized** — Use fluid typography with `clamp()`, touch-friendly orbital scrubbers and pan and zoom gestures, and bottom-sheet detail drawers on mobile. Use `requestAnimationFrame` for animation and target 60 fps.
