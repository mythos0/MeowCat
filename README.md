# 🐱 MeowCat

<p align="center"><b>A procedurally animated desktop cat for Windows 11 — every frame drawn by
code, no sprite sheets, nothing pre-rendered.</b></p>

MeowCat lives *on top of everything* on your screen. There is **zero image art** for the cat:
every whisker, tail wave and ear twitch is computed in real time on a canvas at 60 FPS — so it
can squash, stretch, flip, somersault and change outfit with no animation frames to break.

It treats your **open windows as platforms** — walk near one and it **jumps onto the top
border, strolls along it, then hops to the nearest neighbouring window**. When a **butterfly**
flutters by, the cat hunts it like a real cat: it notices, stalks with a butt-wiggle, creeps
in, then **rears up onto its hind legs and strikes with its front paws** — the butterfly
hovers *above* paw reach and only dips down now and then, so every catch has to be *timed*;
a missed swat makes it **dodge** with a sharp climb-jink while the cat drops to all fours and
chases again. Miss three times and the butterfly escapes; connect once and you earn coins.
And it **dances** — a six-step hind-leg routine: step right → step left → **hands up** →
**turn around** (it shows you its back!) → **shake tail** → a happy squinting **finish**.

| Live on the desktop | Cat Store |
|---|---|
| ![live](docs/screenshots/v32_live.png) | ![store](docs/screenshots/v32_store.png) |

---

## ✨ Features

| | |
|---|---|
| 🎨 **Procedural 2D-canvas cat** | radial-gradient shading, IK legs, chained pendulum tail — 100% code, 0 image frames |
| 🐱 **Three cats, chosen by you** | **Ginger Cat** (the default — the big-headed, short-legged kitten everyone knows), **Grey Tabby**, and the blue-grey plush **Smokey Kitten** to unlock — plus **14 hats** (top hat, crown, bow, pumpkin, santa, flower, shades, witch, party, chef, cowboy, beanie, halo, devil horns) and **6 winter jackets** (puffer, parka, santa coat, knit sweater, powder suit, cardigan) from the Cat Store — every one drawn on the cat in real time, and hats stack with jackets |
| 🦋 **Real butterfly hunts** | butterflies visit every display, hovering **above paw reach** and periodically dipping into it — the cat stalks, **stands on its hind legs and swats**; a missed swat means a sharp **dodge-climb** and a fresh chase, 3 misses = the butterfly escapes, a well-timed connect earns 🪙 + a heart |
| 💃 **Choreographed dance** | a six-step routine danced **on its hind legs**, with **stubby short legs** on a low compact body; the side-steps really **travel across the screen**, the raised paws are the cat's actual front paws (exactly four limbs at all times), and there are zero pose snaps between steps |
| 🐈‍⬛ **Companion kitten** | a second small cat that follows the big cat, leaps up to join it on window tops, wakes when the pair separates, and play-fights |
| 🚶 **Window-top hopping** | any window (any size, resizable) near the cat becomes a walkable platform: jump on, stroll, hop to the next window, drop back down |
| 🖥️ **True multi-monitor** | the cat can be **dragged onto the 2nd monitor** (main streams the real cursor across boundaries) and **walks there by itself** with a single discrete lane hop — no flicker, ever |
| 🚫 **No-walk zones, screenshot-style** | press "Select area on screen" and **drag a rectangle straight off the desktop** (Windows Snipping Tool style, crosshair overlay, Esc cancels); the cat refuses to walk into it, and window tops overlapping it are never used |
| 🔊 **All-sound controls** | a **master toggle** plus separate toggles for single-click meow, double-click meow, random meows, contextual sounds and the reminder chime; **double-click only plays the classic meow** — nothing opens |
| 🤫 **Quiet walking** | footsteps are gone; ambient meows are natural single calls (occasionally a burst) and never overlap a click meow |
| ⏰ **Reminders & Pomodoro** | one-shot / daily / weekly / every-N repeats with bubble + chime; focus/break timer with a celebration dance — both live on the settings homepage |
| 🏆 **Achievements & affection** | pet to build affection, unlock perks (sparkle landings, greeting bows) and achievements |
| 📸 **Photo mode** | Ctrl+Alt+P freezes the pose and saves a transparent PNG |
| 🪶 **Truly low memory** | one small overlay lane, services in-host, **one renderer at rest** — closing Settings immediately frees its process; 6 processes total, ~46MB main |
| 🛡️ **Never quits on its own** | a hard quit gate blocks any non-explicit exit (window loss, crashes, signals, stray quits are reversed and journaled); the cat window is unclosable from every side path and a watchdog re-creates and re-shows it; only **you** can Quit |
| ⌨️ **Hotkeys & privacy** | Ctrl+Alt+C summon/hide, Ctrl+Alt+P photo — all optional toggles; no telemetry ever |

## 🎮 Interactions

