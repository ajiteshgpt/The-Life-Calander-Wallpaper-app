# The-Life-Calander-app-
(For Android )Visualize your life journey, annual progress, or personal goals through elegant, minimalist wallpaper grids. Life Calendar automatically transforms your device’s Home and Lock screens into a high-tech dashboard of time.


# ⏳ Life Calendar: Existential Crisis in 4K

> **"Visualize Time. Live Intentionally."**

Welcome to **Life Calendar**, the only app that replaces your cheerful vacation photos with the cold, hard reality of your fleeting existence—now optimized for your curved screen.

Why look at a picture of your cat when you can stare at a pixel-perfect grid of how many weeks you have left before you become a memory? *Memento Mori*, but make it Material 3.

---

## 🍎 The Inspiration (And The "Why")

**Heavily inspired by the genius concept of "The Life Calendar".**

Let's be real: On iOS, setting this up is easy. You just run a **Shortcut**, set a trigger, and boom—instant anxiety.

**But on Android?** It’s a total headache. You usually have to download a wallpaper engine, find a specific preset, tweak the settings, sacrifice a goat to the KWGT gods, and write three lines of JSON just to see a dot.

**I did the work so you don't have to.**
As a student, I didn't want to waste time configuring widgets or messing with automation scripts every morning. I built a single, native Android app to do it all for me. No shortcuts, no "pro version" needed to change the color. Just install, open, and let the existential dread wash over you.

---

## 🚀 The Three Modes of Reality

### 1. 🧬 The Life Calendar (Existential Mode)
Visualizes your entire lifespan in a 52-column grid (one for every week of the year).

* **The Vibe:** Watching your HP bar deplete in a high-stakes RPG where there are no respawns.
* **Data Points:** Shows total weeks passed and your age in `Years : Months : Days`.
* **Tech Flex:** Automatically calculates expectancy based on an 80-year projection (adjustable if you plan on living forever).

![Life Calendar Mode](WhatsApp%20Image%202026-01-14%20at%205.01.04%20AM.jpeg)

### 2. 📅 The Year Calendar (Speedrun Mode)
A 365-dot grid tracking the current year.

* **The Vibe:** Realizing that January was 3 years ago and tomorrow is already December.
* **Customization:** Toggle between "Year Completed" (for the optimist) or "Year Left" (for the realist).

![Year Calendar Mode](WhatsApp%20Image%202026-01-14%20at%205.01.03%20AM%20(1).jpeg)

### 3. 🎯 The Goal Calendar (Productivity Mode)
A custom-dated grid for specific deadlines (Marathons, Placements, Exams, or that "Neural Networks" course you keep putting off).

* **The Vibe:** The digital equivalent of your mom standing behind you with a stopwatch.
* **Smart Logic:** Automatically defaults to today’s date but respects your right to manually change it.

![Goal Calendar Mode](WhatsApp%20Image%202026-01-14%20at%205.01.03%20AM.jpeg)

---

## 🛠 Under the Hood (How I Built It)

I’m a CSE student, so naturally, I over-engineered this to be as efficient as possible. Here is the logic behind the code:

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
[LinkedIn](#) | [GitHub](#)

**Disclaimer:** Using this app may result in increased productivity, sudden realizations about the passing of time, and a very cool-looking home screen.

> *"Time is a flat circle. We just made it a grid of dots."* 🔘🔘🔘🔘🟠🔘🔘🔘
