# 📐 Time to Stand Up

## 1. Design Philosophy: "Tug of War"
Visualize posture data not as simple records, but as a game where **"Good Habits (Stand)"** push out **"Bad Habits (Sit)"**.

## 2. Color System (Dark Mode)
- **Background:** `#121212` (Deep Charcoal) - Eye comfort.
- **Stand (Active):** `#00FFC2` (Neon Mint) - Positive, Energetic.
- **Sit (Rest):** `#7050FF` (Deep Lavender) - Static, Sedentary.
- **Warning:** `#FF4B4B` (Alert Red) - Triggered when sitting continuously for **30 minutes**.

## 3. Layout & Components
3-tier vertical structure.

### A. Header (Top) - "Status & Control"
- **Left:** Logo text (e.g., *Posturize*)
- **Right:** `[● REC]` (Flashing) / `[CAM ON/OFF]` Toggle.
- **Feature:** Camera is hidden/blurred by default. Toggle to see self (monitoring feel) to reduce privacy pressure.

### B. Main (Center) - "The Orb"
- **Floating Orb** in the center.
- **Standing:** Mint orb floating/breathing animation.
- **Sitting:** Lavender orb flattened/grounded animation.
- **Role:** Glancable status check.

### C. Footer (Bottom) - "The Balance Gauge" ⭐
- **Shape:** Thick horizontal bar (80% width).
- **Structure:** `Stand (Mint)` on left, `Sit (Lavender)` on right. Areas represent the ratio of total time.
- **Warning Trigger:**
  - If sitting continuously for **>30 minutes**, the Sit bar turns `Red` and glows.
- **Data Display:**
  - Left: `Stand 00:45:10`
  - Right: `Sit 01:20:00`
  - Bottom Center: `Total 02:05:10`

## 4. UX Scenario
1. **Initial State:** Request camera permission. Gray orb waits.
2. **Analysis:** Sitting fills the Lavender bar. Standing fills the Mint bar.
3. **Pre-warning:** As continuous sitting approaches 30 minutes (e.g., at 25m), the bar edges pulse red.
4. **Warning:** At 30 minutes of continuous sitting, the Sit bar turns **Bright Red** and the background dims with a red tint. "MOVE YOUR BODY" appears.
5. **Resolution:** User stands up and stretches. The Mint bar pushes back the Red/Lavender area, "purifying" the gauge and returning to a healthy balance.
