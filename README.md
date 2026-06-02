# 🎨 Letter Lab

**Letter Lab** is a customizable, standalone web game designed to help kids master phonics. Unlike standard educational apps, Letter Lab lets parents and teachers record their **own voices** for every letter and number, ensuring the child learns with familiar sounds and specific regional pronunciations.

---

## ✨ Features

- **🎙️ Personalized Phonics**: Record yourself saying "buh", "duh", "puh", etc. Kids learn faster with a voice they know!
- **🔡 Full Alphabet & Numbers**: Support for all letters (a-z) and numbers (0-9).
- **💾 Persistent Memory**: Your recordings are saved locally in your browser using IndexedDB. Close the tab, come back later, and your sounds are still there.
- **🎯 Focus Mode**: Use the "In Game" checkboxes to pick exactly which characters your child needs to practice.
- **📱 iPad & Mobile Ready**: Optimized for touchscreens with large buttons and no accidental zooming or scrolling.
- **🌓 Dark Mode**: Easy on the eyes for evening practice.
- **🎉 Rewards**: A fun star-explosion animation and a synthesized "Tada!" fanfare for every 10 correct answers.

---

## 🚀 How to Use

1.  **Open the App**: Simply open `index.html` in any modern web browser (Safari, Chrome, etc.).
2.  **Grant Permissions**: Allow microphone access when prompted.
3.  **Setup Sounds**:
    -   Find a letter in the grid.
    -   Click the **Microphone (🎙️)** icon to start recording.
    -   Say the phonic sound clearly.
    -   Click the **Stop (⏹️)** icon to finish.
    -   Use the **Play (▶️)** button to check your work.
4.  **Choose Your Pool**: Check the **"In Game"** box for the letters you want to include in the current session.
5.  **Start the Game**: Click the big **"Start Game"** button in the sticky header.
6.  **Play!**: The app will play a sound, and your child taps the matching character.

---

## 🛠️ Technical Highlights

- **Zero Dependencies**: Pure Vanilla JS, HTML, and CSS. No libraries, no frameworks, no bloat.
- **Web Audio API**: Generates procedural sound effects on-the-fly.
- **IndexedDB**: Professional-grade browser storage for audio Blobs and settings.
- **Dynamic UI**: Uses modern CSS (`clamp`, `dvh`, `flexbox`) for a perfect fit on MacBook, iPad, and iPhone.

---

## 📜 License

This project is open-source and free to use for educational purposes.

---

*Made with ❤️ for the next generation of readers.*
