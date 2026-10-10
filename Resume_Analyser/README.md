# Resume Analyzer

An AI-powered resume review application that helps job seekers evaluate their CVs against a target role. Users can upload a resume, provide company and job details, and receive ATS-friendly feedback, scoring insights, and content suggestions to improve their chances of getting shortlisted.

## Overview

This project is a React + Vite + React Router application that uses Puter.js for authentication, file storage, and AI-powered analysis. It is designed for quick resume feedback cycles and stores each analysis result locally in the browser environment via Puter storage.

## Features

- Upload a resume in PDF format
- Enter company name, job title, and job description
- Convert the PDF to an image preview for visual review
- Analyze resume quality with AI feedback
- Get ATS score and improvement suggestions
- Review summary insights for content, structure, tone, and skills
- See previously uploaded resumes and saved results
- Generate a tailored resume experience based on the selected job role

## Tech Stack

- React 19
- React Router 7
- TypeScript
- Vite
- Tailwind CSS
- Puter.js (auth, filesystem, KV storage, AI)
- jsPDF / PDF processing helpers
- docx support in dependencies

## Project Structure

```bash
Resume_Analyser/
├── app/
│   ├── components/
│   ├── lib/
│   ├── routes/
│   ├── app.css
│   ├── root.tsx
│   ├── routes.ts
│   └── welcome/
├── constants/
├── public/
├── types/
├── .dockerignore
├── .gitignore
├── Dockerfile
├── package.json
├── react-router.config.ts
├── tsconfig.json
├── vite.config.ts
└── README.md
```

## Prerequisites

- Node.js 20 or later
- npm 10 or later
- A modern browser
- Access to Puter.js authentication in the browser runtime

## Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd Resume_Analyser
```

2. Install dependencies:

```bash
npm install
```

## Running the App

Start the development server:

```bash
npm run dev
```

Then open the local URL shown in the terminal, usually:

```bash
http://localhost:5173
```

## Production Build

Build the app for production:

```bash
npm run build
```

Run the built app:

```bash
npm run start
```

## Type Checking

```bash
npm run typecheck
```

## How It Works

1. The user signs in using Puter authentication.
2. A resume PDF is uploaded and stored in the Puter filesystem.
3. The PDF is converted into an image preview for display.
4. The user enters details about the target company and role.
5. The app sends the resume and prompt context to the Puter AI service.
6. AI returns structured evaluation data such as scores, ATS feedback, content suggestions, and skills guidance.
7. Results are saved and displayed on the resume review page.

## Scripts

```bash
npm run dev      # Start the app in development mode
npm run build    # Create a production build
npm run start    # Serve the production build
npm run typecheck # Run TypeScript validation
```

## Notes

- This app depends on Puter.js being available in the browser environment.
- It is optimized for resume review workflows and may require valid user authentication before analysis begins.
- The project was built as a portfolio-style or proof-of-concept AI resume evaluation tool.

## License

This project does not currently include a license file. If you plan to distribute or reuse it, add an appropriate license before publishing.
