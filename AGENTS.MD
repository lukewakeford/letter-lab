# Plan: Letter Lab - Phonics Identification Game

Build a single-file, vanilla HTML/JS web game to help kids identify characters through custom-recorded phonic sounds.

## Objective
Create a flexible, standalone phonics platform where parents/teachers record sounds for any letter (a-z) or number (0-9), and kids match those sounds in a fun, reward-driven game.

## Key Features (Implemented)
- **Full Character Support**: Complete grid for a-z and 0-9.
- **Persistent Storage**: Uses `IndexedDB` to save audio recordings and game settings (enabled characters) across browser reloads.
- **Click-to-Record UI**: Intuitive click-to-start/stop recording with visual pulse feedback.
- **Selective Gameplay**: "In Game" toggles for each character, allowing parents to focus on specific problem areas.
- **Game Mode UX**:
    - Interaction locking to prevent sound overlapping/mashing.
    - Visual-first feedback (✅ and ❌ icons) with color-coded buttons.
    - Full-screen, viewport-fit layout (100dvh) to prevent scrolling/zooming.
- **Rewards**: Screen-filling star animation accompanied by a synthesized Web Audio API fanfare.
- **Cross-Platform Polish**: 
    - Fully responsive for MacBook, iPad, and mobile.
    - **Dark Mode** support.
    - Safari mobile compatibility with automatic MIME type fallbacks.

## Technical Implementation
- **Audio Capture**: `MediaRecorder` API with a persistent stream during setup to reduce permission prompts.
- **Audio Playback**: Sequential playback handling to ensure only one phonic sound plays at a time.
- **State Management**: JavaScript `Set` for enabled characters and an object map for Blob URLs.
- **Styling**: Vanilla CSS with modern features like `clamp()`, `@supports`, and `prefers-color-scheme`.
- **Interactions**: `touch-action: manipulation` to eliminate 300ms tap delays and accidental zooms.

## Verification & Testing
- Tested IndexedDB persistence across page refreshes.
- Verified Safari mobile audio recording and playback.
- Confirmed responsive layout on various aspect ratios (iPhone to MacBook).
- Validated Dark Mode contrast and visibility.
