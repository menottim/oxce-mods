# OXCE Mods

A collection of mods for [OpenXcom Extended (OXCE)](https://github.com/MeridianOXC/OpenXcom), generated with [oxce-modgen](https://github.com/menottim/oxce-modgen).

## Table of Contents

- [Mods](#mods)
  - [Black Market](#black-market)
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

## Installation

1. Download or clone this repo
2. Copy the mod folder (e.g., `black-market/`) into your OpenXcom `mods/` directory
3. Launch the game → Options → Mods
4. Enable the mod and click OK

Mods are safe to enable mid-campaign. They override vanilla values via OXCE's merge system — only changed fields are affected.

## About

These mods are YAML-only ruleset overrides — no custom sprites, sounds, or maps. They're designed to change how the game __feels__ without adding new content. All values are derived from actual vanilla stats fetched from the [OXCE repo](https://github.com/MeridianOXC/OpenXcom).

Generated with [oxce-modgen](https://github.com/menottim/oxce-modgen), a Claude Code skill for generating OXCE mods from natural language.
