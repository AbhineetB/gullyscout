# GullyScout 🌿

**Turn an ordinary walk into a small adventure.**

GullyScout is a mobile-friendly web app that encourages people to step away from their screens and explore the world around them through neighbourhood scavenger hunts.

From old buildings and local shrines to trees and hidden corners, the idea is to notice the interesting things we usually walk past every day.

Built for the **Hacktoberfest Open-Source AI Challenge — Week 1: Touch Grass**.

## 🌍 Live Demo

[**Try GullyScout**](https://gullyscout-ai-test-c2in2k8rh-abhi-261c.vercel.app/)

## ✨ Features

- **Real-world exploration:** Discover your surroundings through scavenger-hunt challenges.
- **Mobile-friendly design:** Use the app while exploring outdoors.
- **Photo-based interaction:** Take or upload pictures related to a challenge.
- **AI experimentation:** Explore how image-text similarity can help match photos to challenge descriptions.
- **Open-source AI:** Experiment with running a lightweight vision-language model directly in the browser.

*Note: AI functionality is experimental and may not work reliably in every environment.*

## 🤖 AI Technology

GullyScout explores the use of **MobileCLIP-S0**, a lightweight vision-language model designed for image and text understanding.

The intended approach uses:

- **MobileCLIP-S0:** For comparing images with text descriptions.
- **Transformers.js:** To load and run compatible machine-learning models in JavaScript.
- **ONNX Runtime Web:** For browser-based model inference.

The goal is to process images on the user's device rather than depend on a paid cloud inference API.

Actual model performance depends on successful model loading, browser compatibility, and prediction quality. The AI should be treated as an experimental helper, not as proof that someone visited a particular location.

## 🛠️ Built With

- HTML
- CSS
- JavaScript
- MobileCLIP-S0
- Transformers.js
- ONNX Runtime Web
- Vercel for deployment

## 🚀 Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/AbhineetB/gullyscout-ai-test.git
   ```

2. Open the project folder:

   ```bash
   cd gullyscout-ai-test
   ```

3. Start a local development server from the directory that contains the main `index.html` file. For example, if you have Python installed:

   ```bash
   python3 -m http.server 8000
   ```

4. Open [http://localhost:8000](http://localhost:8000) in your browser.

If the project uses locally stored model assets, ensure those files are present at the expected paths. Opening the HTML file directly may not work correctly for browser-based model loading.

## 📁 Project Structure

```text
gullyscout-ai-test/
├── index.html
├── README.md
└── ai-test/
    ├── index.html
    ├── models/
    │   └── mobileclip_s0/
    └── sample images
```

The `ai-test/` directory contains the separate AI testing page and related model assets. The exact files available may vary as development continues.

## 🔒 Privacy and Limitations

- The intended AI approach runs inference locally in the browser.
- No paid inference API is required by the intended design.
- Model files can be large and may take time to load.
- Browser memory and device performance can affect inference.
- Predictions may be incorrect, so AI results should not be treated as definitive verification.

Local processing does not automatically mean the entire application works offline; external scripts and other resources may still require an internet connection.

## 💡 Why GullyScout?

It's easy to spend hours online without paying attention to the places around us. GullyScout is an attempt to use technology as a reason to go outside, explore locally, and notice more of the real world.

The aim isn't to spend more time on an app. It's to use the app to discover something beyond the screen.

## 📌 Challenge

Created for the [Hacktoberfest Open-Source AI Challenge — Week 1: Touch Grass](https://dev.to/challenges/hacktoberfest-week1-2026-10-05).

---

**GullyScout — Look up. Step out. Explore.**
