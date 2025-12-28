> This project is based on the Mapty application from Jonas Schmedtmann's JavaScript course.
> I significantly refactored the original implementation to introduce a clear MVC architecture,
> focusing on improved state management, separation of concerns, and long-term maintainability.

# 🗺️ Mapty App

Mapty is a map-based workout tracking application built with Vanilla JavaScript,
designed with a clear separation between application state, UI rendering, and control logic.

![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow) ![Architecture](https://img.shields.io/badge/Architecture-MVC-blue) ![Build](https://img.shields.io/badge/Build-Vite-purple)

## 💻 Demo:

🔗 **Live Demo:** https://mapty-mvc-app.netlify.app/

> Try adding a workout by clicking on the map.

## 🌞 Preview:

![Map View](./img/Demo0.png)

![delete Workout](./img/Demo1.png)

## ✨ Features:

- Geolocation-based workout creation
- Running & Cycling workout tracking
- Map markers and route rendering
- LocalStorage persistence

## 🧩 Tech Stack

- Vanilla JavaScript(ES6+)
- Leaflet.js
- HTML5 / CSS3
- LocalStorage API
- Vite (dev & build)

## 🛠️ Architecture

> This project follows a clear MVC pattern

- **mapty-model.js**: application state & business logic
- **sub-model/**: domain entities responsible for workout data modeling and calculations
  (Running, Cycling, and shared Workout logic)
- **mapty-controller.js**: event handling & app flow
- **views/**: UI rendering logic

## 💪 Key Learnings:

- Refactored the application from a single global state into a multi-entity state architecture to improve scalability and maintainability.
- Separated state updates from view rendering to prevent unintended render side effects and ensure predictable UI behavior.
- Applied a clear distinction between domain state and UI instance state to simplify complex UI interactions.
- Used guard conditions strategically to control application flow and handle edge cases in a deterministic way.
- Chose CSS-based solutions over JavaScript for UI-only behaviors to reduce logic complexity.

## ↗️ Future Improvements:

- Enhance workout list UX by highlighting the active item and conditionally rendering action buttons to reduce visual noise.
- Integrate weather data based on workout time and location to provide contextual insights.
- Add reverse geocoding to display human-readable locations from map coordinates.

## 🤖 Quick Start:

```bash
Clone repo
npm install
npm run dev
```
