# Chess Vision Trainer

A fun, interactive web-based tool to improve chess coordinate recognition and spatial memory. Quickly identify chess board squares and columns through gamified practice with scoring, timers, and multiple difficulty levels.

🎮 **Play Now:** https://nozelrosario.github.io/chessvisiontrainer/

## 🎮 Features

- **Three Game Levels & Upfront Level Selection:**
  - **Level 1 (Columns):** ♖ Identify specific chess files (columns) from a–h
  - **Level 2 (Full Grid):** ♘ Locate exact square coordinates (e.g., e4, h7) across all 64 squares
  - **Level 3 (Attack Detection):** ⚔️ Detect tactical threats & pieces under attack in realistic legal chess positions

- **Fancy Upfront Level Selector:**
  - Elegant chess-themed popup with large icons and clear difficulty descriptions
  - Appears upfront when starting/selecting profile and accessible anytime via the **Level** button in the controls

- **Three Timer Options:**
  - **Untimed:** Practice at your own pace with no time pressure
  - **30s Blitz:** Quick challenge to test reflexes and accuracy
  - **60s Standard:** Extended session for deeper practice

- **Pro Mode:** Hide board labels for advanced players testing pure spatial memory

- **Multi-Profile System:** Create and switch between player profiles, each with independent score tracking

- **Interactive Stats & Global Leaderboard Popup:**
  - Click the **High Score** card anytime to open a comprehensive progress and rankings popup
  - **Level Mastery Tab:** Detailed breakdown of your personal bests vs global record holders across all levels, Standard vs PRO mode, and Blitz/Standard timers
  - **Player Rankings Tab:** Hall of Fame leaderboard ranking all profiles by total score and 👑 records held
  - Overview banner displaying total score, crown count, and competitive rank (🥇 Champion, 🥈 Runner-Up, etc.)

- **Visual Feedback:**
  - Color-coded square highlights for correct/incorrect answers
  - Motivational messages and encouragement
  - Score pop animations
  - Timer panic mode (red highlight at 5 seconds)

## 🚀 Getting Started

### Step 1: Launch the Game
Simply open `index.html` in any modern web browser. No installation, no server setup needed!

```bash
# Option A: Direct file open
open index.html

# Option B: Local server (optional)
python -m http.server 8000
# Then visit http://localhost:8000/index.html
```

### Step 2: Create Your Profile
When you first launch the game, a profile selection modal appears:
- **Select from saved profiles** using the dropdown
- **Or create a new profile** by entering a name (up to 12 characters)
- Click **"Save & Play"** to continue

### Step 3: Choose Your Level Upfront
A fancy chess-themed Level Selection popup appears:
- **Level 1: Columns (Files a–h)** — Master vertical files with ease
- **Level 2: Full Grid (a1–h8)** — Test precision across 64 squares
- **Level 3: Attack Detection** — Spot threats and high-value captures
- Tap any level card to immediately set your level and load into the game!

### Step 4: Configure Game Settings (Optional)
Customize your game settings in the top bar:

| Setting | Options | Effect |
|---------|---------|--------|
| **Level** | Columns / Full Grid / Attack Detection | Tap the Level button anytime to switch levels via the fancy popup |
| **Side** | White / Black | Play as White or Black perspective |
| **Timer** | Untimed / 30s / 60s | No timer for practice, or speed challenges |
| **Style** | Classic Vector / Outline / Minimal / High Contrast | Choose your piece visual theme |
| **Mode** | Standard / PRO | PRO hides board labels for pure memory |

### Step 5: Click "Start" and Play!

## 📚 How to Play - Detailed Guide

### Game Flow

1. **You'll see a prompt at the top** showing what to find:
   - In **Columns mode**: "Column: D" — find and click any square in that column
   - In **Full Grid mode**: "Square: E4" — find and click that exact square

2. **Click the correct square** on the board
   - The board is labeled with files (a-h, left to right) and ranks (1-8, bottom to top)
   - Use these labels to locate the correct square

3. **Get instant feedback:**
   - ✅ **Correct:** Square flashes green, you earn **+10 points**, next question appears immediately
   - ❌ **Wrong:** Square flashes red, you lose **-5 points**, same question repeats
   - Encouraging messages appear after each answer

4. **Beat your high score** by getting as many consecutive correct answers as possible

### Example Gameplay

**Scenario 1: Columns Mode**
```
Prompt shown: "Column: F"
Your task: Click any square in the F file (6th column from left)
Result: ✅ Click F5 → +10 points → Next question
        ❌ Click G3 → -5 points → "Find column F again"
```

