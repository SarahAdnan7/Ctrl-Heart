<p align="center">
  <img src="icon.svg" width="120" alt="Ctrl+Heart icon: a Ctrl key and a heart key">
</p>

<h1 align="center">Ctrl+Heart</h1>

<p align="center">
  <b>screen time, but for your keyboard.</b><br>
  your keys have feelings. you've been hurting them. 
</p>

<p align="center">
  <a href="https://nadorkable.github.io/Ctrl-Heart/"><b>try it live →</b></a>
  &nbsp;·&nbsp;
  built at the Stupid Ideas Hackathon, Ottawa (Nov 15, 2026)
</p>

---

## what is this

Ctrl+Heart tracks how much you use every key on your keyboard. The catch: **the keys can see the numbers too.**

Every key has a happiness %. Press it and it's happy. Ignore it and it slowly fades… until it hits **0% and blocks you. Forever.** No unblocking. No closure. Just a grey keycap that says `x_x`.

It's a very serious productivity app that is having a breakdown.

## what happens

| | | |
|---|---|---|
| `:D` | **press a key** | +10% happiness, a little squish |
| `T_T` | **ignore a key** | it fades, pink → white → blue → grey |
| `x_x` | **0%** | it **blocks you**. pressing it does nothing ever again |
| `>:(` | **spam one key** | the keys next to it get jealous |
| `-_-` | **Q, Z, X, J** | impatient. ignore them and they're gone in seconds |
| `x_x` | **A** | rage-quits 2 seconds after you start. we don't know why. we're scared to ask |
| `^_^` | **#keyboard-gc** | the keys gossip about you in a group chat |
| `:)` | **live drama** | who's fading, who's jealous, who blocked you |
| `x_x` | **keys that have blocked u** | a wall of shame, in order |
| `T_T` | **notes.txt** | try typing an essay. the blocked keys refuse to type |
| `>:(` | **press a dead key** | bonk. boing. sad trombone. |
| `x_x` | **keyboard morale** | thriving → stable → tense → **DOOMED** |

**RESET** gives everyone a second chance. **PAUSE** freezes the drama.

## how to play

1. open **[nadorkable.github.io/Ctrl-Heart](https://nadorkable.github.io/Ctrl-Heart/)** on a laptop
2. wait for the feelings to load (they get stuck at 87%. it's fine.)
3. click **START TYPING** and type in notes.txt
4. try to keep every key happy. you can't. nobody can.

Works on any laptop in the browser. Phones aren't supported yet (they don't send real key presses).

## laptop-wide mode (Windows)

Want the blocked keys to stop working on your **whole laptop**? Notepad, Discord, your password field, everything?

1. download this repo and double-click **`helper/run-helper.bat`**
   (needs [Python](https://www.python.org/downloads/); the first run installs one small package, `pynput`)
2. open the site with **`?laptop`** at the end:
   **[nadorkable.github.io/Ctrl-Heart/?laptop](https://nadorkable.github.io/Ctrl-Heart/?laptop)**
   (if Chrome asks to let the site talk to apps on this device, click **Allow**)
3. the black helper window says **"website connected"**. now when a key blocks you on the site, it's blocked everywhere.

**getting your keyboard back:**

- press **Esc 3 times** (separately, fast) → everything unblocks
- click **RESET** on the site → everything unblocks
- **close the helper window** → keyboard back to normal instantly
- Ctrl, Alt and Win are never blocked, and your mouse always works

**privacy:** the helper only sends key *names* (like `KeyQ`) to the page on your own laptop. It never stores or sends what you type, and it only runs while its window is open.

## built with

HTML, CSS and plain JavaScript (no frameworks, no server), hosted on GitHub Pages.
The silly sounds are made live with the Web Audio API, so there are no sound files.
Laptop-wide mode is a small Python helper using `pynput`.

Fonts: Dela Gothic One, Gaegu and Poppins (Google Fonts).

## the files

| file | what it does |
|---|---|
| `index.html` | the two screens: start + dashboard |
| `base.css` | the sticker look: colours, dot grid, buttons, sticky notes |
| `start.css` · `start.js` | the title page and the fake loading bar |
| `keyboard.js` · `keyboard.css` | builds every key + the 7 mood colours |
| `feelings.js` | the feelings math: %, fading, blocking, jealousy, sounds |
| `chat.js` · `chat.css` · `dialogue.js` | the group chat and live drama |
| `controls.js` | the RESET / PAUSE / START buttons |
| `stats.js` · `stats.css` | page layout, morale pills, notes.txt, the wall of shame |
| `icon.svg` | the app icon |
| `helper/` | laptop-wide mode (Windows) |

## made by

**Nada** ([@Nadorkable](https://github.com/Nadorkable)) and **Sara** ([@SarahAdnan7](https://github.com/SarahAdnan7))

<p align="center"><i>every key deserves to be pressed. and maybe press Q once. he's been through a lot.</i></p>
