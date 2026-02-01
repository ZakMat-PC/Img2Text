# LensAI - Portable Deployment Guide

This project is configured to run on any standard Node.js environment, including HuggingFace Spaces, Heroku, or your local machine.

## Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- An OpenAI API Key

## Setup and Running
   
1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Configure Environment Variables**:
   Create a `.env` file in the root directory (or set these in your hosting provider's dashboard):
   ```env
   OPENAI_API_KEY=your_actual_api_key_here
   NODE_ENV=production
   ```

"3". **Build and Start**:
   ```bash
   npm run build
   npm run start
   ```

## Development Mode

To run with live reloading:
```bash
npm run dev
```

## Running on HuggingFace Spaces

1. Create a new "Node.js" Space.
2. Upload the files (excluding `node_modules`).
3. Add your `OPENAI_API_KEY` to the Space's **Secrets**.
4. HuggingFace will automatically run the build and start commands defined in `package.json`.
