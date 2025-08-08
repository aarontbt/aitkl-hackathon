# AI4MY: ASEAN AI Code Fest - Buildathon

## Challenge Title
**Healthcare Reimagined: Building the Future of Malaysian Health**

## Overview
This Build-a-thon challenges teams to create AI-powered prototypes that radically reimagine Malaysian healthcare.
Focus is on **bold, functional concepts** addressing:
- Clinician burnout
- Patient experience
- Proactive public health

## Tracks
### 1. Supercharged Clinician
- **Problem**: Clinicians face admin overload and fragmented data.
- **Mission**: Automate tasks, unify data into insights, and reduce cognitive load.

### 2. Seamless Patient Journey
- **Problem**: Patient navigation is confusing and fragmented.
- **Mission**: Make healthcare access intuitive, personalized, and proactive.

### 3. Proactive Public Health Shield
- **Problem**: Public health is often reactive, slow to spot emerging threats.
- **Mission**: Build AI-driven early warning & rapid response systems.

## Personas
- **Dr. Aisha (Clinician)**: Overwhelmed by admin and fragmented systems.
- **Uncle Tan (Patient)**: Struggles with navigation & care continuity.
- **Siti (Analyst)**: Needs faster, automated outbreak intelligence.

## Deliverables
- Working prototype (public URL)
- Polished UI with "wow" factor
- Functional backend
- 5-min live pitch & demo
- 30–60 sec video demo
- Public GitHub repo with README

## Judging Criteria (100 pts)
1. **Impact & Vision** – 35%
2. **UX & Design** – 30%
3. **Technical Implementation** – 25%
4. **Pitch & Storytelling** – 10%

## Constraints
- Any tech stack allowed
- Teams create/simulate data
- Use AI APIs & low-code tools encouraged

## Recommended Tech Stack
- **Framework**: Next.js 15 (App Router) + TypeScript
- **UI**: Tailwind CSS + shadcn/ui (Radix-based) + Motion
- **Data/state**
  - **App data**: Convex React `useQuery`, `useMutation`, `useAction` (realtime by default)
  - **Forms**: React Hook Form + Zod (shared schemas)
- **Backend**: Convex (database, auth, storage, realtime, serverless functions)
  - Define schema in `convex/schema.ts`; types generated via Convex codegen
  - HTTP actions for webhooks (e.g., Stripe) with inline CORS handling
  - Functions named in kebab-case for consistency
- **Types/validation**: Convex generated types + Zod
- **AI**: Vercel AI SDK (with OpenAI/Anthropic)
- **Payments**: Stripe via Convex HTTP action webhook; verify signatures with Stripe webhook secret
- **Testing/quality**: Vitest, React Testing Library, Playwright; ESLint + Prettier
- **Dev/infra**: pnpm, GitHub Actions (lint/typecheck/test), Vercel (frontend), Convex Cloud (backend)

## Ideas

Telehealth Chatbot: How about creating a chatbot that answers patient questions, checks symptoms, and helps with booking appointments? It's a great way to mess around with natural language processing! Modern AI tools can help you integrate with existing language models or build your own.

Predictive Readmission Tool: Dive into some data and create a model that predicts which patients might end up back in the hospital. It's a solid way to flex your machine learning skills. AI coding assistants can help you implement the ML models and data processing pipelines!

Medication Reminder App: Design an app that reminds people to take their meds and warns them about potential drug interactions. You could even hook it up to health data APIs! AI can help you write the API integrations and build a robust notification system.

Remote Patient Monitoring: Build a system that collects data from wearables and keeps tabs on patients' health in real-time. This is a cool way to explore IoT and data analysis. AI can assist with both the frontend and backend development!

Clinical Decision Support Tool: Make a tool that gives healthcare pros solid recommendations based on patient data. You'll get to work with databases and learn about clinical guidelines. AI can help you design the database schema and implement the recommendation algorithms!

Remote Monitoring Systems: AI-powered devices can continuously monitor patients' vital signs and alert healthcare providers to any concerning changes, enabling proactive care management.

Clinical Decision Support Tool: Make a tool that gives healthcare pros solid recommendations based on patient data. You'll get to work with databases and learn about clinical guidelines. AI can help you design the database schema and implement the recommendation algorithms!

AI-Driven Nutrition Advisor: Develop an app that provides personalized meal plans and nutrition advice based on user preferences, dietary restrictions, and health goals. Use AI to analyze user data and suggest recipes, grocery lists, and nutritional tips. This app can help users make healthier food choices and track their nutritional intake effectively.

AI-Powered Symptom Checker: Develop a smartphone app that uses AI to analyze symptoms and suggest possible conditions. This can be a handy tool for users