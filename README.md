# FoodFacts - Search Nutrition Info by Food Name | Part 2

## Kalvium Assignment Submission

**Live Demo:** http://localhost:5173/ (npm run dev)

### Features Implemented
- **Multi-page SPA** with React Router v6: Home, Product Detail, Saved Items
- **Async Data Fetching** with Axios + custom `useFoodSearch` hook
- **Dynamic Routing** `/product/:barcode` → useParams
- **Global State** useReducer for saved items (lifted to App.jsx)
- **Form Validation** & Error Handling (loading/error/empty/validation states)
- **Component Lifecycle** useEffect cleanup, programmatic nav w/ useNavigate
- **Responsive UI** with modern CSS gradients/flex/grid

### Screenshots for PR
```
Home Search: [Imagine screenshot]
Detail Nutrition: [Imagine]
Saved Items w/ Badge: [Imagine]
Error/Validation: [Imagine]
```

### Testing Flow
1. Home: Search "chocolate" → Click card → Detail loads nutrition
2. Detail: Save product → Badge shows 1 → `/saved`
3. Saved: Remove/View Details → Empty state
4. Edge: Empty search, offline, invalid barcode → Graceful errors
5. Nav: All links + Back button work instantly (no reloads)

### Tech Stack
```
React 18 + Vite
React Router v6
Axios
useReducer/useEffect/useCallback
Custom Hooks
Responsive CSS
```

### Run Instructions
```bash
npm install
npm run dev  # http://localhost:5173/
npm run build
```

### Video Walkthrough Script (4-6min)
1. PR overview (files/folder structure)
2. Live demo: full user flow
3. Code deep-dive: useFoodSearch hook, DetailPage useEffect/useParams, App.jsx reducer
4. Key learnings: Custom hooks > inline fetch, lifted state for siblings, cleanup prevents memory leaks

**Branch:** `part2/routing-and-async` → PR to `main`

Ready for submission! 🙌
