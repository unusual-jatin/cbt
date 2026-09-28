# J-CBT: JEE Mock Test Simulator 🎯

**Live Demo:** [unusual-jatin.github.io/cbt](https://unusual-jatin.github.io/cbt/)

Preparing for JEE means solving hundreds of mock tests. The problem? Most high-quality resources and coaching materials are shared as PDFs, but the actual JEE (Mains and Advanced) is a strict Computer-Based Test (CBT). 

Solving a PDF on a split-screen or printing it out doesn't build the right exam temperament. You miss out on time management, navigating the question palette, and the general UI of the real exam. 

I built **J-CBT** to fix this. It’s a purely client-side web app that lets you upload any PDF mock test, crop out the questions, and immediately take the test in a UI that closely mimics the actual JEE CBT environment.

---

## ✨ Features

* **Privacy-First PDF Rendering:** Powered by Mozilla's `PDF.js`, everything happens right in your browser. Your PDFs are never uploaded to any server.
* **Smart Cropping Tool:** Drag and draw bounding boxes to extract questions from the PDF.
* **Group Mode:** Some questions span across two pages or have a separate image for options. Group mode lets you stitch multiple crops into a single question.
* **Authentic JEE Interface:** 
  * Question Palette (Not Visited, Not Answered, Answered, Marked for Review).
  * Section-wise tabs (Physics, Chemistry, Math, etc.).
  * Single Correct, Multiple Correct, and Numeric answer types.
  * On-screen virtual keypad for numeric questions.
* **Rough Work Pad:** A built-in text area for quick scribbles (not evaluated, just like the real exam's rough sheets).
* **Detailed Post-Exam Report:** Auto-generates a downloadable HTML report showing the time spent per subject, your responses, and the question images.

---

## 🛠️ Tech Stack

This project is built from scratch without any heavy frontend frameworks. 

* **HTML5 & CSS3:** Responsive UI mimicking the standard exam testing engines (like Ginger Webs / TCS iON).
* **Vanilla JavaScript:** Complex state management for timers, question palettes, and user responses.
* **HTML5 Canvas API:** Used for capturing and clipping the specific pixel regions from the PDF pages.
* **PDF.js:** Mozilla's library for parsing and rendering PDF documents natively in the browser.

---

## 🚀 How to Use (For Students)

1. Open the [Live App](https://unusual-jatin.github.io/cbt/).
2. **Upload:** Select your mock test PDF.
3. **Select & Crop:** Navigate through the PDF pages. Click and drag over a question to crop it. Assign it a subject and expected time. 
4. **Exam Mode:** Once you've cropped your questions, hit "Start Exam". You'll get a 3-hour global timer and the standard JEE testing interface.
5. **Report:** When you submit (or when the time runs out), you'll get a breakdown of your performance which you can download for future analysis.

---
