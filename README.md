# OXCE Mods

A collection of mods for [OpenXcom Extended (OXCE)](https://github.com/MeridianOXC/OpenXcom), generated with [oxce-modgen](https://github.com/menottim/oxce-modgen).

## Table of Contents

- [Mods](#mods)
  - [Black Market](#black-market)
  - [Fortress X-COM](#fortress-x-com)
- [Installation](#installation)
- [About](#about)

## Mods

### Black Market

__Type:__ Economy | __Game:__ UFO Defense

Alien weapons, materials, and artifacts available for purchase at steep black market prices. Skip the research grind — if you can afford it.

| Tier | Markup | Examples |
|------|--------|---------|
| Weapons & clips | 5x sell price | Heavy Plasma: 858K, clip: 48K |
| Psi/recon gear | 5x sell price | Psi-Amp: 974K, Mind Probe: 1.5M |
| Strategic materials | 8x sell price | Elerium: 40K/unit, Alloys: 52K/unit |
| UFO components | 8x sell price | Power Source: 2M |
| Research artifacts | 3x sell price | Alien Food: 15K |

A fully kitted Heavy Plasma soldier costs ~1M credits. Early-game monthly funding is ~500K. You __can__ buy alien tech, but it's "mortgage the base" money.

> Folder: [`black-market/`](black-market/)

---

### Fortress X-COM

__Type:__ Base Defense | __Game:__ UFO Defense | __Requires:__ OXCE 7.0+

Base defense overhaul — makes base layout a strategic decision from month 3. Five pillars:

__1. Earlier retaliations:__ Alien retaliations start at month 3 on all difficulties (vanilla: month 10-14). You need defenses early.

__2. Cheaper-but-weaker defenses:__ All defense facilities cost 50% less to build, but hit ratio is reduced by 10 points. You need more of them — layering matters.

__3. Expensive hangars:__ Build cost tripled (200K → 600K), maintenance doubled (25K → 50K). Forces hard choices between interception capacity and base defense.

__4. Defense upgrade tree:__ The Grav Shield (cheapened to 400K, build time halved) unlocks __hardened__ variants of every defense facility:

| Base Defense | Hardened (requires Grav Shield) | Improvement |
|-------------|-------------------------------|-------------|
| Missile (def: 500, hit: 40%) | Hardened Missile (def: 650, hit: 55%) | +30% def, +15% hit |
| Laser (def: 600, hit: 50%) | Hardened Laser (def: 780, hit: 65%) | +30% def, +15% hit |
| Plasma (def: 900, hit: 60%) | Hardened Plasma (def: 1170, hit: 75%) | +30% def, +15% hit |
| Fusion (def: 1200, hit: 70%) | Hardened Fusion (def: 1560, hit: 85%) | +30% def, +15% hit |

__5. Specialized facilities:__ 7 new facilities gated by base infrastructure investment:

| Facility | Tier | Requires | Key Stats |
|----------|------|----------|-----------|
| Training Barracks | Early | — | 10 training slots, 20 personnel |
| Field Hospital | Early | Living Quarters | Faster wound recovery (+1.0 abs, +0.5 rel) |
| Ammunition Depot | Mid | Workshop | 75 storage, costs 5 alien alloys |
| Command Bunker | Mid | Any defense + Mind Shield | +200 passive defense, 1 per base |
| Interrogation Wing | Mid | Containment + Lab | 15 alien capacity, costs 10 alloys |
| Fortress Shield Generator | Late | Grav Shield + hardened defense | +500 defense, draws enemy fire, costs 30 elerium + 50 alloys |
| Psi-Defense Array | Late | Mind Shield + Psi Lab | 200 mind power, costs 15 elerium |

The Grav Shield is the __linchpin__ — in vanilla it's a luxury, here it's the gateway to serious base defense. Combined with the new facility tree, base building becomes a genuine strategic puzzle.

> Folder: [`fortress-xcom/`](fortress-xcom/)

## Installation

1. Download or clone this repo
2. Copy the mod folder (e.g., `black-market/`) into your OpenXcom `mods/` directory
3. Launch the game → Options → Mods
4. Enable the mod and click OK

Mods are safe to enable mid-campaign. They override vanilla values via OXCE's merge system — only changed fields are affected.

## About

These mods are YAML-only ruleset overrides — no custom sprites, sounds, or maps. They're designed to change how the game __feels__ without adding new content. All values are derived from actual vanilla stats fetched from the [OXCE repo](https://github.com/MeridianOXC/OpenXcom).

Generated with [oxce-modgen](https://github.com/menottim/oxce-modgen), a Claude Code skill for generating OXCE mods from natural language.
