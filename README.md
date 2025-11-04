# Weather Monitor App 🌤️

A modern weather dashboard built with **v0.dev** and debugged with **Claude** - from a designer's perspective.

![Weather Monitor Preview](./preview.png) *(Add screenshot here)*

## 📺 Video Tutorial

Watch the full build process: [YouTube Link](#) *(coming soon)*

Part of the **Make It Awesome** series on AI-powered design tools.

---

## 🎯 What This Project Demonstrates

As a product designer, I built this functional weather app using:
- **v0.dev** for AI-generated React components
- **Claude** for prompt crafting and debugging
- **Vercel** for one-click deployment

This project shows the **real workflow** of using AI tools - including the bugs, fixes, and iterations that most tutorials skip.

## ✨ Features

- 🌡️ Real-time weather data from OpenWeather API
- 📍 Location search functionality
- 📅 5-day forecast display
- 🎨 Clean, responsive UI with Tailwind CSS
- 🌙 Current conditions with weather icons
- 💨 Wind speed, humidity, and feels-like temperature

## 🛠️ Built With

| Tool | Purpose | Why I Used It |
|------|---------|---------------|
| **v0.dev** | UI generation | Clean React components with shadcn/ui |
| **Claude** | Prompt writing & debugging | Fixed API issues and improved code quality |
| **OpenWeather API** | Weather data | Free tier, well-documented |
| **Vercel** | Deployment | Seamless integration with v0 |

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ installed
- OpenWeather API key ([Get one free here](https://openweathermap.org/api))

### Installation

```bash
# Clone this repo
git clone https://github.com/yourusername/weather-monitor.git
cd weather-monitor

# Install dependencies
npm install

# Add your API key
# Create .env.local file and add:
# NEXT_PUBLIC_OPENWEATHER_API_KEY=your_key_here

# Run locally
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see the app.

### Deploy to Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/weather-monitor)

Don't forget to add your `OPENWEATHER_API_KEY` in Vercel environment variables!

---

## 🎨 The Design Process

### 1. Initial Concept
Started with a simple idea: "I want to check the weather in a clean, modern interface"

### 2. Prompt Crafting with Claude
Instead of going straight to v0, I used Claude to create a detailed prompt:

```
"Create a weather dashboard component with:
- Search bar for city names
- Current weather display with icon
- Temperature, feels like, humidity, wind speed
- 5-day forecast cards
- Clean, modern design using Tailwind
- Responsive layout
- Use shadcn/ui components"
```

### 3. Generation in v0
- Pasted the Claude-crafted prompt into v0
- Got a solid first version
- Made 2-3 iterations for styling tweaks

### 4. The Bugs (The Real Part!)
**Issues I encountered:**
- ❌ API key not loading from environment variables
- ❌ Error handling missing for failed API calls  
- ❌ Location search not updating forecast
- ❌ Mobile responsiveness issues with forecast cards

### 5. Debugging with Claude
I took the error messages and code back to Claude:
- Pasted error logs
- Asked for specific fixes
- Got working solutions in minutes
- Learned *why* the bugs happened

---

## 📂 Project Structure

```
weather-monitor/
├── app/
│   ├── page.tsx              # Main weather dashboard
│   └── api/
│       └── weather/
│           └── route.ts      # API route for weather data
├── components/
│   ├── ui/                   # shadcn/ui components
│   ├── weather-card.tsx      # Current weather display
│   └── forecast-card.tsx     # 5-day forecast
├── lib/
│   └── utils.ts              # Helper functions
└── public/
    └── weather-icons/        # Weather condition icons
```

## 🐛 Common Issues & Fixes

### Issue 1: API Key Not Working
**Problem:** `Error: API key is required`

**Solution from Claude:**
```typescript
// Wrong (v0 generated this)
const API_KEY = process.env.OPENWEATHER_API_KEY;

// Right (Claude fixed it)
const API_KEY = process.env.NEXT_PUBLIC_OPENWEATHER_API_KEY;
```

### Issue 2: Error Handling
**Problem:** App crashes when city not found

**Solution from Claude:** Added try-catch blocks and user-friendly error messages

See `/fixes/` folder for detailed before/after code examples.

---

## 💡 What I Learned

### As a Designer Using AI Tools:

**✅ Do This:**
- Use Claude to write detailed prompts *before* v0
- Keep iterations in v0 minimal to save credits
- Copy errors directly to Claude for debugging
- Test on mobile early

**❌ Avoid This:**
- Don't iterate endlessly in v0 - costs add up
- Don't ignore console errors until later
- Don't deploy without testing API limits
- Don't skip environment variable setup

### The v0 + Claude Workflow Works Because:
1. **v0** generates clean, production-ready React code
2. **Claude** understands the code and fixes it intelligently  
3. You maintain control without writing everything from scratch
4. Perfect for designers who want functional prototypes

---

## 🔗 Resources

### APIs Used
- [OpenWeather API](https://openweathermap.org/api) - Weather data
- [OpenWeather Icons](https://openweathermap.org/weather-conditions) - Weather icons

### Tools
- [v0.dev](https://v0.dev) - UI generation
- [Claude.ai](https://claude.ai) - Prompt crafting & debugging
- [Vercel](https://vercel.com) - Deployment

### Prompts Used
See `/prompts/weather-app-prompts.md` for all prompts used in this project.

---

## 🎥 Video Chapters

*Timestamps from the tutorial video*

- 00:00 - Intro & tool overview
- 02:15 - Crafting the prompt with Claude
- 04:30 - Generating in v0
- 08:45 - First deployment to Vercel
- 10:20 - Discovering the bugs
- 12:00 - Debugging with Claude
- 16:30 - Final result & key takeaways

---

## 🤝 Contributions

Found a bug? Have a better prompt? Want to add features?

- **Issues:** Report bugs or suggest improvements
- **Pull Requests:** Share your enhancements
- **Discussions:** Share your version or ask questions

## 📱 Connect

Built by a designer learning to code with AI.

- **YouTube:** [Make It Awesome](#)
- **More Projects:** [github.com/yourusername/makeitawesome](https://github.com/yourusername/makeitawesome)

---

## 📝 License

MIT License - use this code however you want!

---

### ⭐ If this helped you:
- Subscribe to the [YouTube channel](#)
- Star this repo
- Share with other designers exploring AI tools

---

**Built with v0, debugged with Claude, deployed on Vercel.**

*Showing the real process - bugs and all.* 🛠️
