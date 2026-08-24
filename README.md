# Chess Vision Trainer

A fun, interactive web-based tool to improve chess coordinate recognition and spatial memory. Quickly identify chess board squares and columns through gamified practice with scoring, timers, and multiplayer leaderboards.

## 🎮 Features

- **Two Game Modes:**
  - **Level 1 (Columns):** Identify specific chess file (column) from a-h
  - **Level 2 (Full Grid):** Identify exact square coordinates (e.g., e4, h7)

- **Three Timer Options:**
  - **Untimed:** Practice at your own pace with no time pressure
  - **30s Blitz:** Quick challenge to test reflexes and accuracy
  - **60s Standard:** Extended session for deeper practice

- **Pro Mode:** Hide board labels for advanced players testing pure spatial memory

- **Multi-Profile System:** Create and switch between player profiles, each with independent score tracking

- **Smart Leaderboards:**
  - Individual high scores per level/mode combination
  - Live competitive feedback ("You just beat X's record!")
  - Personal bests and milestone tracking

- **Visual Feedback:**
  - Color-coded square highlights for correct/incorrect answers
  - Motivational messages and encouragement
  - Score pop animations
  - Timer panic mode (red highlight at 5 seconds)

## 🚀 How to Play

1. **Open `index.html`** in any modern web browser (no installation needed)
2. **Create or Select a Profile** using the modal dialog
3. **Choose Your Difficulty:**
   - Select Level (Columns or Full Grid)
   - Select Timer (Untimed, 30s, or 60s)
   - Toggle Pro Mode for extra challenge
4. **Tap "Start"** to begin
5. **Click the highlighted square/column** shown at the top
6. **Earn points** for correct answers (+10 points) and lose points for mistakes (-5 points)
7. **Beat your high score** and compete with other players!

## 📊 Score System

- ✅ **Correct Answer:** +10 points
- ❌ **Wrong Answer:** -5 points
- Scores are **tracked per player** and **per game mode** combination
- High scores persist across browser sessions via localStorage

## 🎯 Game Modes & Variations

| Level | Description | Difficulty |
|-------|-------------|-----------|
| Columns (L1) | Identify only the file (a-h) | Easy |
| Full Grid (L2) | Identify exact coordinate (a1-h8) | Medium/Hard |
| + Pro Mode | Hide board labels (any level) | +Difficulty |
| + 30s Blitz | Time-based challenge | Speed Focus |
| + 60s Standard | Extended practice session | Endurance Focus |

## 🛠️ Technical Details

- **Technology Stack:** Pure HTML + CSS + Vanilla JavaScript (no dependencies)
- **Storage:** Browser localStorage for profiles and score persistence
- **Responsive Design:** Works on desktop, tablet, and mobile devices
- **Performance:** Single-file architecture (~27KB) for instant loading
- **Accessibility:** Semantic HTML, keyboard navigation support

## 📝 Local Development

No build step required! This is a static single-file application:

```bash
# Simply open in your browser:
open index.html

# Or serve locally with any HTTP server:
python -m http.server 8000
# Then visit http://localhost:8000/index.html
```

## 🎨 Customization

The app uses CSS variables for easy theming. Modify the `:root` variables at the top of `<style>` to change:

- `--light-square` / `--dark-square`: Board square colors
- `--bg-color`: Background
- `--text-color`: Text color
- `--accent-color`: Button and success color
- `--penalty-color`: Error/penalty color

## 💾 Data Storage

All data is stored locally in your browser (localStorage):
- Player profiles: `chess_trainer_profiles`
- Current player: `chess_trainer_current_profile`
- High scores: `chess_user_score_{username}_{level}_{mode}_{timer}`

**Note:** Clearing browser cache will reset all data. Export scores manually if needed.

## ✨ Tips for Success

1. **Start with Columns mode** to learn the files (a-h) from left to right
2. **Practice without timer first** to build muscle memory
3. **Enable Pro Mode** only after mastering the board layout
4. **Use 30s Blitz** to train speed and reflexes
5. **Create player profiles** to track progress against friends

## 🐛 Troubleshooting

**Scores not saving?**
- Check if localStorage is enabled in your browser
- Ensure you're not in private/incognito mode

**Board looks small?**
- This is a responsive app—resize your browser or rotate your device
- Font sizes and square sizes scale with viewport

**Profile data missing?**
- Clearing browser cache will reset all data
- Try refreshing the page or checking if cookies are blocked

## 📦 Browser Compatibility

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile browsers: ✅ Full support (iOS Safari, Chrome Android, etc.)

Requires modern browser with ES6 JavaScript support (2015+).

## 🤝 Contributing

Found a bug or have an idea? Feel free to open an issue or submit a pull request!

## 📄 License

This project is open source. See LICENSE file for details.

---

**Created by Nozel Rosario**

Happy training! ♟️✨
