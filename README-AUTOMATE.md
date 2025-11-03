# 🤖 Automate - AI Web Agent & Automation

<div align="center">

![Automate Logo](chrome-extension/public/icon-128.png)

**Open-source AI-powered Chrome extension for intelligent web automation**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Chrome Web Store](https://img.shields.io/badge/Chrome-Extension-blue?logo=google-chrome)](https://chrome.google.com/webstore)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5-blue?logo=typescript)](https://www.typescriptlang.org/)

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Development](#-development) • [Contributing](#-contributing)

</div>

---

## 🌟 Overview

**Automate** is a powerful, open-source Chrome extension that brings AI-driven automation to your browser. Built with a sophisticated multi-agent system, Automate can understand natural language commands and execute complex web tasks autonomously.

### Why Automate?

- 🆓 **100% Free & Open Source** - No hidden costs, full transparency
- 🔒 **Privacy-First** - All processing happens locally in your browser
- 🧠 **Multi-LLM Support** - Works with OpenAI, Anthropic, Google Gemini, Ollama, and more
- 🎯 **Smart Automation** - Intelligent task planning and execution
- 🛠️ **Developer-Friendly** - Built with modern web technologies and extensible architecture

---

## ✨ Features

### 🎭 Multi-Agent Intelligence

Automate uses a specialized multi-agent system for sophisticated task execution:

- **🧭 Navigator Agent** - Handles DOM interactions and web navigation
- **📋 Planner Agent** - Creates high-level task strategies and breakdowns
- **✅ Validator Agent** - Ensures task completion and validates results

### 🚀 Core Capabilities

- **Natural Language Control** - Just describe what you want to do
- **Complex Workflow Automation** - Chain multiple actions together
- **Form Filling** - Automatically fill out web forms
- **Data Extraction** - Scrape and extract information from websites
- **Cross-Page Navigation** - Navigate through multiple pages seamlessly
- **Visual Element Detection** - Identify and interact with page elements
- **Error Recovery** - Intelligent handling of failures and retries

### 🔌 LLM Provider Support

Choose your preferred AI provider:

- OpenAI (GPT-4, GPT-3.5)
- Anthropic Claude (Claude 3.5 Sonnet, Opus, Haiku)
- Google Gemini (Gemini Pro, Ultra)
- Ollama (Local models)
- OpenRouter (Access to multiple models)
- Custom API endpoints

---

## 📦 Installation

### From Chrome Web Store (Recommended)

1. Visit the [Chrome Web Store](#) (coming soon)
2. Click "Add to Chrome"
3. Configure your AI provider API key in the extension settings

### Manual Installation (Development)

```bash
# Clone the repository
git clone https://github.com/yourusername/automate.git
cd automate

# Install dependencies (requires Node.js >=22.12.0)
pnpm install

# Build the extension
pnpm build

# Load in Chrome
# 1. Navigate to chrome://extensions/
# 2. Enable "Developer mode"
# 3. Click "Load unpacked"
# 4. Select the `dist/` directory
```

---

## 🎯 Usage

### Quick Start

1. **Click the Automate icon** in your Chrome toolbar
2. **Enter your API key** for your preferred LLM provider
3. **Start automating!** Type natural language commands like:
   - "Fill out this contact form with my details"
   - "Find all product prices on this page"
   - "Navigate to the checkout page"
   - "Extract all email addresses from this page"

### Example Commands

```
📝 Form Automation
"Fill in the name field with 'John Doe'"
"Submit this form"
"Select 'United States' from the country dropdown"

🔍 Data Extraction
"Get all article titles from this page"
"Extract the pricing information"
"Find all links in the navigation menu"

🌐 Navigation
"Go to the pricing page"
"Click the 'Learn More' button"
"Scroll to the footer section"

🔗 Multi-Step Tasks
"Search for 'AI automation tools' and open the first result"
"Add this product to cart and proceed to checkout"
```

---

## 🛠️ Development

### Tech Stack

- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite + Turbo (monorepo)
- **Styling**: Tailwind CSS
- **AI Integration**: LangChain.js
- **Browser APIs**: Chrome Extension Manifest V3
- **Testing**: Vitest + Puppeteer

### Project Structure

```
automate/
├── chrome-extension/      # Main extension code
│   ├── src/background/    # Background service worker
│   │   ├── agent/         # Multi-agent system
│   │   └── browser/       # Browser automation
│   └── manifest.js        # Extension manifest
├── pages/
│   ├── side-panel/        # Main UI (React)
│   ├── options/           # Settings page
│   └── content/           # Content scripts
├── packages/              # Shared packages
│   ├── ui/                # React components
│   ├── storage/           # Chrome storage wrapper
│   ├── i18n/              # Internationalization
│   └── shared/            # Common utilities
└── docs/                  # Documentation
```

### Development Commands

```bash
# Install dependencies
pnpm install

# Start development mode (hot reload)
pnpm dev

# Build for production
pnpm build

# Run type checking
pnpm type-check

# Run linter
pnpm lint

# Run tests
pnpm test

# Run end-to-end tests
pnpm e2e

# Create distribution zip
pnpm zip
```

### Adding New Features

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes** following our [coding standards](CONTRIBUTING.md)
4. **Test thoroughly**: `pnpm test && pnpm type-check`
5. **Submit a pull request**

---

## 🤝 Contributing

We love contributions! Please read our [Contributing Guide](CONTRIBUTING.md) to learn about our development process and how to propose bugfixes and improvements.

### Ways to Contribute

- 🐛 Report bugs and issues
- 💡 Suggest new features
- 📝 Improve documentation
- 🔧 Submit pull requests
- ⭐ Star the project
- 🗣️ Spread the word

### Code of Conduct

This project adheres to a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

---

## 📚 Documentation

- [User Guide](docs/USER_GUIDE.md) - Complete usage instructions
- [API Documentation](docs/API.md) - Developer API reference
- [Architecture Overview](docs/ARCHITECTURE.md) - System design and structure
- [Agent System](docs/AGENTS.md) - Multi-agent implementation details
- [Privacy Policy](PRIVACY.md) - How we handle your data
- [Security](SECURITY.md) - Security policies and reporting

---

## 🔐 Privacy & Security

- **No Data Collection** - We don't collect or store any user data
- **Local Processing** - All automation runs in your browser
- **API Key Security** - Your API keys are stored locally and never transmitted to our servers
- **Open Source** - Fully auditable codebase

Read our full [Privacy Policy](PRIVACY.md) and [Security Policy](SECURITY.md).

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🌐 Community & Support

- **GitHub Issues** - [Report bugs or request features](https://github.com/yourusername/automate/issues)
- **Discussions** - [Ask questions and share ideas](https://github.com/yourusername/automate/discussions)
- **Discord** - Join our community server (coming soon)
- **Twitter** - Follow [@AutomateAI](#) for updates

---

## 🙏 Acknowledgments

Built with ❤️ by the open-source community.

Special thanks to:
- [LangChain](https://github.com/langchain-ai/langchainjs) - For AI/LLM integration
- [Chrome Extensions](https://developer.chrome.com/docs/extensions/) - For the extension platform
- All our [contributors](https://github.com/yourusername/automate/graphs/contributors)

---

## 🗺️ Roadmap

- [ ] Firefox extension support
- [ ] Visual workflow builder
- [ ] Task recording and playback
- [ ] Cloud sync for automation scripts
- [ ] Browser extension marketplace
- [ ] Advanced scheduling capabilities
- [ ] Team collaboration features
- [ ] Mobile app companion

---

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/automate?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/automate?style=social)
![GitHub issues](https://img.shields.io/github/issues/yourusername/automate)
![GitHub pull requests](https://img.shields.io/github/issues-pr/yourusername/automate)

---

<div align="center">

**[⬆ Back to Top](#-automate---ai-web-agent--automation)**

Made with 🤖 by developers, for developers

</div>