| you do | the cat does |
|---|---|
| **single click** | a natural single meow |
| **double-click** | the classic meow — that's it, nothing opens (while music is actually playing the meow politely holds its tongue and mouths a silent ♪ instead) |
| **drag & drop** | rides your cursor anywhere — including across monitor boundaries |
| **right-click** | menu: Settings · Store · Reminders · Dance · Feed · Sleep · Quit |
| **feed it** | a fish appears — it bites, chews and swallows |
| **nothing** | it lives its own life: strolls, naps, grooms, hunts butterflies, makes biscuits |
| **multiple meows in a row** | they **queue and play one after another** — never cutting each other off |

> **v3.18 housekeeping** — the voice feature set ("hey cat" commands, the speech engines and
> the YouTube launcher) is **gone entirely**: it never worked reliably on real machines and it
> cost a background process. The Cat Store is now a **curated boutique** — three cats, hats and
> dresses — and a cat that bumps into a wall now **stops, sniffs and turns around once** like a
> real cat instead of flipping back and forth in place.
>
> **v3.18.1** replaces the v3.18.0 installer, which was uploaded corrupted and could not start
> on some PCs ("version not compatible"). It also keeps the cat inside its roaming lane when
> it chases your cursor or the laser dot to the very screen edge.
>
> **v3.19 — the real ginger cat is home.** v3.18 accidentally swapped the beloved default
> ginger kitten for a different-looking cat wearing the same name. The **real Ginger Cat** —
> the big-headed, short-legged, big-eyed kitten that has been the default since the early
> releases — is back, byte-for-byte, and is the **default cat again**. If your save file was
> switched to the grey tabby by v3.18, the ginger cat **walks home automatically** on first
> launch. The wardrobe also doubled: **7 new hats** (witch, party, chef, cowboy, beanie,
> halo, horns) and **6 new costumes** (sakura, sunshine, rainbow, strawberry, hero suit,
> pirate) — every one of them rendered, mirrored and pixel-diffed across all three cats
> before shipping.
>
> **v3.20 — the Cat Store closes cleanly now.** A major bug could take the whole cat down
> when you closed the Cat Store window; the close path is rebuilt so closing the store only
> ever closes the store, and three independent safety nets (a visibility fallback, a 2-second
> cat watchdog and an all-windows-lost resurrection) make sure the cat **always** comes back.
> At the same time the wardrobe is **hats-only**: all dresses/costumes were removed at your
> request — every one of the 14 hats is still there, still rendered and pixel-verified on all
> three cats.>
>
> **v3.21 — the unkillable cat + winter jackets are back.** The Cat Store close bug that
> survived v3.20 is now fixed **at the root**: the one crash class that could still kill the
> whole app instantly (a compositor crash running *inside* the main process) is gone — GPU
> work runs in its own crash-isolated process again — the cat window itself is now
> **unclosable** from every side path, a 2-second watchdog re-creates *and re-shows* the cat
> no matter what, and a renderer-level close bypass discovered and sealed during development
> (a `window.close()` that destroyed the window without any close event firing) is denied and
> journaled. And at your request, **winter jackets return to the Cat Store**: six procedurally
> drawn coats — puffer, parka, santa coat, knit sweater, powder suit, cardigan — fitted to
> every body type, stackable with every hat, all pixel-verified across the three cats.

## 📥 Install (Windows 11)

1. Download **`MeowCat-3.21.0-portable.exe`** from the [latest release](../../releases/latest).
2. Double-click it — no installer, no runtime, no admin rights. A tray icon appears and the
   cat starts exploring.
3. Quit anytime from the tray menu.

> Fully self-contained (Electron 33 embedded) — nothing else to install. The process is named
> **MeowCat** in Task Manager, not some framework name.

## ❓ FAQ

* **Is anything sent to the internet?** No. MeowCat has no telemetry and no network features at
  all — everything runs locally on your machine.
* **Does it slow my PC down?** It's a single small canvas being redrawn — exactly one renderer at rest and a small
  crash-isolated GPU helper; closing the Settings window frees its process immediately.
* **Where did the other cats go?** v3.18 curates the store: Grey Tabby, Ginger Cat and Smokey
  Kitten — with 14 hats and 6 winter jackets to collect. (Old save files with removed cats roll onto the
  default cat automatically — and since v3.19 the default cat is the **real Ginger Cat**
  again; a save that v3.18 parked on the grey tabby walks back home on first launch.)
* **Why is the cat sometimes on a window?** Windows' top borders are its shelves — it's a
  feature, not a glitch. It will hop down on its own.
* **Why didn't my zone-selection show on the other monitor?** Move the mouse there — the
  crosshair overlay follows your cursor across displays.
* **The cat disappeared / my PC slept** — it revives itself. It cannot quit on its own; only
  the tray menu's Quit (or you) can close it.

## 👨‍💻 Developer

Built by [**mythos0**](https://github.com/mythos0) — the private source repository, the public
issue tracker and future releases all live on GitHub.

## 📄 License

MIT © 2026 mythos0 — see [LICENSE](LICENSE).
