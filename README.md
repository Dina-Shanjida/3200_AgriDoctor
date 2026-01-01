🌱 AgriDoctor – Crop Disease Detection PWA (Version 2)

AgriDoctor is an AI-powered Progressive Web App (PWA) that helps farmers detect crop diseases instantly using machine learning. The app works offline after initial setup, making it ideal for rural areas with limited or no internet connectivity.

Version 2 introduces improved navigation, prediction history tracking, and farmer-friendly crop knowledge pages.

✨ Features
🔍 AI-Powered Disease Detection

Uses TensorFlow.js machine learning models

Identifies crop diseases from leaf images

🌾 Multi-Crop Support

Corn

Potato

Wheat

📱 Offline-First PWA

Fully functional offline after model download

Ideal for rural and low-connectivity environments

🌐 Bilingual Support

English

Bengali (বাংলা)

📷 Camera & Gallery Integration

Capture photos directly

Upload images from device gallery

🔄 Blur Detection

Automatically detects blurry images

Prompts user to retake clearer photos

🍃 Smart Leaf Detection

Uses COCO-SSD

Automatically detects and crops leaf regions for better accuracy

💡 Treatment Solutions

Disease description

Suggested treatments and solutions

🆕 What’s New in Version 2
🧭 Navbar Navigation

Added a responsive navigation bar

Easy access to:

Home

History

Features

About

🕒 Prediction History Page

Stores previous predictions using localStorage

Farmers can:

View past disease detection results

Track crop health over time

Works fully offline

📘 Features Page (Farmer Knowledge Hub)

Dedicated Features page for farmers

Provides basic agricultural knowledge for:

Corn

Potato

Wheat

Helps farmers:

Understand crops better

Learn common disease patterns

Improve early decision-making

🦠 Supported Diseases
🌽 Corn

Common Rust

Gray Leaf Spot

Leaf Blight

Healthy Detection

🥔 Potato

Early Blight

Late Blight

Healthy Detection

🌾 Wheat

Brown Rust

Yellow Rust

Healthy Detection

🛠️ Tech Stack

Frontend Framework: React 18 + TypeScript

Build Tool: Vite

Styling: Tailwind CSS + shadcn/ui

ML Framework: TensorFlow.js

Object Detection: COCO-SSD (@tensorflow-models/coco-ssd)

PWA: vite-plugin-pwa + Workbox

State Management: React Context API

Routing: React Router DOM

Storage: Browser localStorage (Prediction History)

📦 Installation
Prerequisites

Node.js v18 or higher

npm or bun

Setup
# Clone the repository
git clone https://github.com/Dina-Shanjida/3200_AgriDoctor.git

# Navigate to project directory
cd 3200_AgriDoctor

# Checkout version2 branch
git checkout version2

# Install dependencies
npm install
# or
bun install

# Start development server
npm run dev
# or
bun dev


The app will be available at:
👉 http://localhost:8080

🏗️ Project Structure
src/
├── components/
│   ├── ui/                 # shadcn/ui components
│   ├── Header.tsx          # Navbar
│   ├── PhotoTips.tsx
│   └── ...
├── contexts/
│   └── LanguageContext.tsx
├── data/
│   └── diseaseInfo.ts
├── pages/
│   ├── Index.tsx
│   ├── About.tsx
│   ├── History.tsx         # Prediction history page (NEW)
│   ├── Features.tsx        # Crop features & info page (NEW)
│   └── NotFound.tsx
├── screens/
│   ├── HomeScreen.tsx
│   ├── ImagePreview.tsx
│   ├── PredictionResult.tsx
│   └── LanguageSelection.tsx
├── services/
│   ├── predictionService.ts
│   └── modelPreloader.ts
└── hooks/

🧠 ML Pipeline

Image Capture (Camera / Gallery)

Blur Detection (Laplacian Variance)

Leaf Detection (COCO-SSD)

Image Preprocessing (224×224, RGB normalization)

Model Inference (Crop-specific TensorFlow.js model)

Results Display (Disease name, description, solution)

Save Prediction to History (localStorage)

🌍 Localization

English (Default)

Bengali (বাংলা)

Language preference is stored in localStorage and persists across sessions.

📄 License

This project is open-source and available under the MIT License.

👥 Contributing

Contributions are welcome!
Feel free to open issues or submit pull requests.

📞 Support

For support or bug reports, please open an issue on GitHub.

Made with ❤️ for farmers
© 2025 AgriDoctor
