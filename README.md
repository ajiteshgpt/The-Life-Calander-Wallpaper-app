# ⏳ Life Calendar (For Android): Existential Crisis in 4K

## all versions here 👇
## 📥 [https://github.com/ajiteshgpt/The-Life-Calander-Wallpaper-app/releases]

# 🚨 READ THIS BEFORE YOU INSTALL! 🚨

## ⚠️ WARNING: YOU MIGHT SEE A SCARY POPUP ⚠️

When you try to install this app, your phone (specifically Google Play Protect) might act like it’s seen a ghost. It looks exactly like this:

![Google Play Protect Warning](https://github.com/ajiteshgpt/The-Life-Calander-app-/blob/main/DO%20NOT%20OPEN%20!!!!/WhatsApp%20Image%202026-01-14%20at%206.57.19%20AM.jpeg)

*^ If you see this image, don't panic!*

### 😱 WHY IS THIS HAPPENING?!
Relax! Take a deep breath. 🧘‍♂️

The message says: **"Play Protect hasn't seen this app before."**

This **does not** mean the app is a virus, a secret government spy tool, or trying to steal your collection of cat memes.

It simply means:
1.  This app is **not on the Google Play Store** (yet).
2.  Because it's a side-loaded app (APK), Google is just being an overprotective parent saying, *"I don't know this stranger!"*

### 🛠️ WHAT SHOULD I DO?
Don't let the robot overlords boss you around.

1.  When the popup appears, click **"More details"**.
2.  Select **"Install anyway"**.
3.  Enjoy the app!

---

### 🕵️‍♂️ "NO SPY" GUARANTEE
I promise there is **NO spyware**, **NO malware**, and **NO funny business** hidden inside.

I barely have enough time to code this app, let alone figure out how to hack the Pentagon through your phone. The only thing this app wants to steal is your... attention (and maybe some of your boredom).

**Happy using!** 🚀







--
> **"Visualize Time. Live Intentionally."**

**Visualize your life journey, annual progress, or personal goals through elegant, minimalist wallpaper grids. Life Calendar automatically transforms your device’s Home and Lock screens into a high-tech dashboard of time.**

Why look at a picture of your cat when you can stare at a pixel-perfect grid of how many weeks you have left before you become a memory? 

---
## 🍎 The Inspiration (And The "Why")

**Heavily inspired by the genius concept of [The Life Calendar](https://www.thelifecalendar.com/).**

Let's be real: On iOS, setting this up is easy. You just run a **Shortcut**, set a trigger, and boom—instant anxiety.

**But on Android?** It’s a total headache. You usually have to download a wallpaper engine, find a specific preset, tweak the settings, sacrifice a goat to the KWGT gods, and write three lines of JSON just to see a dot.

**I did the work so you don't have to.**
As a student, I didn't want to waste time configuring widgets or messing with automation scripts every morning. I built a single, native Android app to do it all for me. No shortcuts, no "pro version" needed to change the color. Just install, open, and let the existential dread wash over you.

---

## 🍎 The Android Evolution

**The definitive Life Calendar experience, built natively for Android.**

The **Life Calendar** philosophy—visualizing your life in weeks—is a famous stoic concept found on the web and iOS shortcuts. However, Android users have been stuck with messy widgets, complex wallpaper engines, or paid apps that drain battery.

**I solved that.**
This isn't just a widget; it's a seamless implementation of the Life Calendar aesthetic. I built a native Android engine that renders your timeline directly onto the wallpaper layer. No shortcuts, no configuration headaches, just a clean, automated interface that syncs with your life.

---

## 🚀 The Three Modes of Reality

### 1. 🧬 The Life Calendar (Existential Mode)
Visualizes your entire lifespan in a 52-column grid (one for every week of the year).

* **The Vibe:** Watching your HP bar deplete in a high-stakes RPG where there are no respawns.
* **Data Points:** Shows total weeks passed and your age in `Years : Months : Days`.
* **Tech Flex:** Automatically calculates expectancy based on an 80-year projection (adjustable if you plan on living forever).

<p align="center">
  <img src="https://github.com/ajiteshgpt/The-Life-Calander-app-/blob/main/DO%20NOT%20OPEN%20!!!!/3.jpeg?raw=true" height="500" alt="Life Calendar Mode">
</p>

### 2. 📅 The Year Calendar (Speedrun Mode)
A 365-dot grid tracking the current year.

* **The Vibe:** Realizing that January was 3 years ago and tomorrow is already December.
* **Customization:** Toggle between "Year Completed" (for the optimist) or "Year Left" (for the realist).

<p align="center">
  <img src="https://github.com/ajiteshgpt/The-Life-Calander-app-/blob/main/DO%20NOT%20OPEN%20!!!!/1.jpeg?raw=true" height="500" alt="Year Mode">
</p>

### 3. 🎯 The Goal Calendar (Productivity Mode)
A custom-dated grid for specific deadlines (Marathons, Placements, Exams, or that "Neural Networks" course you keep putting off).

* **The Vibe:** The digital equivalent of your mom standing behind you with a stopwatch.
* **Smart Logic:** Automatically defaults to today’s date but respects your right to manually change it.

<p align="center">
  <img src="https://github.com/ajiteshgpt/The-Life-Calander-app-/blob/main/DO%20NOT%20OPEN%20!!!!/2.jpeg?raw=true" height="500" alt="Goal Mode">
</p>

---

## 🛠 Under the Hood (How I Built It)

I’m a CSE student (mostly dealing with AI/ML tensors), so naturally, I over-engineered this. I switched from training models to "vibe coding" Android views, letting my neural nets (and a few LLMs) handle the boilerplate while I focused on the logic:

### 🔋 Battery Optimization (The pOLED Advantage)
I run this on my own phone, so battery life was priority #1.
* **True Black (#000000):** I utilized **Physical Pixel Shutdown**. On devices like the Moto Edge 40 (or any OLED), black pixels literally turn off. The background consumes **0% battery**.
* **Memory Management:** I implemented strict bitmap recycling. Once the wallpaper is drawn, the app calls `recycle()` immediately to free up RAM. No bloat, no lag.

### ⏱ Precision Scheduling (Solving the Android Doze Issue)
Android loves to put apps to sleep to save power, which makes updating a wallpaper at exactly midnight tricky.
* **The Logic:** `PeriodicWorkRequest` is too inaccurate (it has a 15-minute flex window).
* **The Fix:** I used **Chained One-Time Requests** with millisecond calculations to ensure the update hits exactly at 12:00:01 AM.
* **WakeLocks:** I implemented a `PARTIAL_WAKE_LOCK` for exactly 3 seconds during the update process so the CPU doesn't kill the drawing task halfway through.

### 📐 Curved Screen Optimization
* **The 60dp Buffer:** I noticed dots getting cut off on curved displays (like my Moto Edge). I added dynamic horizontal padding so the grid stays perfectly centered and visible, regardless of the screen curvature.

---

## 👨‍💻 Connect with the Creator

**Ajitesh Gupta**
[LinkedIn](https://www.linkedin.com/in/ajiteshgpt/) | [GitHub](https://github.com/ajiteshgpt)

**Feel free to drop a suggestion!**
If you have a feature idea, open an issue. If you find a bug... well, it's a feature. (Just kidding, tell me about it).
*Note: Feature requests like "Stop time" or "Add 5 extra years to my life" will be marked as `wont-fix`.*

**Disclaimer:** Using this app may result in increased productivity, sudden realizations about the passing of time, and a very cool-looking home screen.

> *"Time is a flat circle. We just made it a grid of dots."* 🔘🔘🔘🔘🟠🔘🔘🔘
