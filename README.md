# 🐱 MeowCat

<p align="center"><b>A procedurally animated desktop cat for Windows 11 — every frame drawn by
code, no sprite sheets, nothing pre-rendered.</b></p>

MeowCat lives *on top of everything* on your screen. There is **zero image art** for the cat:
every whisker, tail wave and ear twitch is computed in real time on a canvas at 60 FPS — so it
can squash, stretch, flip, somersault and change breed with no animation frames to break.

It strolls your taskbar and treats your **open windows as platforms** — walk near one and it
**jumps onto the top border, strolls along it, then hops to the nearest neighbouring window**
(any window size, resized windows included). It now **really eats**: a fish appears on the
ground, the cat bites chunk after chunk off it, chews side-to-side with working cheeks, and
swallows. Pick the **Panda** and it behaves like a real bear — researched panda anatomy and
behavior: it **waddles** with a heavy rolling gait, **sits up to hook and gnaw a bamboo
stalk** with both paws, **somersaults** across the ground, and naps sprawled flat.

| Live on the desktop | Premium Cat Store — 20 breeds |
|---|---|
| ![live](docs/screenshots/v32_live.png) | ![store](docs/screenshots/v32_store.png) |

| Mochi Kitten (new) | Panda & bamboo |
|---|---|
| ![mochi](docs/screenshots/v32_mochi.png) | ![panda](docs/screenshots/v31_panda.png) |

---

## ✨ Features

| | |
|---|---|
| 🎨 **Procedural 2D-canvas cat** | 8 body types, 20 breeds, radial-gradient shading, IK legs, chained pendulum tail — 100% code, 0 image frames |
| 🐱 **20 breeds** | Grey/Orange Tabby, Siamese, Calico, Persian, Tuxedo, Bombay, Russian Blue, Ginger Kitten, Ragdoll, Bengal, Maine Coon, **Panda**, and v3.2's new designs: **Mochi Kitten** (fluffy orange-white chibi with huge slate-blue eyes — matched to the community reference photo), **Scottish Fold** (folded ears + blush), **Snow Angora** (all-white with odd blue/green eyes), **Somali** (russet brush tail), **British Plush**, **Choco Munchkin** (sausage cat on stub legs), **Sakura** |
| 🤸 **20 actions** | walk, run, sit, sleep, dance, scratch, jump, stretch, groom, pounce, knead, loaf, yawn, startle · **real eating** (fish biting + chewing, v3.2) + panda-only waddle, bamboo munch, somersault roll |
| 🐼 **A panda that's not a cat** | bear barrel body, stub tail, dark muzzle + slanted eye patches, low round ears, heavy waddle, sits up to eat bamboo with both paws, travels with its somersaults, naps sprawled — all behavior researched from real giant pandas |
| 💗 **11 emotes** | hearts, music note, question, exclaim, sweat, anger mark, laugh, star, Zzz, fish — pop in **snugly above the cat's head** (v3.2 anchor fix), context-aware |
| 🐟 **Real eating (v3.2)** | the fish lies on the ground, shrinks with every bite, the tail fin goes first; side-to-side chewing with a bulging cheek and blissful closed eyes; three bites + a gulp |
| 🚶 **Window-top hopping** | any window (any size) near the cat becomes a walkable platform: jump on, stroll, hop to the next window, drop back down |
| ⏰ **Reminders & timers** | one-shot / daily / weekly / every-N repeats — the cat announces yours with a movement, a speech bubble and a chirp |
| 🛒 **Cat Store** | premium dark storefront with live previews; **unlimited-coins promo — every breed unlocks free** |
| ⚡ **Instant settings** | double-click the cat → Settings opens in milliseconds (warm window pool) |
| 🪶 **Low memory (v3.2)** | lean process model: no GPU process, one helper window, services in-host — roughly **5 processes** in Task Manager instead of 7 |
| 🔊 **Real sounds** | three recorded meows, purr, chirp, footsteps, scratch foley — drag & drop is quiet on purpose |
| 🚫 **Always visible** | topmost enforcement keeps the cat above fullscreen apps and games |
| 🧸 **About & credits** | version info and the developer's GitHub, one click away |

## 🎮 Interactions

| you do | the cat does |
|---|---|
| **double-click** it | opens the Settings popup instantly |
| single click | purrs, shows love, earns you coins |
| drag & drop | rides your cursor; lands on the nearest window border or the ground |
| right-click | menu: Settings · Reminders · Dance · Feed · Sleep · Quit |
| feed it (menu) | a fish appears — it bites, chews and swallows (the panda gets bamboo) |
| nothing | it lives its own life: strolls, naps, grooms, pounces, makes biscuits |

## 📥 Install (Windows 11)

1. Download **`MeowCat-3.2.0-portable.exe`** from the [latest release](../../releases/latest).
2. Double-click it — no installer, no runtime, no admin rights. A tray icon appears and the
   cat starts exploring.
3. Quit anytime from the tray menu.

> Fully self-contained (Electron 33 embedded) — nothing else to install. The process is named
> **MeowCat** in Task Manager, not some framework name.

## ❓ FAQ

* **Is anything sent to the internet?** No. MeowCat has no telemetry and no network features.
* **Does it slow my PC down?** It's a single small canvas being redrawn — and v3.2 trimmed the
  process count and RAM use hard (no GPU process, one helper window).
* **Why is the cat sometimes on a window?** Windows' top borders are its shelves — it's a
  feature, not a glitch. It will hop down on its own.
* **Why doesn't the cat wander to random screen spots anymore?** v3.2 removed open-field
  roaming on community feedback — it now strolls along the ground like a real desktop cat.
* **How do I get the Panda / Mochi Kitten?** Double-click the cat → Cat Store. Everything is
  free during the unlimited-coins promo.

## 👨‍💻 Developer

Built by [**mythos0**](https://github.com/mythos0) — the private source repository, the public
issue tracker and future releases all live on GitHub.

## 📄 License

MIT © 2026 mythos0 — see [LICENSE](LICENSE).
