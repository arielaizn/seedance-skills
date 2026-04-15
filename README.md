# 🎬 Seedance Skills — Golden Angel Method

> The most advanced prompt engineering system for **Seedance 2.0** — reverse-engineered from the cinematic "Golden Angel" project.

[![Skills](https://img.shields.io/badge/skills-3-blueviolet?style=flat-square)](#skills)
[![Method](https://img.shields.io/badge/method-Golden%20Angel-gold?style=flat-square)](#the-golden-angel-method)
[![Platform](https://img.shields.io/badge/platform-Hermes%20Agent-black?style=flat-square)](https://github.com/hermesagent)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](#license)

---

## What Is This?

This repo contains 3 production-ready `.skill` files for [Hermes Agent](https://github.com/hermesagent) that transform any generic video idea into a **cinematic, multi-clip Seedance 2.0 sequence** — with full visual consistency, controlled camera movement, and a unique anti-heroic tone.

The system was built by deeply analyzing the prompts from **"The Golden Angel"** — a dark tokusatsu cinematic project that achieved unprecedented visual continuity across multiple AI-generated clips.

---

## The Golden Angel Method

Three core principles extracted from the original project:

### 1. 🔒 Visual Style Lock
One spec. Copied **exactly** across every clip. No drift, no variation.
```
Cinematic IMAX look, Panavision C-series, 35mm, f4
Low-saturation grey-blue palette, compressed shadows with texture,
slight edge softness, moderate film grain
```

### 2. 🎥 Camera Handoff
The **end position** of clip N becomes the **start position** of clip N+1.
Plan the entire camera journey before generating a single frame.
```
Clip 1: Start low-angle right → End high-angle left profile
Clip 2: Start high-angle left profile → End stabilized handheld
Clip 3: Start stabilized handheld → End slightly below, unstable
```

### 3. ⚡ Anti-Heroic Constraint
Every moment of power is paired with physical cost. No glowing heroes.
No triumphant poses. Everything is heavy, forced, and real.
```
"yanked upward abruptly, not graceful flight"
"sword moves once — short, direct motion, no flourish"
"enemies still remain — scattered, not defeated"
```

---

## Skills

### 📦 `seedance-prompt-master.skill`
The complete single-prompt building system based on Golden Angel architecture.

**Includes:**
- Full 8-block prompt structure (Core Theme → Character → Visual Style → Camera → 5×3s Sequence → End State → Finish Lock)
- Anti-Heroic constraint table
- Environment-as-reaction principle
- Camera-as-character principle
- Color grade & lens reference tables
- Step-by-step workflow

**Trigger phrases:**
`"write me a prompt"` / `"upgrade my prompt"` / `"Seedance prompt"` / any scene description

---

### 📦 `seedance-15sec-technique.skill`
The multi-clip chaining system for building videos longer than 15 seconds with full continuity.

**Includes:**
- Camera Handoff planning (pre-generation)
- Visual Style Lock (exact copy protocol)
- Finish Block as consistency anchor
- The `Continue the story...` formula
- Common mistakes + fixes table
- Real scenario templates (action, brand film, nature)

**Trigger phrases:**
`"15-second technique"` / `"extend the video"` / `"continuity"` / `"longer video"`

---

### 📦 `golden-angel-template.skill`
A fill-in-the-blank template for building a complete 3-clip cinematic series from scratch.

**Includes:**
- Pre-generation planning table (aesthetic name, camera handoff plan, narrative arc)
- Full template for Clip 1 (transformation / opening)
- Full template for Clip 2 (first pressure / encounter)
- Full template for Clip 3 (escalation / crisis)
- Pre-generation checklist for each clip
- Anti-Heroic Quick Reference card

**Trigger phrases:**
`"Golden Angel template"` / `"plan a series"` / `"3-clip sequence"` / `"cinematic series"`

---

## Installation

### Install a single skill

1. Download the `.skill` file from this repo
2. Send it to your Hermes Agent chat
3. Done — installed instantly ✅

### Install all 3 skills at once

```bash
git clone https://github.com/arielaizn/seedance-skills
```
Then send each `.skill` file to Hermes Agent.

---

## How It Works

`.skill` files are ZIP archives containing a `SKILL.md` file with YAML frontmatter and structured markdown.  
Hermes Agent reads the skill, loads it into context, and uses it to guide every prompt it writes.

```
seedance-prompt-master.skill
└── seedance-prompt-master/
    └── SKILL.md   ← YAML frontmatter + full methodology
```

---

## Example Output

A prompt generated using `seedance-prompt-master` + `golden-angel-template`:

```
Core Theme: Dark realistic tokusatsu, BLACK SUN aesthetic,
damaged flesh transformation, apocalyptic battlefield

Character Setup
Face: Use reference@Image1 exactly, no beautification.
Maintain wounds, bandages, blood. Expression: gloomy —
transformation shows restrained pain only, no heroic energy.
Clothing: Open trench coat, exposed defined upper body
Environment: Smoke-filled wasteland, grey-blue overcast sky,
meteors streaking with fire

Visual Style
Cinematic IMAX look, Panavision C-series, 35mm, f4
Low-saturation grey-blue palette, compressed shadows, film grain
BLACK SUN: fusion of organic flesh and alien tech, heavy realism

Camera Rules
Single continuous take
Start low-angle right side, slow orbit to front, end high-angle left profile
Subtle handheld "breathing" motion throughout

0–3s   Stare — raises head, looks at right hand. Skin cracks, faint eye gleam.
3–6s   Activation — hand clenches. Golden particles, pulse wave. Controlled pain.
6–9s   Tear — six wings erupt. Camera shakes, loses focus, snaps back.
9–12s  Growth — hair shifts platinum gold. Close-up emphasis.
12–15s Completion — sword materializes. Camera finishes orbit to high-angle close-up.

Finish: Cinematic realism, Dolby Vision, 4K 60fps, no glow, dark blockbuster tone
```

---

## Compatibility

| Platform | Status |
|----------|--------|
| Hermes Agent | ✅ Native `.skill` support |
| Seedance 2.0 | ✅ Optimized for |
| Kie.ai | ✅ Works via Hermes seedance-video-studio skill |

---

## Credits

- **Prompt architecture:** Reverse-engineered from "The Golden Angel" project
- **15-second technique:** Originally discovered by Daniel Biton
- **Skill packaging:** [PixMind Studio](https://arielaizenshtat.com)

---

## License

MIT — use freely, credit appreciated.
