# HRD-Special-Lecture

Reference materials and prompt library for an HRD special lecture demonstrating practical Gemini workflows across three surfaces: conversational chat, Google Opal node-based tools, and Google Sheets with Canvas.

## Repository Structure

- **`chat-prompts/`** — Multi-part prompts for testing how Gemini handles sequential requests in a single conversation. Each topic is split into three numbered prompts (brief, visual, interactive sandbox) so the audience can see discrete outputs build on each other.

- **`opal-services/`** — Setup documentation for node-based AI utilities built inside Google Opal. Each file describes the system architecture, the build prompt, and realistic test inputs for the tool.

- **`gemini-google-sheets/`** — Prompts for generating mock data and building editable dashboards directly inside Google Sheets using Gemini and the Canvas feature.

- **`demo-workflow/`** — Live demonstration scripts and step-by-step reference flow for running the seminar.

## How to Use

Every prompt in this repo lives inside a code block with a copy button. Open any `.md` file, copy the prompt, and paste it into the relevant surface:

- Chat prompts go into the Gemini chat interface
- Opal service prompts go into the corresponding node configuration in Google Opal
- Sheets prompts go into Gemini inside Google Sheets (chat or Canvas, as noted per file)

Many files also include preview screenshots showing what the generated output looks like.

## Topics Covered

**Chat prompts**
- Next.js Server Components vs Client Components
- CSS Flexbox vs Grid

**Opal tools**
- Feature-to-Database Planner — converts feature descriptions into Frontend UI, Backend API, and Database schema layers
- Non-Linear Full-Stack Error Detective — analyzes stack traces and produces a prioritized debugging checklist
- API Payload Structure Visualizer — traces how data changes shape from client to validation to database
- DevData Engine — generates TypeScript interfaces and matching mock JSON datasets

**Google Sheets**
- Budget Tracking Dashboard — two-step workflow: generate mock spending data, then build an editable dashboard via Canvas
