# Hostile Planets – Game Design Document

<p align="center">
  <img src="../../images/icons/doc.svg" alt="Game Design Document" width="40" />
</p>

<p align="center">
  <strong>A fast-paced twin-stick arcade survival shooter</strong><br/>
  <em>World Domination Software LLC — Game Design Document (Pre-Production Review)</em>
</p>

<p align="center">
  ← <a href="./README.md">Back to README</a> &nbsp;|&nbsp; <a href="./Overview.md">Overview</a> &nbsp;|&nbsp; <a href="./Gameplay.md">Gameplay</a>
</p>

---

> **📋 Document Purpose**
>
> This document is a **pre-production design review** for *Hostile Planets*, intended for players, community members, and contributors. It exists to gather feedback and gauge interest before full development begins. This is not a development specification — it is a vision document focused entirely on **gameplay, design, and player experience**.
>
> We'd love to hear what excites you. Join the conversation in [Hostile Planets Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/hostile-planets-general).

---

## 📖 Table of Contents

- [Game Overview](#-game-overview)
- [Core Gameplay Loop](#-core-gameplay-loop)
- [Player Objective](#-player-objective)
- [Map Structure](#️-map-structure)
- [Enemy Behavior](#-enemy-behavior)
- [Fuel Risk System](#-fuel-risk-system)
- [Special Items and Artifacts](#-special-items-and-artifacts)
- [Powerups](#-powerups)
- [Planet Modifiers](#-planet-modifiers)
- [Scoring System](#-scoring-system)
- [Visual Style](#-visual-style)
- [Replayability](#-replayability)
- [Future Expansion Ideas](#-future-expansion-ideas)

---

## 🚀 Game Overview

**Hostile Planets** is a fast-paced **twin-stick arcade survival shooter** inspired by classic arena games like *Robotron 2084*. Players pilot a lone spacecraft to dangerous alien worlds, racing to collect fuel resources while fighting off waves of increasingly ferocious alien creatures.

Each planet is a deadly arena. Every run is a desperate race between greed and survival.

| | |
|---|---|
| **Genre** | Twin-Stick Arcade Survival Shooter |
| **Platform** | Mobile (primary target) |
| **Perspective** | Top-down arena |
| **Inspiration** | Robotron 2084, classic arcade survival games |
| **Core Fantasy** | Lone hero versus impossible alien odds |

The game is designed around short, intense sessions — perfect for mobile play. A single planet run should take **two to five minutes**, making every decision matter.

---

## 🔄 Core Gameplay Loop

Each session in Hostile Planets follows a clear, satisfying loop that keeps escalating tension from the first second to the last:

```
🛸 Land on Planet
       ↓
🗺️  Explore the Arena
       ↓
⛽ Collect Fuel Scattered Across the Map
       ↓
👾 Survive Alien Swarms
       ↓
⚖️  Risk vs Reward: More Fuel or Return Now?
       ↓
🚀 Return to Ship — Deposit Fuel
       ↓
🌍 Unlock Next Planet
       ↓
🔁 Repeat with Increasing Difficulty
```

> **Design Intent:** The core loop is intentionally simple — land, collect, survive, escape. The tension comes from the risk-reward decision of how long to stay before the aliens overwhelm you.

---

## 🎯 Player Objective

The primary objective on every planet is the same:

> **Collect enough fuel to power your ship and escape the planet alive.**

But it's never that simple. Here's what players must juggle every run:

- ⛽ **Fuel scattered across the map** must be physically returned to the ship to count.
- 💀 **Dying before depositing** means all carried fuel is lost — start the planet over or try again.
- ⚖️ **Balancing risk and survival** is the core skill — knowing *when* to push further and when to run.
- 🌊 **Alien swarms grow** — the longer you stay on a planet, the more dangerous it becomes.

There is no hand-holding. The planet does not care if you make it out.

---

## 🗺️ Map Structure

Each level represents a **different alien planet**, rendered as a small, self-contained arena map designed for fast arcade play.

### 🛸 Map Landmarks

| Location | Description |
|---|---|
| **Player Ship (Center)** | Spawn point and fuel deposit zone. Always in the center of the map. |
| **Fuel Deposits** | Scattered across the arena in clusters and isolated spots. |
| **Enemy Spawn Points** | Enemies spawn from the edges and designated spawn zones. |
| **Artifact Locations** | Rare item spawn points, randomized each run. |

### 🌍 Planet Types

Each planet features a unique **terrain style**, **visual theme**, and **environmental modifiers** that make every world feel distinct:

| 🌿 Planet | Theme |
|---|---|
| **Alien Jungle** | Dense alien flora, bioluminescent ground cover, toxic spores |
| **Ice Planet** | Frozen tundra, crystalline structures, blizzard visibility effects |
| **Volcanic Planet** | Rivers of lava, ash clouds, crumbling terrain |
| **Crystal Caverns** | Underground cave system, glowing crystal formations |
| **Desert Ruins** | Ancient alien structures, sandstorms, open terrain |
| **Abandoned Colony** | Derelict human outpost, dark corridors, unknown horrors |

> **Design Goal:** Planets are primarily visual and thematic variations on the same core arena. The gameplay loop stays consistent — only the aesthetics, enemies, and modifiers change to keep runs fresh.

---

## 👾 Enemy Behavior

Alien creatures are the primary threat. They spawn around the edges of the map and aggressively pursue the player. As planets progress, enemies become faster, smarter, and more relentless.

### 🧬 Enemy Types

| Enemy | Behavior |
|---|---|
| 🐛 **Swarm Creatures** | Slow individually, dangerous in numbers. Appear in large groups on early planets. |
| 🐆 **Fast Hunters** | Speed-focused predators that close distance quickly. Appear on mid-tier planets. |
| 🛡️ **Armored Enemies** | Require sustained fire to destroy. Slow but relentless. |
| 💥 **Exploding Aliens** | Rush the player and detonate on contact. Clear them early — or use them against each other. |
| ⭐ **Elite Monsters** | Rare, powerful creatures with unique attack patterns. High risk, high reward to defeat. |

### 📈 Difficulty Scaling

```
Planet 1–3   ░░░░░░░░░░  Slow swarmers, learning the map
Planet 4–6   ████░░░░░░  Faster enemies, early hunters introduced
Planet 7–9   ███████░░░  Mixed types, armored units appear
Planet 10+   ██████████  Full chaos — elites, explosives, speed rush
```

Enemy spawn rates increase the longer a player lingers on a planet. **Staying too long is always punished.**

---

## ⛽ Fuel Risk System

The fuel mechanic is the **beating heart of Hostile Planets**. It transforms simple collection into a high-stakes decision loop.

### How It Works

1. 🔍 Fuel canisters are scattered across the arena.
2. 🤲 Players pick up fuel by moving over it — it is stored in a limited carry capacity.
3. 🚀 Fuel only counts toward progression once deposited at the ship.
4. 💀 **If the player is defeated before returning to the ship, all carried fuel is lost.**

### The Risk vs Reward Decision

```
┌─────────────────────────────────────────────────┐
│  LOW RISK PATH                HIGH RISK PATH    │
│                                                 │
│  Deposit often           Hold more fuel         │
│  Stay near ship          Explore further        │
│  Lose little if killed   Lose more if killed    │
│  Slower progression      Faster progression     │
└─────────────────────────────────────────────────┘
```

> **Design Intent:** This system ensures every second on the planet is a calculated gamble. Players who play conservatively survive but progress slowly. Players who push their luck can clear planets faster — or lose everything.

---

## 💎 Special Items and Artifacts

Rare **alien artifacts** occasionally spawn on the map. These are high-value, high-risk pickups — often located far from the ship, in dangerous territory.

### 🏺 Artifact Types

| Artifact | Effect |
|---|---|
| 🏺 **Ancient Alien Relic** | Massive score multiplier bonus |
| 💎 **Energy Crystal** | Grants a temporary offensive ability boost |
| ⚠️ **Unstable Power Core** | Detonates all enemies in a wide radius — but it's dangerous to carry |

### What Artifacts Provide

- 🏆 **Large score bonuses** — ideal for leaderboard competition
- ⚡ **Temporary abilities** — shift the tide of battle for a short window
- 💣 **Enemy clearing effects** — can save a player in a desperate situation

> Artifacts function similarly to bonus items in classic arcade games — tempting, valuable, and always dangerous to pursue.

---

## ⚡ Powerups

Temporary **powerups** appear randomly across the arena and give players a short-lived edge against alien swarms. They disappear if not collected quickly.

### 🔋 Powerup Types

| Powerup | Effect |
|---|---|
| 🔫 **Rapid Fire** | Dramatically increases firing rate for a short duration |
| 🌀 **Spread Shot** | Fire spreads into a wide arc — great against swarms |
| 🛡️ **Temporary Shield** | Absorb one hit without losing carried fuel |
| 💨 **Speed Boost** | Short burst of movement speed — for escaping or repositioning |
| 💥 **Area Shockwave** | Clears all nearby enemies in an instant explosion |

> Powerups are **survival tools**, not game-breakers. They help a skilled player turn a desperate situation around — but they won't save someone who isn't paying attention.

---

## 🌐 Planet Modifiers

Each planet may include an **environmental modifier** that adds a unique twist to the familiar gameplay loop. Modifiers stack with enemy difficulty to make each planet feel distinct.

### 🔧 Modifier Examples

| Modifier | Effect |
|---|---|
| 🪐 **Low Gravity** | Movement feels floaty — harder to stop and harder to dodge |
| ☠️ **Toxic Atmosphere** | Slow HP drain while not inside the ship's safe zone |
| 🌫️ **Reduced Visibility** | Fog obscures the outer edges of the map |
| ⚡ **Enemy Speed Increase** | All aliens on this planet move significantly faster |
| ☄️ **Meteor Showers** | Random meteor strikes create hazard zones on the map |

> **Design Goal:** Modifiers are **spice, not overhaul**. They adjust strategy without changing the core gameplay loop. A veteran player should still feel capable — just challenged.

---

## 🏆 Scoring System

Points are earned throughout each run. The scoring system is designed to reward skill, aggression, and risk-taking.

### 🎯 How Points Are Earned

| Action | Points |
|---|---|
| ☠️ Defeating an enemy | Per kill, scales with enemy type |
| ⛽ Collecting and depositing fuel | Bonus for efficient fuel runs |
| 💎 Collecting artifacts | High flat bonus |
| ⏱️ Surviving longer | Time-based survival bonus |
| 🌍 Planet completion | Completion bonus scales with difficulty |

### 📊 Score Tracking

```
  Per Planet     ────►  High score table per planet
  Per Run        ────►  Total score across all planets in one session
  Leaderboard    ────►  Global comparison with other players
```

> High scores encourage **replayability** — players who master a planet's enemy patterns and modifier interactions will always have room to improve their score.

---

## 🎨 Visual Style

*Hostile Planets* uses a **low-poly stylized art direction** that prioritizes clarity and visual excitement over realism.

### Design Pillars

| Pillar | Description |
|---|---|
| 🎯 **Readability First** | Enemy silhouettes are always distinct and clearly readable at a glance |
| 🌈 **Bright, Vivid Colors** | Each planet uses a strong color palette to create immediate atmosphere |
| 🕹️ **Arcade Energy** | Visual effects — explosions, pickups, score popups — are punchy and satisfying |
| 🪐 **Alien Character** | Environments feel genuinely alien, not just re-skinned Earth settings |

### Visual References

- **Alien Jungle** → Deep greens and glowing purples, bioluminescent ground lighting
- **Ice Planet** → Cold whites and blues, sharp crystalline geometry
- **Volcanic Planet** → Deep reds and oranges, glowing lava channels
- **Crystal Caverns** → Multi-spectrum crystal refractions, underground darkness broken by vivid color
- **Desert Ruins** → Warm ochres and sandy browns, ancient glyphs, dust particle effects
- **Abandoned Colony** → Grey industrial tones with flickering emergency lighting

> The goal is that each planet should be **immediately recognizable** in a screenshot and feel meaningfully different to explore.

---

## 🔁 Replayability

*Hostile Planets* is designed to be played many times. Every run should feel **familiar but never identical**.

### What Changes Each Run

| Element | Variation |
|---|---|
| 👾 **Enemy Spawns** | Randomized spawn timing and positions each run |
| 💎 **Artifact Locations** | Randomly placed on each planet load |
| ⚡ **Powerup Timing** | Powerups appear at randomized intervals and locations |
| 🌐 **Planet Modifiers** | Applied per planet, creating different challenge profiles |

### What Drives Players Back

- 🏆 **High Score Competition** — always a reason to run one more time
- 📈 **Skill Growth** — learning enemy patterns rewards repeated play
- 🌍 **Planet Variety** — distinct environments keep the game feeling fresh
- ⚡ **Short Sessions** — each planet run is short enough to always fit in one more

---

## 🔭 Future Expansion Ideas

The following are **potential directions** for expanding *Hostile Planets* after the core experience is established. These are ideas, not commitments.

| Idea | Description |
|---|---|
| 🌍 **Additional Planets** | More alien worlds with unique environments and enemy sets |
| 👽 **New Alien Enemy Types** | Expand the enemy roster with new behaviors and attack patterns |
| 🏯 **Boss Encounters** | Rare mega-bosses that appear between planet runs as endurance challenges |
| 🛸 **New Player Ships** | Different ship classes with varied carry capacity, speed, and weapon loadouts |
| 👥 **Multiplayer Survival** | Co-op survival modes where players coordinate fuel collection and enemy defense |

> Have a feature idea or want to vote on what gets built next? Join the discussion at [Hostile Planets Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/hostile-planets-general).

---

## 📣 Share Your Feedback

This document exists to **start a conversation**. We want to know:

- 🎮 Does the core risk-vs-reward fuel mechanic sound fun to you?
- 🌍 Which planet types are you most excited to explore?
- 👾 What enemy types sound the most interesting to fight?
- ⚡ Are there powerups or mechanics you'd love to see added?

Drop your thoughts in the [Hostile Planets Discussions](https://github.com/World-Domination-Software/Projects/discussions/categories/hostile-planets-general) — your feedback directly shapes what gets built.

---

<p align="center">
  <img src="../../images/icons/support.svg" alt="Discussions" width="28" />
  &nbsp;
  <img src="../../images/icons/roadmap.svg" alt="Roadmap" width="28" />
  &nbsp;
  <img src="../../images/icons/bug.svg" alt="Bug Reports" width="28" />
</p>

**→ [README](./README.md) · [Overview](./Overview.md) · [Gameplay](./Gameplay.md) · [Getting Started](./Getting-Started.md) · [Implementation Notes](./Implementation-Notes.md)**
