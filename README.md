# Cravely

> Turn whatever is in your fridge into culinary magic.

Cravely is an AI-driven kitchen companion built to eliminate food waste, simplify meal prep, and make home cooking effortless. Powered by Google's Gemini models, Cravely analyzes available pantry items, respects dietary needs, and generates personalized recipes on demand.

## Features

- User registration and login
- Account-specific saved recipes and pantry
- AI-Powered Recipe Generation (via `gemini-3.8-flash`)
- Smart Pantry & Expiry Tracker
- Weekly Meal Planner
- Automated Shopping List generation
- Filter & customize recipes by:
  - Available ingredients
  - Dietary restrictions
  - Cuisine type
  - Cooking time
  - Servings
- Save favorite recipes to dedicated collection
- Detailed recipe views (ingredients, step-by-step instructions, macros, cooking tips)
- Responsive layout & modern UI
- MongoDB / PostgreSQL database for storing user accounts and pantry items

## Tech Stack

### Frontend

- React
- Vite
- React Router
- Tailwind CSS
- Axios
- Lucide React

### Backend

- Node.js
- Express.js
- PostgreSQL (Neon) / MongoDB
- `@google/genai` (Gemini SDK)
- JSON Web Tokens (JWT)
- bcryptjs
- CORS

### API & Services

- Google Gemini API (`gemini-3.8-flash`) for AI generation
- Render (Backend Hosting)
- Vercel (Frontend Hosting)

## Project Structure

```text
Cravely
│
├── aigenerator
│   ├── frontend
│   │   └── aigenerator
│   │       ├── src
│   │       ├── public
│   │       ├── package.json
│   │       └── ...
│   │
│   └── backend
│       ├── controllers
│       ├── routes
│       ├── utils
│       │   └── gemini.js
│       ├── server.js
│       ├── package.json
│       └── ...
│
├── .gitignore
└── README.md
