
# ReframeCaster - Farcaster Positive Reframing Tool

**Turn Negativity Into Positivity with AI-Powered Language Transformation**


ReframeCaster is a Farcaster Mini App that helps users transform negative or hostile language into positive, constructive communication using AI-powered sentiment analysis and reframing.

## 🎯 Research Scope (Batasan Masalah)

This application was developed with specific research constraints:

### 1. **Platform Scope**

- **Exclusive to Farcaster**: This system is designed specifically for the Farcaster social platform ecosystem
- **Post Creation Focus**: Covers interaction through post/cast creation only
- **Not included**: Other social media platforms (Instagram, TikTok, YouTube, Facebook)

### 2. **Input Processing**

- **Text-only**: Processes text input in **English and Bahasa (Indonesia)** languages only
- **No multimedia**: Does not process or moderate images, audio, or video content

### 3. **AI Technology Approach**

- **Third-party LLM API**: Uses Google Gemini API via third-party service
- **Prompt Engineering**: Focuses on prompt engineering optimization for reframing results
- **No fine-tuning**: Does not include fine-tuning or training LLM models from scratch

### 4. **API Key Management**

- **BYOK (Bring Your Own Key)**: Users must configure their own API keys
- **Client-side Configuration**: API keys are set up directly in the app interface
- **Encrypted Storage**: Keys are encrypted and stored locally in the browser

### 5. **Reframing Strategy**

- **Positive Rephrasing**: Focuses on transforming negative tone into constructive communication
- **Preserves Core Meaning**: Does not change the fundamental message intent
- **Empathetic Language**: Emphasizes empathy and professional communication

### 6. **Functional Features**

Based on user needs survey, features are limited to:

- ✅ **Text Input**: Draft messages in English or Bahasa
- ✅ **Automatic Reframing**: AI-powered reframing using Gemini
- ✅ **Simple Sentiment Statistics**: Track analysis history (total, negative, positive)
- ✅ **Direct Publish to Farcaster**: One-click publish to Farcaster feed

---

## 🚀 Features

### 1. **Bilingual Sentiment Analysis**
- [React 19 Documentation](https://react.dev/)
- [Google Gemini API](https://ai.google.dev/gemini-api/docs)

# ReframeCaster

**AI-Powered Positive Language Reframing for Farcaster**

ReframeCaster is a professional Farcaster Mini App that leverages AI to transform negative or hostile language into positive, constructive communication. Designed for seamless integration with the Farcaster platform, it empowers users to communicate empathetically and professionally.

---

## Key Features

- **Bilingual Sentiment Analysis:**
  - Detects sentiment in English and Bahasa Indonesia
  - Identifies negative, aggressive, passive-aggressive, or neutral tones
  - Provides reasoning for detected sentiment

- **AI-Powered Positive Reframing:**
  - Instantly transforms negative language into constructive alternatives
  - Preserves the core message and intent
  - Utilizes Google Gemini 2.5 Flash for fast, accurate results

- **Statistics Dashboard:**
  - Tracks total analyses, negative, and positive sentiment counts
  - Stores statistics securely in the browser

- **Direct Farcaster Integration:**
  - Compose and publish casts directly from the app
  - One-click "Use & Publish" for immediate action

- **Secure API Key Management (BYOK):**
  - Users provide their own API keys (no server-side storage)
  - Client-side encryption with Web Crypto API

---

## Technology Stack

- **Framework:** Next.js 16 (App Router, React 19.2, Turbopack)
- **UI:** Shadcn/ui, Radix UI, Tailwind CSS
- **AI Model:** Google Gemini 2.5 Flash via `@google/genai`
- **Farcaster SDK:** `@farcaster/miniapp-sdk`
- **Type Safety:** TypeScript, Zod
- **Linting/Formatting:** Ultracite (Biome)

---

## Getting Started

### Prerequisites

- Node.js 20+ and npm
- Google Gemini API Key ([Get one here](https://aistudio.google.com/app/apikey))
- Farcaster account (for publishing casts)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/ola-akanbi/reframe-caster.git
   cd reframe-caster
   npm install
   ```
2. (Optional) Configure environment variables in `.env.local` for deployment.
3. Start the development server:
   ```sh
   npm run dev
   ```
4. Open [http://localhost:3000](http://localhost:3000) in your browser.

### API Key Setup

1. Enter your Google Gemini API key in the app interface when prompted.
2. The key is encrypted and stored locally in your browser.
3. You can clear and reconfigure the key at any time.

---

## Usage

1. Draft your message in English or Bahasa Indonesia.
2. Click "Analyze & Refine" to process your text.
3. Review the sentiment analysis and positive reframe suggestion.
4. Choose to keep your original, use the suggestion, or publish directly to Farcaster.
5. Track your sentiment statistics in the dashboard.

---

## Security & Privacy

- API keys are encrypted using AES-GCM and stored only in your browser.
- No text or keys are stored on any server (except for Gemini API requests).
- All statistics and data remain private and local to your device.

---

## Research Scope & Limitations

- **Platform:** Exclusive to Farcaster (no support for other social platforms)
- **Input:** Text-only (English and Bahasa Indonesia); no multimedia
- **AI:** Uses third-party LLM API (no model fine-tuning)
- **API Keys:** BYOK, encrypted and stored locally
- **Reframing:** Focuses on positive, empathetic language while preserving intent

---

## Code Quality

- Type safety with TypeScript
- Accessible React components
- Modern JavaScript/TypeScript patterns
- Proper error handling
- Semantic HTML
- Linting and formatting with Ultracite (Biome)

Run checks and auto-fix with:
```sh
npm run check
npm run fix
```

---

## Deployment

### Deploy to Vercel

1. Push to GitHub
2. Import to Vercel
3. Configure environment variables as needed
4. Deploy

### Farcaster Manifest

For production as a Farcaster Mini App:

1. Sign your manifest at: <https://farcaster.xyz/~/developers/mini-apps/manifest>
2. Add signed values to environment variables:
   - `FARCASTER_HEADER`
   - `FARCASTER_PAYLOAD`
   - `FARCASTER_SIGNATURE`
3. Ensure `.well-known/farcaster.json` is accessible

Refer to [Farcaster Mini Apps Documentation](https://miniapps.farcaster.xyz/docs/guides/publishing)

---

## Learn More

- [Farcaster Mini Apps Docs](https://miniapps.farcaster.xyz/)
- [Farcaster SDK Reference](https://miniapps.farcaster.xyz/docs/sdk/actions)
- [Publishing Guide](https://miniapps.farcaster.xyz/docs/guides/publishing)
- [Next.js Documentation](https://nextjs.org/docs)
- [React 19 Documentation](https://react.dev/)
- [Google Gemini API](https://ai.google.dev/gemini-api/docs)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)

---

## Contributing

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

---

## License

This project is licensed under the MIT License.

---

## Acknowledgments

- Farcaster Team for the Mini Apps platform
- Google for Gemini API
- Vercel for Next.js and hosting
- Research participants for user needs survey

---

**Made with ❤️ for positive communication on Farcaster**
- Semantic HTML
