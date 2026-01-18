# 🎭 EmotiSense
**Emotion-Aware Conversational UI**


> **A sophisticated chat interface that understands how you feel—detecting emotions from text, voice, and video, then adapting its responses and visual design in real-time to create a more empathetic, supportive conversation experience.** ✨

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1--mini-green.svg)](https://openai.com/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black.svg)](https://vercel.com/)

---

## ✨ What It Does

EmotiSense is an intelligent conversational interface that uses **advanced multimodal emotion inference** to:

1. **Detect Emotions** — Analyze text, audio transcripts, and video transcripts to identify emotional states with high precision
2. **Adapt Responses** — Generate contextually appropriate, empathetic responses that match the user's emotional state
3. **Transform UI** — Dynamically adjust visual themes, color accents, and suggestion chips based on detected emotions
4. **Provide Insights** — Offer detailed analytics and emotional pattern recognition across conversations

All powered by real-time AI inference with seamless, state-driven UI updates—no page reloads, just smooth, responsive interactions.

---

## 🎯 Core Features

### 🧠 **Advanced Emotion Intelligence**
- **Multimodal Detection** — Analyzes text, audio transcripts, and video transcripts for comprehensive emotion understanding
- **Real-time Classification** — Detects 7 emotional states (joy, sadness, anger, fear/anxiety, disgust, surprise, neutral) with confidence scoring
- **Contextual Awareness** — Considers conversation history for more accurate emotion detection
- **Structured Output** — Reliable JSON parsing with robust error handling

### 💬 **Intelligent Response Generation**
- **Tone Adaptation** — Assistant responses dynamically adjust to match emotional context
- **Empathetic Communication** — Emotion-specific response strategies (calm for anxiety, celebratory for joy, supportive for sadness)
- **Conversation Continuity** — Maintains context across extended conversations
- **Safety Features** — Built-in self-harm detection with appropriate crisis resources

### 🎨 **Adaptive User Experience**
- **Dynamic Theming** — UI colors, accents, and visual elements subtly shift based on emotional state
- **Smart Suggestions** — AI-powered conversation starters tailored to current emotion and context
- **Emotion Timeline** — Visual representation of emotional patterns over time
- **Glassmorphism Design** — Modern, translucent UI with cinematic video backgrounds

### 📊 **Analytics & Insights**
- **Conversation Analytics** — Comprehensive emotion distribution charts and frequency analysis
- **Emotional Insights** — Deep dive into emotional patterns, transitions, and recommendations
- **Export Capabilities** — Download conversations as Markdown or JSON
- **Share & Collaborate** — Share conversations with others

### 🎤 **Multimodal Input Support**
- **Text Input** — Primary communication method with real-time emotion detection
- **Voice Recording** — Capture audio with optional transcript analysis
- **Video Support** — Video capture with transcript-based emotion inference
- **Voice-to-Text** — Real-time speech recognition for hands-free interaction

### 📱 **Modern Mobile Experience**
- **Responsive Design** — Beautiful, functional experience across all device sizes
- **Touch-Optimized** — 44px+ touch targets, safe area support for notched devices
- **Bottom Navigation** — Intuitive mobile navigation with hamburger menu
- **Keyboard Handling** — Smart scroll-to-input when keyboard appears

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16** | React 19.2 with App Router, Server Components |
| **TypeScript** | Type-safe development with strict mode |
| **Tailwind CSS** | Utility-first styling with custom design tokens |
| **shadcn/ui** | Beautiful, accessible component library |
| **Recharts** | Interactive data visualizations |
| **Lucide Icons** | Modern, consistent iconography |
| **next-themes** | Seamless dark/light mode support |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance async Python API |
| **OpenAI GPT-4.1-mini** | Advanced emotion classification & response generation |
| **Pydantic v2** | Robust data validation & serialization |
| **asyncio** | Efficient async/await patterns |

### **Data & Infrastructure** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL with RPC functions for secure schema access |
| **Upstash Redis** | Job orchestration, caching, rate limiting |
| **RPC Architecture** | Secure private schema access via public functions |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting with edge optimization |
| **Railway** | Backend API with auto-scaling |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INPUT                               │
│    Text Message + Optional Audio/Video + Transcript         │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│              EMOTION CLASSIFICATION                         │
│  ┌────────────────────────────────────────────────────┐    │
│  │  OpenAI GPT-4.1-mini analyzes:                    │    │
│  │  • Text content                                    │    │
│  │  • Audio/video transcripts                        │    │
│  │  • Conversation history                           │    │
│  │  → Returns: emotion, confidence, arousal, valence │    │
│  └────────────────────────────────────────────────────┘    │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│              RESPONSE GENERATION                           │
│  ┌────────────────────────────────────────────────────┐    │
│  │  Tone-adapted assistant response:                  │    │
│  │  • Emotion-specific strategies                     │    │
│  │  • Context-aware language                         │    │
│  │  • Empathetic communication                       │    │
│  └────────────────────────────────────────────────────┘    │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│              UI ADAPTATION                                  │
│  • Dynamic theme colors & accents                          │
│  • Emotion-specific suggestion chips                      │
│  • Visual emotion indicators                              │
│  • Smooth, state-driven transitions                       │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎨 Design Philosophy

### **Empathetic, Not Manipulative**
Every interaction is designed to support and understand, never to exploit emotional states. The UI adapts subtly, creating a calming presence for distress and celebrating positive moments authentically.

### **Multimodal Intelligence**
By analyzing text, voice, and video transcripts together, the system builds a comprehensive understanding of emotional context that goes beyond surface-level sentiment analysis.

### **Real-Time Responsiveness**
Emotion detection and UI adaptation happen instantly, creating a fluid experience where the interface feels alive and responsive to the user's state.

### **Accessibility First**
- WCAG AA contrast compliance
- Keyboard navigation throughout
- Screen reader support
- Reduced motion preferences
- Mobile-optimized touch targets

---

## 📸 Key Experiences

### 🏠 **Landing Page**
*Cinematic video backgrounds that adapt to light/dark mode, with clear value proposition and smooth scroll interactions*

### 💬 **Playground**
*Real-time emotion-aware chat interface with dynamic theming, smart suggestions, and conversation history*

### 📊 **Analytics Dashboard**
*Interactive charts showing emotion distribution, frequency patterns, and timeline visualizations*

### 💡 **Insights Page**
*Deep emotional pattern analysis with transition tracking and personalized recommendations*

### 📱 **Mobile Experience**
*Fully responsive design with bottom navigation, hamburger menu, and optimized touch interactions*

---

## 📖 User Guide

### Getting Started

1. **Start a Conversation** — Navigate to the playground and type your first message
2. **See Emotion Detection** — Watch as your emotion is detected and displayed with confidence
3. **Experience Adaptation** — Notice how the UI subtly adapts to your emotional state
4. **Explore Suggestions** — Use AI-powered suggestions to continue the conversation
5. **View Analytics** — Check your conversation analytics for emotional patterns

### Understanding Your Experience

| Feature | What It Does |
|---------|-------------|
| **Emotion Detection** | Real-time classification of your emotional state with confidence scoring |
| **Tone Adaptation** | Assistant responses that match your emotional context (toggleable) |
| **Dynamic Theming** | UI colors and accents that shift based on detected emotion |
| **Smart Suggestions** | Context-aware conversation starters tailored to your state |
| **Analytics** | Visual insights into your emotional patterns over time |
| **Export** | Download conversations as Markdown or JSON for your records |

### Pro Tips

- **Be Authentic** — The system works best with genuine emotional expression
- **Use Voice** — Try voice-to-text for a more natural conversation flow
- **Explore Analytics** — Review your emotional patterns to gain self-awareness
- **Toggle Tone** — Experiment with tone adaptation on/off to see the difference
- **Try Templates** — Use conversation templates for structured interactions

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, airy interface with warm tones
- 🌙 **Dark Mode** — Deep, calming interface optimized for focus
- 🖥️ **System** — Automatically follows OS preference

### Emotion Themes
The UI adapts to detected emotions:
- **Joy** → Warm, celebratory accents
- **Sadness** → Gentle, supportive tones
- **Anger** → Calming, grounding colors
- **Anxiety** → Reassuring, stable palette
- **Neutral** → Balanced, professional theme

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Emotion Detection | ~1-2 seconds |
| Response Generation | ~2-3 seconds |
| Total Response Time | ~3-5 seconds |
| Frontend Bundle | Optimized with code splitting |
| Lighthouse Score | 90+ |
| Mobile Ready | ✅ Fully responsive |
| Accessibility | ✅ WCAG AA compliant |

---

## 🛡️ Safety & Privacy

- ✅ **No Medical Claims** — Assistant does not provide medical diagnosis
- ✅ **Self-Harm Detection** — Pattern matching with crisis resource provision
- ✅ **Privacy-Focused** — Media metadata only (no raw file storage by default)
- ✅ **Rate Limiting** — Per-IP rate limiting via Redis
- ✅ **Secure Schema** — Private database schema accessed via RPC functions
- ✅ **Input Validation** — Comprehensive Pydantic validation
- ✅ **CORS Protection** — Configurable origin restrictions

---

### Test Coverage

- ✅ Emotion detection accuracy across 7 emotional states
- ✅ Response quality and tone adaptation
- ✅ Conversation history persistence
- ✅ Analytics and insights generation
- ✅ Export functionality
- ✅ Mobile responsiveness
- ✅ Accessibility compliance

---

## 🏆 Technical Highlights

This project demonstrates advanced capabilities in:

- **🧠 Multimodal AI Inference** — Combining text, audio, and video transcripts for comprehensive emotion understanding
- **⚛️ Modern React Architecture** — Next.js 16 App Router, React 19.2, Server Components, optimized rendering
- **🎨 Sophisticated UX Design** — Emotion-driven UI adaptation, glassmorphism, cinematic backgrounds, smooth animations
- **🐍 Async Python Backend** — FastAPI with proper async/await patterns, efficient database access
- **☁️ Cloud Architecture** — Supabase RPC functions, Upstash Redis, Railway deployment, Vercel edge optimization
- **📱 Mobile-First Design** — Responsive layouts, touch optimization, safe area support, keyboard handling
- **♿ Accessibility Excellence** — WCAG AA compliance, keyboard navigation, screen reader support
- **🔒 Security Best Practices** — Private schema access, input validation, rate limiting, CORS protection
- **📊 Data Visualization** — Interactive charts, emotion timelines, pattern recognition
- **🔧 DevOps & Testing** — Comprehensive test suites, deployment automation, monitoring

---

## 👨‍💻 Creator

**Derril Filemon**  
*AI Engineer & Fullstack Developer*

📍 Goteborg, SWEDEN  
📧 [LinkedIn](https://www.linkedin.com/in/derril-filemon-a31715319) • [GitHub](https://github.com/derril-tech)

---

## 🙏 Acknowledgments

- **[OpenAI](https://openai.com/)** — GPT-4.1-mini API for emotion intelligence
- **[Supabase](https://supabase.com/)** — PostgreSQL database with RPC architecture
- **[Upstash](https://upstash.com/)** — Redis caching and job orchestration
- **[Railway](https://railway.app/)** — Backend deployment platform
- **[Vercel](https://vercel.com/)** — Frontend hosting with edge optimization
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful, accessible component library
- **[Recharts](https://recharts.org/)** — Powerful charting library
- **[Lucide](https://lucide.dev/)** — Beautiful icon library

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
# openai-emotion-aware-conversational-ui
