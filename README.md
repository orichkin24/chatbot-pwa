# ChatBot PWA

A Progressive Web App (PWA) chatbot built with Next.js, TypeScript, and OpenRouter API.

## Features

- 💬 Real-time chat interface
- 📱 Progressive Web App (installable on mobile/desktop)
- 🎨 Beautiful UI with Tailwind CSS
- 🌙 Dark mode support
- ⚡ Fast and responsive
- 🤖 Powered by OpenRouter AI models

## Prerequisites

- Node.js 18+
- npm or yarn
- OpenRouter API key

## Getting Started

1. **Clone the repository**

```bash
git clone <your-repo-url>
cd chatbot-pwa
```

2. **Install dependencies**

```bash
npm install
```

3. **Set up environment variables**

Create a `.env.local` file in the root directory:

```bash
cp .env.example .env.local
```

Edit `.env.local` and add your OpenRouter API key:

```env
OPENROUTER_API_KEY=your_api_key_here
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

Get your OpenRouter API key from: https://openrouter.ai/keys

4. **Run the development server**

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

5. **Build for production**

```bash
npm run build
npm start
```

## Tech Stack

- **Framework**: Next.js 15
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **PWA**: next-pwa
- **AI**: OpenRouter API
- **Linting**: ESLint

## Project Structure

```
chatbot-pwa/
├── app/
│   ├── api/
│   │   └── chat/
│   │       └── route.ts      # Chat API endpoint
│   ├── layout.tsx            # Root layout with PWA config
│   ├── page.tsx              # Main chat interface
│   └── globals.css           # Global styles
├── public/
│   └── manifest.json         # PWA manifest
├── .env.example              # Environment variables template
└── next.config.ts            # Next.js configuration with PWA
```

## Customization

### Change AI Model

Edit `app/api/chat/route.ts` and change the model:

```typescript
model: "anthropic/claude-3.5-sonnet", // Change to any OpenRouter model
```

Available models: https://openrouter.ai/models

### Update PWA Configuration

Edit `public/manifest.json` to customize app name, colors, and icons.

## License

MIT
