# Magisches Leseabenteuer 🦄✨

A simple, distraction-free reading web app designed for 2nd graders to practice German reading.

**Live Demo:** [https://gil-mor.github.io/reading-game/](https://gil-mor.github.io/reading-game/)

## About this Project
This app was "vibe-coded" with **Gemini** by **Gil Mor** and his 8-year-old child. It was built to make reading practice fun, interactive, and personalized.

### Features
- **10-Minute Reading Challenge:** A gentle timer helps track progress without the pressure of "winning" or "losing."
- **Overtime Mode:** If the time runs out, the child can choose to continue reading, and the timer tracks the extra effort with a "bonus" count.
- **Dynamic Story Menu:** Choose between different adventures.
- **Child-Friendly Design:** Pastel colors and simple navigation using Enter or Arrow keys.
- **Customizable Content:** Easily add your own stories and drawings.

---

## Running Locally

Since the app fetches story data dynamically via JSON and text files, it requires a local web server to run (opening the `index.html` file directly in a browser will cause a CORS error).

1. Open your terminal or command prompt.
2. Navigate to the project folder.
3. Run the following command:
   ```bash
   python -m http.server 8000
   ```