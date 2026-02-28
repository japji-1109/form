# form

📘 Offline Learning Notes App

A simple and responsive web application built using HTML, CSS, and JavaScript that allows users to save learning notes locally using Local Storage.

The app works even without an internet connection and provides real-time online/offline status updates.

📌 Project Overview

The Offline Learning Notes App is designed to:

Allow users to write topic-based notes

Save notes locally in the browser

Automatically load saved notes on page refresh

Detect internet connectivity status

Work completely offline

This project demonstrates how to use Web Storage API (localStorage) and browser network detection features.

🚀 Features

✅ Save notes offline using localStorage

✅ Auto-load saved notes on page reload

✅ Online / Offline detection

✅ Clean modern UI with gradient background

✅ Responsive layout

✅ Hover animation effects

✅ User-friendly interface

🛠️ Technologies Used

HTML5

CSS3

JavaScript (ES6)

Web Storage API (localStorage)

Browser Network API (navigator.onLine)

📂 Project Structure
Offline-Notes-App/
│
├── index.html
└── README.md
🖥️ How to Run the Project

Download or clone the project folder.

Open the folder.

Double-click on index.html.

The app will open in your browser.

No installation required.
No backend required.
Works fully in the browser.

📖 Application Features Explanation
1️⃣ Saving Notes Offline

When the form is submitted:

localStorage.setItem("topic", topicInput.value);
localStorage.setItem("notes", notesInput.value);

Data is stored inside the browser.

It remains saved even after refreshing the page.

No internet required.

2️⃣ Loading Saved Notes

On page load:

window.onload = () => {
  topicInput.value = localStorage.getItem("topic") || "";
  notesInput.value = localStorage.getItem("notes") || "";
};

This ensures:

Previously saved notes automatically appear.

Data persistence is maintained.

3️⃣ Online / Offline Detection

The app uses:

navigator.onLine

Event listeners:

window.addEventListener("online", updateStatus);
window.addEventListener("offline", updateStatus);

This allows the app to:

Display “You are online 🌐”

Display “You are offline 📵 (App still works)”

4️⃣ UI Design Features

Gradient background using:

background: linear-gradient(135deg, #ff9a9e, #fad0c4);

Soft card design with:

Rounded corners

Box shadow

Smooth hover animations

📱 Responsive Design

Uses Flexbox for centering

Works on mobile, tablet, and desktop

Input fields adjust automatically

🎯 Learning Objectives

This project demonstrates:

How to use Local Storage

How to store and retrieve browser data

Event handling in JavaScript

Form submission handling

Online/Offline detection

Modern CSS styling

UI/UX design principles

🔮 Future Enhancements

Add multiple note saving (array storage)

Add delete button

Add edit option

Add dark mode

Add timestamp for notes

Add IndexedDB support

Convert to PWA (Progressive Web App)

👩‍💻 Author

Name: Japji Kaur
Course: B.Tech – 1st Year
Project Type: Web Development Mini Project
