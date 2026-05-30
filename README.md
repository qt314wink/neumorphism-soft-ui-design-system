# Jewelmorphism Design System

**Creator:** Jennipher Troup · [girlwithstarryeyes@outlook.com](mailto:girlwithstarryeyes@outlook.com)

> *Part of the **Morphica** family — a series of design systems that translate physical material properties and natural phenomena into browser-native UI language.*

A UI design language derived from gem-like light refraction, chromatic depth, and physics-based elemental animations. Jewelmorphism takes the soft-shadow logic of neumorphism and pushes it through a prism: every surface refracts, every interaction has mass, every state transition carries the physics of light through crystal.

✅ Available as a **GitHub Template** — use this repo as a starting point for any project in the Morphica family.

---

## Design Principles

**Refraction over reflection.** Neumorphism creates soft shadows that simulate a surface pushing out of its background. Jewelmorphism layers chromatic splitting on top — the highlight doesn't just catch light, it bends it. UI elements have spectral depth.

**Physics-based state transitions.** Hover, focus, active, and disabled states are animated as physical events: elements don't just change color, they respond to simulated forces. A pressed button compresses. A focused input glows from within like a lit gem interior.

**Material coherence.** Every token in the system is derived from a physical property of gemstone or crystal: hardness (weight scale), refractive index (opacity and blur values), cleavage planes (grid and spacing logic), inclusion patterns (texture overlays).

---

## Design Tokens

```css
/* Chromatic depth */
--gem-primary:    #7c3aed;   /* amethyst core */
--gem-refract-1:  #a855f7;   /* violet split */
--gem-refract-2:  #06b6d4;   /* cyan split */
--gem-surface:    rgba(255,255,255,0.08);
--gem-gloss:      rgba(255,255,255,0.18);

/* Shadow system — dual-source like a gem under two lights */
--shadow-light:   -4px -4px 10px rgba(255,255,255,0.12);
--shadow-dark:    4px 4px 16px rgba(0,0,0,0.4);
--shadow-inner:   inset 2px 2px 6px rgba(0,0,0,0.3);

/* Physics timing */
--t-compress:  0.08s cubic-bezier(0.25, 0, 0.5, 1);
--t-release:   0.3s  cubic-bezier(0.34, 1.56, 0.64, 1);
--t-glow:      0.5s  cubic-bezier(0.4, 0, 0.2, 1);
```

---

## Component Architecture

All components are pure HTML/CSS — no JavaScript required for visual states. Interaction physics are layered via CSS custom property updates where needed, and optionally extended with a lightweight JS animation layer.

```
jewelmorphism/
├── tokens/
│   ├── color.css         # Gem palette + refraction splits
│   ├── shadow.css        # Dual-source shadow system
│   ├── motion.css        # Physics timing functions
│   └── space.css         # Crystal cleavage grid
├── components/
│   ├── button/
│   ├── card/
│   ├── input/
│   ├── badge/
│   └── modal/
└── index.html            # Full component showcase
```

---

## Using as a Template

1. Click **"Use this template"** on GitHub
2. Name your repo
3. Import `tokens/` into your project
4. Override the gem tokens to match your material source

To fork into a new Morphica system: change the `--gem-*` variables to a new material vocabulary (stone, glass, ceramic, fabric) and rebuild the shadow system from that material's light behavior.

---

## The Morphica Family

| System | Material Source | Aesthetic |
|---|---|---|
| [ChromaFlora](https://github.com/qt314wink/chromaflora-sitezip) | Bioluminescence, cosmic growth | Procedural glow, living light, bloom |
| **Jewelmorphism** | Gems, crystal, refracted light | Chromatic depth, physics interaction |
| [Woodmorphism](https://github.com/qt314wink/woodmorphism) | Wood grain, organic structure | Warmth, grain flow, structural honesty |

---

girlwithstarryeyes@outlook.com · Philadelphia, PA
