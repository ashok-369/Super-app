# Super App — Production-Ready Portal

A highly polished, responsive, and pixel-perfect unified dashboard and entertainment discovery application built using **React 19**, **Vite**, **TypeScript**, **Zustand**, and **Tailwind CSS v4**.

---

## 🚀 Key Features

### 1. Registration Screen
- **Full Validation Rules**: Includes real-time inputs validation (Name: $\ge 3$ characters, Username: no spaces, Email: valid syntax, Mobile Number: exactly 10 digits).
- **Consent Checks**: Enforces terms and registration sharing consent.
- **Save State**: Automatically registers user profiles and proceeds to category selection.

### 2. Category Selection Screen
- **Selective Genre Cards**: Modern 3x3 category grid containing individual representations (Action, Drama, Romance, Thriller, Horror, Western, Fantasy, Music, Fiction) with smooth scaling on hover and select indicators.
- **Constraint Enforcement**: Requires at least 3 categories selected before proceeding. Otherwise, showing custom warnings.
- **Active Pills**: Active category pills with close 'X' buttons displaying counts.

### 3. Bento Dashboard Grid
- **User Profile Widget**: Custom generated avatar based on username, displaying credentials and selected category tags.
- **Real-Time Weather Widget**: Dynamic, real-time weather details fetched from the open-source, key-unrestricted *Open-Meteo API*, detailing temp, condition, wind, humidity, pressure, and auto-clock metrics.
- **Personalized Notes Widget**: Clean notebook with active debounced auto-saving capabilities, synchronized with localStorage and showing live "Saved at [Time]" indicators.
- **Interactive Countdown Timer**: Numerical setter wheels for hours, minutes, and seconds. Rendered inside a circular SVG countdown ring indicating accurate progress ratio, and synthesizes a dual-tone synthetic bell chime (built using Web Audio API) when the clock reaches zero.
- **News Feed Slider**: Pulls entertainmentheadlines from *saurav.tech*. Automatically slides articles every 2 seconds with fade-in/fade-out animations and pause-on-hover triggers.

### 4. Entertainment Discovery Catalog
- **Netflix-Style recommendations**: Categorizes collections by selected interests.
- **Flexible Data sources**: Attempts live search querying using OMDB API if a key is provided, while falling back to a comprehensive, high-quality curated movie collection if offline or key is empty.
- **Details Modal Overlay**: Immersive overlays displaying release year, runtime, starring cast, ratings progress, and plot summaries.

---

## 🛠️ Technical Stack & Architecture

- **Framework**: React 19 + Vite + TypeScript (Native Esbuild compilation)
- **Styling**: Tailwind CSS v4 (Modern performance, customized keyframe transitions, and custom thin scrollbars)
- **State Management**: Zustand 5 (Persistent sync with `localStorage` for profile details, notes, and genres)
- **Icons**: Lucide React
- **Sound Synth**: Web Audio API (No physical mp3 asset requirement)

---

## ⚙️ Running Locally

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Start the development server**:
   ```bash
   npm run dev
   ```

3. **Production build**:
   ```bash
   npm run build
   ```

4. **Lint & Typecheck**:
   ```bash
   npm run lint
   ```
