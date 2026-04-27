# 🗺️ Mapty – Workout Tracker

Mapty is a browser-based application that allows users to log and track their workouts (running or cycling) on an interactive map. It uses modern JavaScript features and integrates with the Leaflet library for map rendering.

## 🚀 Features

- 📍 Display interactive map using geolocation
- 🏃 Log running workouts (distance, duration, cadence)
- 🚴 Log cycling workouts (distance, duration, elevation gain)
- 🗂️ Store workouts using local storage (persistent data)
- 🔄 Automatically load saved workouts on page refresh
- 🖱️ Click on the map to add new workouts
- 📌 Zoom to workout location on click

## 🧠 Concepts Learned

This project focuses on applying core JavaScript concepts, including:

- Object-Oriented Programming (OOP)
- Classes and inheritance
- Encapsulation and abstraction
- Working with browser APIs (Geolocation API)
- Using external libraries (Leaflet)
- Event handling
- Local storage for data persistence

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- Leaflet.js

## 📦 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/mapty.git
   ```

2. Navigate to the project folder:

   ```bash
   cd mapty
   ```

3. Open `index.html` in your browser.

> ⚠️ Note: Geolocation may not work if you open the file directly. Use a live server (e.g., VS Code Live Server extension).

## 📁 Project Structure

```
mapty/
│── index.html
│── style.css
│── script.js
│── assets/
```

## ⚠️ Known Limitations

When retrieving workout data from local storage, objects lose their prototype chain. This means they no longer inherit methods from their original class instances (e.g., `Running` or `Cycling`).

### Current Approach

- Loop over the data retrieved from local storage
- Recreate objects by instantiating the appropriate class based on stored data

### Temporary Workaround

- Non-essential inherited methods (such as `click()`) are currently disabled

## 🔮 Future Improvements

- Edit existing workouts
- Delete individual workouts
- Sort workouts
- Add more workout types (e.g., swimming)
- Sync with a backend/database
- Improve mobile responsiveness
- Implement a robust solution for restoring prototype chains from local storage

## 🙌 Acknowledgements

This project is part of the JavaScript course by Jonas Schmedtmann.

## 📄 License

This project is for educational purposes and does not include a specific license.
