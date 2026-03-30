# 🧮 Universal Calculator Hub

A **Progressive Web App** with 120+ calculators across 18 categories. Works fully offline after first load. Installable on any device.

## Live Demo

> Deploy to GitHub Pages, Netlify, or Vercel — see [Deployment](#deployment) below.

## Features

- 120+ calculators across 18 categories
- Academic, Finance, Shopping, Fuel, Health, CS/Binary, Science, Sound, and more
- Full offline support via Service Worker
- Installable as a native-like app (PWA)
- Dark / Light theme toggle
- Favorites & History (localStorage)
- Deep-link support (`?view=finance`)
- Keyboard support on the calculator
- Mobile responsive

## Categories

| Category | Calculators |
|---|---|
| 🎓 Academic | CGPA, Attendance, SPI/CPI, Grade Target, Exam Countdown, Study Time |
| 💰 Finance | EMI, Compound Interest, Income Tax, Profit/Loss, SIP, Salary |
| 🛒 Shopping | Discount, GST, Multi-Discount, Cashback, Price Drop, Unit Price |
| 🚗 Fuel & Travel | Fuel Cost, Round Trip, Cost/km, Petrol vs EV, Trip Budget |
| ❤️ Health | BMI, TDEE/Calories, Water Intake, Ideal Weight, Heart Rate |
| 💾 CS & Binary | 1's/2's/9's/10's Complement, Base Converter, IEEE 754, Data Types |
| ⚗️ Science | Force, KE, Ohm's Law, Molarity, pH, Half-Life, Ideal Gas, Dilution |
| 🔊 Sound | Frequency/Wavelength, Decibel, Music Notes, Doppler Effect |
| 🔄 Converters | Length, Weight, Temperature, Speed, Area, Liquid, Pressure, Energy |
| + 9 more | Math, Tech, Daily Life, Productivity, House & Area, Date & Time, Equations, Alphabet, Global |

## Getting Started

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/universal-calculator-hub.git
cd universal-calculator-hub

# Run locally (requires Node.js)
npm start
# Opens at http://localhost:3000
```

Or just open `index.html` directly in a browser — no build step needed.

## Deployment

### GitHub Pages

1. Push to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your app is live at `https://YOUR_USERNAME.github.io/universal-calculator-hub`

### Netlify (drag & drop)

1. Go to [netlify.com](https://netlify.com)
2. Drag the `calc-hub-app` folder onto the deploy area
3. Done — live in seconds

### Vercel

```bash
npx vercel
```

## Icons

The `icons/` folder needs `icon-192.png` and `icon-512.png` for the PWA install prompt.  
Open `generate-icons.html` in a browser to generate and download them, then place in `icons/`.

## Project Structure

```
calc-hub-app/
├── index.html          # Main app shell
├── app.js              # All calculator logic (120+ calculators)
├── style.css           # All styles
├── manifest.json       # PWA manifest
├── sw.js               # Service worker (offline support)
├── package.json        # npm scripts
├── icons/
│   ├── icon.svg
│   ├── icon-192.png    # Generate via generate-icons.html
│   └── icon-512.png
└── generate-icons.html # Icon generator tool
```

## License

MIT
