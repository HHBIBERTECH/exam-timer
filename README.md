# Exam Timer

A single-file, browser-based classroom exam timer built for exam supervisors. Designed for clarity on classroom projectors and TVs, it features a live 3-hour countdown, secure exam code masking, equipment condition toggles, and a ruler-style progress timeline.

---

## Features

* **Multi-Exam Support (1–3 Concurrent Exams):** Switch between 1, 2, or 3 columns to manage multiple exams running simultaneously in the same room.
* **Secure Exam Code Masking:** Enter 6-digit numeric exam codes during setup without revealing them to students—digits display as dots (`••••••`) before the exam begins (or `n/a` when blank) and automatically reveal once the timer starts.
* **Equipment Condition Toggles:** Dedicated, high-contrast **Headphones** and **Calculator** icons default to prohibited (crossed out in red) and can be clicked to toggle permission per exam.
* **Paper & Digital Exam Modes:** Displays standard desk instructions for paper exams or a three-column NZQA login and backup guide when **Digital Exam** is checked.
* **Automated Toilet & Exit Status Banner:** Automatically switches between **Toilets Closed • Students May Not Leave** (first 45 minutes and final 15 minutes) and **Toilets Open • Students May Leave** (middle 2 hours).
* **Ruler Progress Timeline:** An open-top, color-coded ruler integrated into the countdown panel with 5-, 15-, and 30-minute ticks, **Start**, **1 Hour**, **2 Hours**, and **Finish** milestone badges, and a moving red tracking triangle.
* **Auto-Save & Refresh Protection:** Saves all inputs, icon states, and active timer timestamps to `localStorage`, and warns before closing or refreshing an active exam.

---

## Getting Started

1. Download or save the HTML file (e.g., `index.html`) to your computer.
2. Double-click the file to open it in any modern web browser (Chrome, Edge, Safari, or Firefox)—no internet connection or installation required.

---

## Supervisor User Guide

### 1. Pre-Exam Setup (Before Starting the Clock)
* **Number of Exams:** Select `1`, `2`, or `3` next to **Exams:** in the control bar to match the number of exams in the room.
* **Exam Name:** Click inside each top box (showing `--`) and type the exam title.
* **Exam Code:** Click the **Exam Code** field and type the 6-digit numeric code. Entered digits appear as dots (`••••••`) until the exam begins; leave blank to display `n/a`.
* **Special Exam Instructions & Equipment Icons:**
  * Enter any specific exam rules (e.g., *Open Book*, *Resource Booklet Provided*) in the instruction field.
  * Click the **Headphones** or **Calculator** icons to toggle permission (**Red Slash** = Prohibited [default]; **Unslashed** = Permitted).
* **Paper vs. Digital Instructions:**
  * Leave **Digital Exam** unchecked to display standard paper-exam desk instructions.
  * Check **Digital Exam** to display the three-column NZQA login and backup instructions.
* **Display Controls:** Click **⛶ Full Screen** to fill the classroom screen, or **🔍 100%** (or press `Ctrl + 0` / `Cmd + 0`) to ensure browser zoom is at 100%.

### 2. Running the 3-Hour Exam
* **Starting the Timer:** Click **Start 3 Hour Exam** at the official start time. Setup controls hide automatically, **Exam Codes** reveal in full, and **Start Time** and **Finish Time** (exact 3-hour mark) populate automatically.
* **Ruler Progress Scale:**
  * **Orange Zones (First 45 mins & Final 15 mins):** Toilets closed; students may not leave the room.
  * **Green Zone (Middle 2 hours):** Toilets open; students may leave with supervisor permission.
  * **Red Triangle & Shading:** Tracks exact elapsed time across the ruler in real time.

### 3. Saving, Refreshing & Resetting
* **Accidental Refresh Protection:** If the browser is refreshed mid-exam, the timer, entered text, exam codes, and icon states restore automatically.
* **Resetting:** Click the muted **Reset Exam** button and confirm the prompt to clear the timer and return to the pre-exam setup screen.
