# Hangman Game (Persian) 🎮

A classic Hangman game fully localized in Persian, built with **Pygame**.  
Test your vocabulary by guessing Persian words across various categories—fruits, animals, cities, and objects. The game features an interactive on-screen keyboard, visual hangman stages, background music, sound effects, and a sleek glass‑morphism UI.

![Hangman Screenshot](hangman.png)  
*(Add a screenshot of the game to your repository for a better preview)*

---

## ✨ Features

- **Persian Language Support** – Full right‑to‑left (RTL) text rendering using `arabic_reshaper` and `python‑bidi`.
- **Category Selection** – Choose from four categories:  
  🍎 Fruits, 🐆 Animals, 🏙 Cities, 🪑 Objects.
- **Interactive Keyboard** – Click on Persian alphabet buttons to guess letters.
- **Hint System** – After 3 wrong guesses, a “Hint” button appears to help you.
- **Visual Hangman** – Progressively displays hangman stages (0–6 mistakes).
- **Dynamic Backgrounds** – Each category has its own themed background image.
- **Sound Effects & Music** – Menu and game background music, plus click, correct, wrong, win, and lose sounds.
- **Particle Effects** – Decorative particles in menus and victory screen.
- **Glass‑morphism UI** – Modern semi‑transparent panels and keyboard buttons with blur effects.

---

## 📦 Requirements

Make sure you have **Python 3.7+** installed.  
The game uses the following libraries:

- `pygame`
- `arabic_reshaper`
- `python‑bidi`

You also need **Persian font** (Vazirmatn) and asset files (images, sounds) – see [Assets](#assets) below.

---

## 🚀 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/hangman-persian.git
   cd hangman-persian
   ```

2. **Create and activate a virtual environment** (recommended)
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install pygame arabic_reshaper python-bidi
   ```

4. **Place the required assets**  
   The game expects the following folder structure (create them if missing):

   ```
   assets/
   ├── images/
   │   ├── hangman_0.png ... hangman_6.png   (7 images for hangman stages)
   │   ├── background_fruits.png
   │   ├── background_animals.png
   │   ├── background_cities.png
   │   └── background_objects.png
   ├── sounds/
   │   ├── click.wav
   │   ├── correct.wav
   │   ├── wrong.wav
   │   ├── win.wav
   │   ├── lose.wav
   │   ├── music_menu.ogg
   │   └── music_game.ogg
   └── Vazirmatn-Regular.ttf   (Persian font file, placed in the root of assets or alongside the script)
   ```

   > **Note:** The font file `Vazirmatn-Regular.ttf` is expected to be in the same directory as the script, not inside `assets/`.  
   > You can download it from [Vazirmatn GitHub](https://github.com/rastikerdar/vazirmatn).

5. **Run the game**
   ```bash
   python hangman.py
   ```

---

## 🎮 How to Play

1. **Main Menu** – Click “شروع بازی” (Start Game) to begin.
2. **Category Selection** – Pick a category.
3. **Game Screen** –  
   - A word is hidden; guess letters by clicking on the Persian keyboard.  
   - Each correct guess reveals the letter in the word.  
   - Each wrong guess advances the hangman drawing and increases your mistake count.  
   - After 3 mistakes, a “راهنما” (Hint) button appears – click it to see a hint for the word.  
4. **Win / Lose** – If you guess all letters, you win! Otherwise, after 6 mistakes, you lose.  
   - The final screen shows the correct word and offers a “بازی مجدد” (Play Again) button.

---

## 🗂 Project Structure

```
hangman-persian/
├── hangman.py              # Main game script
├── README.md               # This file
├── assets/                 # (not included in repo – see above)
│   ├── images/
│   ├── sounds/
│   └── Vazirmatn-Regular.ttf
├── requirements.txt        # (optional) list of dependencies
└── .gitignore
```

---

## 🛠 Customisation

You can easily modify the game:

- **Add new categories** – Edit the `WORDS_DATA` dictionary in `hangman.py`.
- **Change visuals** – Replace the background images or hangman stage images.
- **Adjust difficulty** – Change `max_mistakes` (currently 6) in the `game_loop` function.

---

## 🧩 Dependencies & Credits

- **Pygame** – [pygame.org](https://www.pygame.org/)
- **Arabic Reshaper** – [python-arabic-reshaper](https://github.com/mpcabd/python-arabic-reshaper)
- **Python Bidi** – [python-bidi](https://github.com/MeirKriheli/python-bidi)
- **Vazirmatn Font** – [Vazirmatn](https://github.com/rastikerdar/vazirmatn) (Open Font License)

---

## 🤝 Contributing

Contributions, bug reports, and feature requests are welcome!  
Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is open‑source and available under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## 📧 Contact

For any questions, feel free to reach out via [GitHub Issues](https://github.com/yourusername/hangman-persian/issues).

---

Enjoy the game!  
