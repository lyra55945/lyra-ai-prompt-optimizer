# 🚀 Lyra - AI Prompt Optimizer

Transform vague requests into precision-crafted prompts that unlock AI's full potential across all platforms.

![Lyra AI Prompt Optimizer](https://img.shields.io/badge/AI-Prompt%20Optimizer-blue)
![Next.js](https://img.shields.io/badge/Next.js-15.3.2-black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4.1.6-38B2AC)

## ✨ Features

- **4-D Methodology**: Deconstruct, Diagnose, Develop, Deliver
- **Multi-Platform Support**: ChatGPT, Claude, Gemini, and more
- **Real AI Integration**: Powered by OpenRouter API with GPT-4o
- **Modern UI**: Clean, responsive design with Tailwind CSS
- **Advanced Options**: Customizable system prompts
- **Copy-to-Clipboard**: Easy prompt sharing

## 🎯 The 4-D Methodology

1. **DECONSTRUCT** - Extract core intent, key entities, and context
2. **DIAGNOSE** - Audit for clarity gaps and ambiguity
3. **DEVELOP** - Apply optimization techniques based on request type
4. **DELIVER** - Construct precision-crafted final prompts

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- OpenRouter API key ([Get one here](https://openrouter.ai/keys))

### Installation

```bash
# Clone the repository
git clone <your-repo-url>
cd lyra-ai-optimizer

# Install dependencies
npm install

# Set up environment variables
cp .env.local.example .env.local
# Edit .env.local and add your OpenRouter API key

# Start development server
npm run dev
```

Visit `http://localhost:8000` to see Lyra in action!

## 🌐 Deploy to Production

### Option 1: Vercel (Recommended)

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/lyra-ai-optimizer)

1. Click the deploy button above
2. Connect your GitHub account
3. Add environment variable: `NEXT_PUBLIC_OPENROUTER_API_KEY`
4. Deploy!

### Option 2: Quick Deploy with Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Follow the prompts and add your API key when asked
```

### Option 3: Other Platforms

- **Netlify**: Connect GitHub repo, add env vars
- **Railway**: Auto-detects Next.js, just connect repo
- **DigitalOcean**: Use App Platform with GitHub integration

## 🔧 Configuration

### Environment Variables

```env
NEXT_PUBLIC_OPENROUTER_API_KEY=your_openrouter_api_key_here
```

### Supported AI Platforms

- **ChatGPT/GPT-4**: Structured sections, conversation starters
- **Claude**: Longer context, reasoning frameworks  
- **Gemini**: Creative tasks, comparative analysis
- **Others**: Universal best practices applied

## 🎨 Optimization Techniques

### Foundation Techniques
- Role assignment
- Context layering
- Output specifications
- Task decomposition

### Advanced Techniques
- Chain-of-thought reasoning
- Few-shot learning
- Multi-perspective analysis
- Constraint optimization

## 📱 Usage Examples

### Basic Mode
```
Input: "Write me a marketing email"
Output: Optimized prompt with clear structure and requirements
```

### Detail Mode
```
Input: "Help with my resume"
Output: Comprehensive prompt with clarifying questions and frameworks
```

## 🛡️ Security Notes

- API key is exposed in frontend (NEXT_PUBLIC_)
- For production, consider implementing backend API routes
- Monitor API usage to prevent abuse
- Set up rate limiting if needed

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Next.js](https://nextjs.org/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)
- UI components from [shadcn/ui](https://ui.shadcn.com/)
- AI powered by [OpenRouter](https://openrouter.ai/)

---

**Made with ❤️ for AI enthusiasts and professionals**