**Scenario 2: Full Grid Mode**
```
Prompt shown: "Square: H7"
Your task: Click the exact intersection of H file and 7 rank
Result: ✅ Click H7 → +10 points → Next question
        ❌ Click H6 → -5 points → "Try again"
```

**Scenario 3: Pro Mode (Full Grid)**
```
All board labels are hidden!
Prompt: "Square: C3"
You must rely on pure spatial memory to locate it
The board gets tricky without the helpful a-h and 1-8 labels
```

## 📊 Scoring Explained

### Point System
- **+10 points** for every correct answer
- **-5 points** for every wrong answer
- Score never goes below 0
- Scores reset for each new game

### High Score Tracking
- Each player has **independent scores** for every mode combination:
  - Columns + Untimed
  - Columns + 30s Blitz
  - Columns + 60s Standard
  - Full Grid + Untimed
  - Full Grid + 30s Blitz
  - Full Grid + 60s Standard
  - + Pro Mode variants (12 total combinations!)
  
- High score displays **best player's name** if you haven't beaten it yet
- Shows **"You"** if it's your personal record

### Example Score Scenarios
```
Your session:
- Q1: Correct → Score: 10
- Q2: Correct → Score: 20
- Q3: Wrong → Score: 15
- Q4: Correct → Score: 25
- Timer ends → Final Score: 25
- This becomes your high score if it beats your previous best!
```

## 🎯 Game Modes & Difficulty Levels

| Mode | Level | Timer | Difficulty | Best For |
|------|-------|-------|-----------|----------|
| **Columns** | 1 | Untimed | ⭐ Easy | Learning the files (a-h) |
| **Columns** | 1 | 30s Blitz | ⭐⭐ Medium | Speed training |
| **Columns + Pro** | 1 | Untimed | ⭐⭐ Medium | Memory without labels |
| **Full Grid** | 2 | Untimed | ⭐⭐ Medium | Learning coordinates |
| **Full Grid** | 2 | 30s Blitz | ⭐⭐⭐ Hard | Speed & accuracy |
| **Full Grid + Pro** | 2 | 60s Standard | ⭐⭐⭐ Hard | Advanced memory training |
| **Attack Detection** | 3 | Untimed / Blitz | ⚔️ Tactical Master | Spotting threats, captures & high-value targets |

### Recommended Learning Path
```
Start here ↓
Columns + Untimed (master a-h files)
         ↓
Columns + 30s Blitz (speed the files up)
         ↓
Columns + Pro + Untimed (memorize without labels)
         ↓
Full Grid + Untimed (learn exact squares)
         ↓
Full Grid + 30s Blitz (speed test full board)
         ↓
Attack Detection (master tactical vision & threat calculation!)
```

## 🎮 UI Elements Explained

### Control Panel (Top Section)
- **Level Button:** Opens the fancy Level Selection popup with rich icons & mode summaries
- **Side dropdown:** Choose White or Black board perspective
- **Timer dropdown:** Choose Untimed, 30s Blitz, or 60s Standard
- **Style dropdown:** Choose Classic Vector, Sharp Outline, Crisp Minimal, or High Contrast
- **PRO checkbox:** Toggle coordinate labels on/off
- **Start button:** Begin a new training session

### Score Board (Three Cards)
- **Left card:** Player name (or countdown timer if timer mode active)
  - "Switch" button: Change to a different player profile
