# 🛒 AI Grocery List Generator

An intelligent, AI-powered grocery list generator and meal planning assistant built with React. Plan your meals, set dietary preferences, and instantly generate organized, categorized shopping lists — or chat with an AI assistant for recipe ideas and grocery advice. conver this into new form of saying

> Powered by **Groq API** (LLaMA 3.3 70B) for fast, accurate grocery and meal planning responses.

---

## ✨ Features

### 🍽️ Meal Planner
- **Add meals** with name, type (Breakfast / Lunch / Dinner / Snack / Dessert), and serving count
- **Dietary preferences** — Vegetarian, Vegan, Gluten-Free, Keto, Low-Carb, Dairy-Free, Paleo
- **Allergy & restriction input** for personalized lists
- **Budget level selection** — Budget, Regular, or Premium
- **One-click generation** of a complete, categorized grocery list with quantities and shopping tips

### 💬 Chat Assistant
- Conversational AI that answers grocery, recipe, and meal prep questions
- **Smart detection** — automatically generates structured grocery lists when shopping-related queries are detected
- **Quick suggestion chips** for common prompts like meal plans, ingredient lists, and budget shopping
- Copy any generated list to clipboard instantly

### 🎨 Design
- Dark green-themed UI with a clean, modern aesthetic
- Categorized items with emoji icons (🥦🍎🧀🥩🍞 and more)
- Responsive layout that works on desktop and mobile
- Smooth animations and polished micro-interactions

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher)
- npm (comes with Node.js)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/ai-grocery-list-generator.git
   cd ai-grocery-list-generator
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | React 19 (Create React App) |
| **AI / LLM** | Groq API — LLaMA 3.3 70B Versatile |
| **Styling** | Inline CSS with a custom design system |
| **Language** | JavaScript (JSX) |

---

## 📁 Project Structure

```
ai-grocery-list-generator/
├── public/
│   ├── index.html
│   ├── favicon.ico
│   └── manifest.json
├── src/
│   ├── App.jsx          # Main application (planner + chat + API logic)
│   ├── App.css           # Base styles
│   ├── index.js          # React entry point
│   └── index.css         # Global styles
├── package.json
└── README.md
```

---

## 🔧 How It Works

1. **Meal Planner tab** — User adds meals with type and servings, selects diet/budget preferences, then clicks "Generate Grocery List." The app constructs a structured prompt and sends it to the Groq API requesting a JSON response with categorized items, quantities, and shopping tips.

2. **Chat Assistant tab** — Free-form conversation with the AI. The app detects grocery-related queries using keyword matching and automatically requests structured JSON grocery lists. Non-grocery queries receive standard conversational responses. The AI is domain-restricted to food, nutrition, and meal planning topics.

---

## 🌐 Deployment

This is a **static site** (no backend server) and can be deployed for free on any static hosting platform.

### Deploy on Render

1. Push your code to GitHub
2. Go to [render.com](https://render.com) → **New** → **Static Site**
3. Connect your repository
4. Set:
   - **Build Command:** `npm install && npm run build`
   - **Publish Directory:** `build`
5. Deploy 🚀

### Other Platforms

| Platform | Build Command | Output Directory |
|----------|---------------|------------------|
| **Vercel** | `npm run build` | `build` |
| **Netlify** | `npm run build` | `build` |
| **GitHub Pages** | `npm run build` | `build` |

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
