# 🧮 Universal Calculator Hub

A **Progressive Web App** with **96 calculators** across **18 categories**. Works fully offline after first load. Installable on any device.

## 🎯 Live Demo

> Deploy to GitHub Pages, Netlify, or Vercel — see [STARTUP_GUIDE.md](STARTUP_GUIDE.md)

## ✨ Features

- **96 calculators** across 18 categories
- Academic, Finance, Shopping, Fuel, Health, CS/Binary, Science, Sound, and more
- Full offline support via Service Worker
- Installable as a native-like app (PWA)
- Dark / Light theme toggle
- Favorites & History (localStorage)
- Deep-link support (`?view=finance`)
- Keyboard support on the calculator
- Mobile responsive
- Zero dependencies, pure vanilla JS

## 📊 Calculator Breakdown

| Category | Count | Examples |
|---|---|---|
| 🎓 Academic | 6 | CGPA, Attendance, SPI/CPI, Grade Target |
| 💰 Finance | 6 | EMI, Compound Interest, Income Tax, SIP |
| 🛒 Shopping | 6 | Discount, GST, Multi-Discount, Cashback |
| 🚗 Fuel & Travel | 5 | Fuel Cost, Round Trip, Petrol vs EV |
| ❤️ Health | 5 | BMI, TDEE/Calories, Water Intake |
| 💾 CS & Binary | 6 | 1's/2's Complement, Base Converter, IEEE 754 |
| ⚗️ Science | 5 | Force, Ohm's Law, pH, Half-Life, Ideal Gas |
| 🔊 Sound | 5 | Frequency, Decibel, Music Notes, Doppler |
| 🔄 Converters | 10 | Length, Weight, Temperature, Speed, Area |
| 🏡 House & Area | 7 | Room Area, Paint, Flooring, Plot Area |
| ➗ Math | 6 | Percentage, Quadratic, GCD/LCM, Factorial |
| 💻 Tech | 5 | Storage, Binary, Bandwidth, Uptime |
| 🏠 Daily Life | 5 | Electricity, Age, Tip, Sleep Cycle |
| 🧠 Productivity | 5 | Time Allocation, Task Priority, Goal Progress |
| 📅 Date & Time | 5 | Date Diff, Time Calc, Unix Timestamp |
| 📐 Equations | 4 | Linear, X→Y Table, Ratio, Percentage |
| 🔡 Alphabet | 5 | Letter Position, Word Value, Caesar Cipher |
| 🌐 Global | 5 | Currency, PayPal Fees, Fiverr Income |

**Total: 96 calculators**

## 🚀 Quick Start

See [STARTUP_GUIDE.md](STARTUP_GUIDE.md) for complete deployment instructions.

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/universal-calculator-hub.git
cd universal-calculator-hub

# Run locally (requires Node.js)
npm start
# Opens at http://localhost:3000
```

Or just open `index.html` directly in a browser — no build step needed.

## 📦 What's Included

```
calc-hub-app/
├── index.html          # Main app shell
├── app.js              # All 96 calculators + logic
├── style.css           # All styles (dark/light theme)
├── manifest.json       # PWA manifest
├── sw.js               # Service worker (offline support)
├── icons/              # App icons (192x192, 512x512)
├── package.json        # npm scripts
├── STARTUP_GUIDE.md    # Complete deployment guide
└── CONTRIBUTING.md     # How to add calculators
```

## 🤝 Contributing

Want to add a calculator? See [CONTRIBUTING.md](CONTRIBUTING.md)

## 📄 License

MIT — see [LICENSE](LICENSE)

## 🔒 Security

See [SECURITY.md](SECURITY.md) for security policy and reporting vulnerabilities.

---

**Made with ❤️ for students, professionals, and anyone who needs quick calculations**
