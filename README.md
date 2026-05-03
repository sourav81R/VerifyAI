# VerifyAI 🛡️  

> **Trust, but Verify.**
> An AI-powered platform for detecting deepfakes, verifying news credibility, and analyzing media integrity.


![Tech](https://img.shields.io/badge/tech-Next.js%20%7C%20TypeScript%20%7C%20Firebase-black)
![AI](https://img.shields.io/badge/AI-Gemini%20%7c%20Genkit-purple)

## 📖 Overview

**VerifyAI** is a modern web application designed to combat misinformation in the digital age. It leverages advanced Large Language Models (LLMs) and computer vision techniques to analyze text, images, and video content. With a futuristic, high-tech interface, users can instantly receive credibility scores, fact-check summaries, and deepfake probability ratings.

## ✨ Core Features

### 🔍 Verification Tools
-   **📝 Text Verification:** Input news headlines or articles to receive a comprehensive AI analysis.
    -   *Outputs:* Credibility score, fact-check summary, and highlighting of manipulated phrases.
-   **🖼️ Image Verification:** Upload images to detect deepfake manipulations.
    -   *Outputs:* Probability score (Real vs. Fake), marked image previews, and referenced articles.
-   **🎥 Video Verification:** Analyze video URLs (YouTube, TikTok, etc.) for inconsistencies.
    -   *Outputs:* Likelihood score and inconsistency analysis.

### 🎨 User Experience
-   **Visual Results Dashboard:** Results are presented in animated cards with clear color-coded trust indicators:
    -   🟢 **Green:** Reliable
    -   🟡 **Yellow:** Suspicious
    -   🔴 **Red:** Fake
-   **Responsive Design:** Seamless experience across mobile and desktop devices.
-   **Theme System:** Fully supported Light and Dark modes with a high-tech aesthetic.

## 🛠️ Tech Stack

### Frontend
-   **Framework:** [Next.js 15](https://nextjs.org/) (App Router)
-   **Language:** [TypeScript](https://www.typescriptlang.org/)
-   **Styling:** [Tailwind CSS](https://tailwindcss.com/)
-   **UI Components:** [Shadcn/ui](https://ui.shadcn.com/) (Radix UI primitives)
-   **Icons:** Lucide React / Clean line-based icons

### Backend & AI
-   **BaaS:** [Firebase](https://firebase.google.com/) (Firestore, Auth)
-   **AI Orchestration:** [Genkit](https://firebase.google.com/docs/genkit)
-   **Logic:** Server Actions (`actions.ts`) & Edge Functions

## 🎨 Design System

The application follows a "Machined & Modern" aesthetic.

| Element | Color / Value | Hex Code | Usage |
| :--- | :--- | :--- | :--- |
| **Primary** | Deep Blue | `#2962FF` | Trust, Technology |
| **Background** | Dark Gray | `#2B3035` | High-tech backdrop |
| **Accent** | Electric Purple | `#BE29FF` | Interactive elements |
| **Font** | Inter | `sans-serif` | Clean, technical readability |

## 📂 Project Structure

The project is organized for scalability, separating UI components, AI logic, and Firebase configurations.

```text
VerifyAi/
├── src/
│   ├── ai/                 # AI Logic & Genkit Flows
│   │   ├── flows/          # Specific analyzers (Image, Text, TTS)
│   │   └── genkit.ts       # Genkit configuration
│   ├── app/                # Next.js App Router Pages
│   │   ├── actions.ts      # Server Actions
│   │   ├── globals.css     # Tailwind & Global Styles
│   │   └── layout.tsx      # Root Layout
│   ├── components/         # React Components
│   │   ├── ui/             # Reusable Shadcn UI components
│   │   ├── layout/         # Header, Footer, Nav
│   │   └── verifier.tsx    # Main Verification Logic
│   ├── firebase/           # Firebase Config & Hooks
│   └── lib/                # Utilities & Types
├── next.config.ts          # Next.js Configuration
└── package.json            # Dependencies
```
## 🚀 Getting Started
   Prerequisites
   
- Node.js (v18 or higher)

- npm or yarn

- A Firebase project with Firestore enabled

## Installation
Clone the repository
```
git clone https://github.com/yourusername/verifyai.git
cd verifyai
```
### Install dependencies
```
npm install
# or
yarn install
```
### Environment Setup Create a .env.local file in the root directory and add your Firebase and AI API keys:
```
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project_id.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
GOOGLE_GENAI_API_KEY=your_gemini_key
```
Run the development server
```
npm run dev
```
Open http://localhost:3000 with your browser.
