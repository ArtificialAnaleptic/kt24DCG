# Kill Team 2024 Datacard Editor

This is a single-file HTML application for creating, editing, and managing multiple datacards for Kill Team 2024. It runs entirely in your web browser and saves your work locally.

This tool is based heavily on the work of /u/setounet.

I was given a partial version of this adapted version and attempted to fix it.

HTML is really not my strong point so if this hasn't been updated it's worth checking out /u/setounet's [https://www.kttools.app](https://www.kttools.app) to see if he's improved it instead :)

**THERE IS NO MOBILE VERSION IT WILL NOT WORK WELL ON MOBILE. THERE ARE LIKELY A LOT OF VISUAL AND CLIPPING BUGS I'VE MISSED.**

<img width="800" alt="image" src="https://github.com/user-attachments/assets/dc557432-25b2-4a42-affb-8a9c47624357" />

## Features

* **Deck Management:** Create, edit, and delete multiple datacards in a single session. Sessions are maintained if you leave the page. Save your deck with the export feature and reset if you want to start fresh.
* **Live Editor:** A three-panel layout allows you to select a card from the "Card Manager" (left), edit its properties in the "Editor" (right), and see a live preview in the main central panel.
* **Full Card Customisation:**
    * Edit Unit Name, Title, and Portrait.
    * Adjust main stats (APL, Move, Save, Wounds).
    * Set keywords and base size.
* **Dynamic Editors:**
    * **Weapons:** Add or remove any number of melee or ranged weapons.
    * **Abilities:** Add or remove any number of Passive or Active abilities.
* **Portrait Controls:** Upload a custom image and then pan, zoom, and toggle the fit (`cover`/`contain`) to position it perfectly within the card's portrait slot. Sometimes it loses part of the file when you move/zoom. Just click "fit" to reset this.
* **Automatic Rules:** The tool includes a database of common weapon rules. When you add a rule (e.g., "Lethal 5+", "Piercing 1") to a weapon, its definition is automatically displayed at the bottom of the card (if you have selected the checkbox for this on the given card).
* **Data Persistence:**
    * **Local Storage:** Your entire deck is automatically saved to your browser's local storage as you make changes.
    * **JSON Export:** Export your complete deck to a `.json` file for backup or sharing.
    * **JSON Import:** Import a `.json` deck file to load a saved or shared collection.
    * **Reset:** A "Reset Deck" button clears all data from local storage and starts you with a fresh, blank card.

## How to Use

This is a standalone application. No server or build process is required.

1.  Save the `index.html` file to your computer.
2.  Open the file directly in any modern web browser (e.g., Google Chrome, Firefox, Brave).
3.  The application will load, and you can begin creating your deck.

## Data Management

* **Saving:** All data is saved *automatically* to your browser's `localStorage`. This means your deck is tied to the specific browser you are using.
* **Backing Up:** It is **highly recommended** to use the **"Export Deck (JSON)"** button to create a permanent backup file of your work.
* **Restoring:** Use the **"Import Deck (JSON)"** button to restore your deck from a backup file. This will overwrite any cards currently in your collection.