- **Middle card:** Current game score (updates in real-time)
- **Right card:** High score for this mode (shows owner's name)

### Game Display
- **Yellow text (top):** Current prompt ("Column: A", "Square: E4", etc.)
- **White text:** Feedback message (encouragement or correction)
- **Chessboard:** 8x8 grid with labeled coordinates
  - Light squares: #eeeed2 (cream)
  - Dark squares: #769656 (olive green)
  - Click squares to answer

### Feedback Messages
- ✅ **Correct:** "Excellent vision!", "Spot on!", "Genius!", "Magnus would be proud!", "Speedy calculations! ⚡"
- ❌ **Wrong:** "Oops, that was [square] (-5)", then shows which square you clicked
- 🔥 **Competitive:** "You just beat Sarah's record!", "Tied with Alex!", "Just 5 pts away!"
- 👑 **Victory:** "Top of the leaderboard with 120!"

## ⏱️ Timer Modes

### Untimed Mode
- No pressure, unlimited time
- Perfect for learning and building confidence
- Score accumulates as long as you play

### 30s Blitz
- Fast-paced challenge
- Tests reflexes and quick recognition
- Great for speed training

### 60s Standard
- Extended session
- Allows more questions (typically 6-12 depending on speed)
- Good for endurance and consistency

**Timer Mechanics:**
- Counter shows remaining time in top-left (Time card)
- At 5 seconds remaining: **PANIC MODE** activates
  - Timer text turns red and pulses
  - Get ready—game ends at 0s!
- When time runs out: Game automatically ends, score is saved

## 💡 Strategy & Tips

### For Beginners (Columns Mode)
1. Learn the **file order left-to-right:** a, b, c, d, e, f, g, h
2. Start **untimed** to focus on accuracy, not speed
3. Repeat games to build muscle memory
4. Once comfortable, try **30s Blitz** to add pressure

### For Intermediate Players (Full Grid Mode)
1. Understand **rank system:** 1 (bottom) to 8 (top)
2. Practice combining **files + ranks** (e.g., e4 = e file + 4 rank)
3. Use landmarks: center squares (d4, e4, d5, e5) as reference points
4. Try **Untimed** first, then gradually add time pressure

### For Advanced Players (Pro Mode)
1. **Remove visual crutches** by enabling Pro Mode
2. Visualize the board **in your mind's eye** without labels
3. Use **60s Standard** to test endurance
4. Compete on leaderboards against other players
5. Track your **personal bests** across all modes

### General Tips
- **Take breaks** to maintain focus and accuracy
- **Play daily** for best results—consistency beats talent!
- **Challenge friends** by creating separate profiles and comparing scores
- **Don't memorize randomly**—think about coordinate patterns
- **Celebrate milestones**—each high score is progress!

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

**Can't see labels on the board?**
- Check if Pro Mode is enabled (toggle it off to see labels)
- Refresh the page

**Wrong answer deducting too many points?**
- Each wrong answer costs -5 points (minimum score is 0)
- This is intentional to encourage accuracy over guessing

## 📦 Browser Compatibility

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile browsers: ✅ Full support (iOS Safari, Chrome Android, etc.)

Requires modern browser with ES6 JavaScript support (2015+).

## 🤝 Contributing

Found a bug or have an idea? Feel free to open an issue or submit a pull request!

---

## 🔄 Development Workflow

This project uses a **dual-branch deployment strategy** to ensure production stability while enabling safe development:

### 📊 Branch Structure

| Branch | Purpose | URL | Deployment |
|--------|---------|-----|------------|
| **main** | Production | 🟢 https://nozelrosario.github.io/chessvisiontrainer/ | Automatic (GitHub Actions) |
| **develop** | UAT/Testing | 🔵 https://nozelrosario.github.io/chessvisiontrainer/develop/ | Automatic (GitHub Actions) |

### 🔁 Development Workflow

1. **Create a feature branch** from `develop`
   ```bash
   git checkout develop
   git pull origin develop
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** and test locally
   ```bash
   python -m http.server 8000
   # Test at http://localhost:8000/index.html
   ```

3. **Push to your feature branch**
   ```bash
   git push origin feature/your-feature-name
   ```

4. **Create a Pull Request** from your feature branch → `develop`
   - Describe the changes and why they were made
   - Link any related issues

5. **Test on UAT** at https://nozelrosario.github.io/chessvisiontrainer/develop/
   - Once the PR is merged to `develop`, changes deploy automatically
   - Test thoroughly to ensure everything works

6. **Create a PR** from `develop` → `main` (production)
   - This requires at least 1 approval
   - Automated checks must pass
   - Direct commits to `main` are blocked

7. **Merge to main** and deploy to production
   - Once merged, changes go live at https://nozelrosario.github.io/chessvisiontrainer/
   - Deployment is automatic via GitHub Actions

### ✅ Guidelines

- **Always work on feature branches**, never commit directly to `develop` or `main`
- **Test changes on the develop UAT URL** before merging to production
- **Use descriptive commit messages** and PR titles
- **Keep PRs focused** on a single feature or fix
- **Review code carefully** before approving PRs
- **Production (`main`) should always be stable** and deployable

### 🚀 Deployment

Deployments are **fully automated** via GitHub Actions workflow (`.github/workflows/deploy.yml`):

- **Push to `main`** → Automatic deployment to production URL
- **Push to `develop`** → Automatic deployment to UAT URL
- Each branch deploys independently to its respective URL
- No manual deployment steps required!

---

## 📄 License

This project is open source. See LICENSE file for details.

---

**Created by Nozel Rosario**

Happy training! ♟️✨
