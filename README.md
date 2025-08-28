# IngredientIQ – Smart Cooking Assistant

## ✨ Highlights
- OCR-powered pantry scanning using Google Vision API or Tesseract.js  
- Ingredient-based recipe suggestions with dietary filters (vegan, keto, gluten-free, etc.)  
- Expiry tracking & notifications to reduce food waste  
- Smart recommendations considering cooking tools, time, and skill level  
- AI-enhanced recipe personalization (200+ recommendations supported)  

## 🧱 Tech Stack
**Frontend:** React Native, Tailwind CSS  
**Backend:** FastAPI (Python, async APIs)  
**Database:** PostgreSQL (ingredients, recipes, preferences)  
**OCR & Vision:** Google Vision API / Tesseract.js  
**Caching & Notifications:** Redis + Firebase Cloud Messaging  
**Deployment:** Vercel (frontend), Render/Heroku (backend)  

## 🗺️ Architecture (planned)

flowchart LR
  U[User: React Native App] -->|API calls| B[Backend: FastAPI]
  B -->|SQL| D[(PostgreSQL)]
  B -->|OCR| V[Google Vision / Tesseract.js]
  B -->|cache/events| R[(Redis)]
  B -->|notifications| N[Firebase Cloud Messaging]

  
planned structure

/frontend   # React Native mobile app
/backend    # FastAPI app
/docs       # screenshots, diagrams
