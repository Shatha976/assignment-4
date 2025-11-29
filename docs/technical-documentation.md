# 📄 Technical Documentation – Assignment 3 Portfolio Website

## 1. Project Overview
This portfolio website showcases my skills, projects, and experience.  
In Assignment 3, the project was expanded with advanced JavaScript logic, performance improvements, API integration, and state management.

---

## 2. Technologies Used
- **HTML5** – Content structure  
- **CSS3** – Layout, animations, responsiveness  
- **JavaScript (ES6)** – Logic, interactivity, API calls  
- **GitHub REST API** – Dynamic project loading  
- **LocalStorage** – Persistent state management  
- **IntersectionObserver** – Lazy animations  
- **GitHub Pages** – Deployment  

---

## 3. File Structure

```
assignment-3/
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── script.js
├── assets/
│   └── images/
├── docs/
│   ├── ai-usage-report.md
│   └── technical-documentation.md
└── README.md
```

---

## 4. Core Features (Technical Breakdown)

### 4.1 Theme Toggle (Light/Dark Mode)
- Uses a button with sun/moon icons  
- Saves selected theme to `localStorage`  
- Updates `<body data-theme="">` dynamically  
- Uses CSS variables for theme colors  
- Applies instantly after page reload  

---

### 4.2 Name Personalization System
- A modal appears if no name exists in storage  
- User enters name → saved in `localStorage`  
- Greeting text updates dynamically:
```
Hi, I'm Shatha! Welcome, <name>!
```
- Includes a **Reset Name** button

---

### 4.3 Session Timer
- Starts counting when page loads  
- Displays elapsed minutes/seconds  
- Updates every second  
- Useful for user engagement tracking  

---

### 4.4 AI Message Enhancer
Transformations supported:
- Friendly  
- Professional  
- Concise  
- Grammar Fix  

Uses a `switch(action)` block to modify the message.  
Shows animated notification when applied.

---

### 4.5 Contact Form Handler
- Validates empty fields  
- Disables send button during simulation  
- Shows confirmation with personalized name  
- Resets form after sending  

---

### 4.6 GitHub API Integration
API endpoint:
```
https://api.github.com/users/<username>/repos?sort=updated
```

Logic:
1. Show loading text  
2. Fetch repositories  
3. On success: generate animated cards  
4. On failure: show error message  
5. Supports reload button  

---

### 4.7 Smooth Scrolling & IntersectionObserver
- All internal links scroll smoothly  
- Elements with `.fade-in` animate only when visible  
- Improves load performance by delaying animations  

---

## 5. Performance Optimization

### Implemented Improvements
- Deferred JavaScript loading  
- Compressed project/hero images  
- Removed unused CSS and redundant styles  
- Cached DOM lookups for performance  
- Used IntersectionObserver instead of scroll events  
- Limited GitHub API fetch to 6 repos  
- Avoided layout thrashing  
- Logged actual load performance in console

### Results
- Faster page load  
- Reduced blocking scripts  
- Smooth animations  
- Excellent performance for a static site  

---

## 6. Responsiveness
- Layout adjusts using CSS Grid & Flexbox  
- Text uses `clamp()` for scalable size  
- Mobile-friendly navigation  
- Fully responsive on all devices  

---

## 7. Future Enhancements
- Backend integration for real message sending  
- Multi-language support  
- AI-powered GitHub project summaries  
- Dark/light theme auto-detection  

---

## 8. Credits
Created by **Shatha Alharbi**  
Assignment: **SWE – Assignment 3**
