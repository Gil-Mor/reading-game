# Magical Reading Adventure / Magisches Leseabenteuer 🦄✨

A simple, distraction-free reading web app designed for helping kids to practice reading.

**Live Demo:** [https://gil-mor.github.io/reading-game/](https://gil-mor.github.io/reading-game/)

## About this Project
This app was "vibe-coded" by me and my daughter. It was built to make reading practice fun, interactive, and personalized.

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

---

## Adding or Replacing Stories

You can easily expand the library with your own adventures:

1.  **Prepare the folder:** Create a new folder inside the `stories/` directory. Use a simple name without spaces (e.g., `der-kleine-drache`). This will be your **Story ID**.
2.  **Write the story:** Inside your new folder, create a file named `story.txt`.
    *   Write your story text here.
    *   Use **two empty lines** (a double line break) to separate pages.
3.  **Add illustrations (Optional):** Inside your story folder, create another folder named `drawings/`. Add up to 5 images named `1.png`, `2.png`, `3.png`, `4.png`, and `5.png`.
4.  **Register the story:** Open `stories.json` in the root directory and add an entry for your new story:
    ```json
    {
      "id": "der-kleine-drache",
      "title": "Der kleine Drache lernt fliegen"
    }
    ```
    *   The `id` must match your folder name exactly.
    *   The `title` is what will appear on the main menu button.

5.  **Refresh:** Reload the website to see your new story in the list!