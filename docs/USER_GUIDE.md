# 📖 User Guide - Automate

Welcome to Automate! This guide will help you get started with AI-powered web automation.

## Table of Contents

- [Getting Started](#getting-started)
- [Basic Usage](#basic-usage)
- [Advanced Features](#advanced-features)
- [Command Examples](#command-examples)
- [Troubleshooting](#troubleshooting)
- [Tips & Best Practices](#tips--best-practices)

---

## Getting Started

### Installation

1. **Install the Extension**
   - From Chrome Web Store (coming soon)
   - Or load unpacked from the `dist/` folder

2. **Configure Your API Key**
   - Click the Automate icon in your Chrome toolbar
   - Go to Settings (gear icon)
   - Select your preferred LLM provider
   - Enter your API key
   - Save settings

### Supported LLM Providers

- **OpenAI**: GPT-4, GPT-4 Turbo, GPT-3.5 Turbo
- **Anthropic**: Claude 3.5 Sonnet, Claude 3 Opus, Claude 3 Haiku
- **Google**: Gemini Pro, Gemini Ultra
- **Ollama**: Run local models (llama2, mistral, etc.)
- **OpenRouter**: Access to multiple models

---

## Basic Usage

### Opening Automate

1. Click the Automate icon in your Chrome toolbar
2. The side panel will open on the right side of your browser
3. Type your command in the chat interface

### Simple Commands

```plaintext
"Click the login button"
"Fill in the email field with john@example.com"
"Go to the pricing page"
"Submit this form"
```

### Natural Language

Automate understands natural language, so you can be conversational:

```plaintext
"Can you find the contact form and fill it out?"
"I need to search for 'AI tools' on this page"
"Please extract all the prices from this page"
```

---

## Advanced Features

### Multi-Step Automation

You can chain multiple actions together:

```plaintext
"Search for 'Chrome extensions' in the search bar, 
then click on the first result, 
and extract all the headings"
```

### Data Extraction

Extract structured data from web pages:

```plaintext
"Get me all the product names and prices from this page"
"Extract all email addresses and phone numbers"
"Find all links in the navigation menu"
```

### Form Automation

Automate can handle complex forms:

```plaintext
"Fill out this contact form with:
Name: John Doe
Email: john@example.com
Message: I'd like to learn more about your services"
```

### Navigation

Navigate through websites intelligently:

```plaintext
"Go to the checkout page"
"Find and click the 'About Us' link"
"Scroll down to the footer"
"Open the menu and go to Settings"
```

---

## Command Examples

### E-commerce

```plaintext
✓ "Add this product to my cart"
✓ "Find the cheapest laptop on this page"
✓ "Compare the prices of all listed items"
✓ "Apply the discount code SAVE20"
```

### Research & Data Collection

```plaintext
✓ "Extract all article titles from this news site"
✓ "Get the author names from all blog posts"
✓ "Find all download links on this page"
✓ "Create a list of all companies mentioned in this article"
```

### Social Media

```plaintext
✓ "Like the first 5 posts"
✓ "Follow users who commented on this post"
✓ "Extract all hashtags from this page"
```

### Productivity

```plaintext
✓ "Fill out this job application with my resume data"
✓ "Schedule a meeting for next Tuesday at 2pm"
✓ "Download all PDF files from this page"
```

---

## Troubleshooting

### Common Issues

**"API Key Invalid" Error**
- Double-check your API key in Settings
- Ensure you have credits/quota with your provider
- Verify the key has the correct permissions

**"Element Not Found" Error**
- Wait for the page to fully load before issuing commands
- Try being more specific in your description
- Some elements may be hidden or require scrolling

**Extension Not Responding**
- Refresh the page and try again
- Check the browser console for errors (F12)
- Restart Chrome if issues persist

**Rate Limiting**
- Your LLM provider may have rate limits
- Wait a moment between commands
- Consider upgrading your API plan

### Debugging

Enable debug mode in Settings to see detailed logs:
1. Open Automate Settings
2. Enable "Debug Mode"
3. Check the browser console (F12) for detailed information

---

## Tips & Best Practices

### 🎯 Be Specific

**Good**: "Click the blue 'Submit' button at the bottom of the form"  
**Better**: "Click the submit button"

### ⏱️ Wait for Page Loads

Always ensure the page has fully loaded before issuing commands. Automate will wait, but complex pages may need extra time.

### 🔄 Break Down Complex Tasks

For very complex automations, break them into smaller steps:

1. Navigate to the page
2. Fill out the form
3. Verify the data
4. Submit

### 💾 Save Frequent Commands

You can save frequently used commands:
- Click the star icon next to your command
- Access saved commands from the quick menu

### 🔒 Security

- Never share your API keys
- Be cautious when automating sensitive operations
- Review actions before automation on important pages

### ⚡ Performance

- Close unused tabs to improve performance
- Clear browser cache if experiencing slowdowns
- Use simpler commands when possible

---

## Keyboard Shortcuts

- `Ctrl/Cmd + Enter` - Execute command
- `Ctrl/Cmd + K` - Focus command input
- `Esc` - Close side panel
- `Ctrl/Cmd + /` - Show command history

---

## Getting Help

- **Documentation**: See our [full documentation](https://github.com/yourusername/automate/wiki)
- **Issues**: Report bugs on [GitHub Issues](https://github.com/yourusername/automate/issues)
- **Community**: Join our [Discord server](#)
- **Email**: Contact support@automate.example.com

---

## Next Steps

- Explore [Advanced Automation Techniques](docs/ADVANCED.md)
- Learn about the [Multi-Agent System](AGENTS.md)
- Check out [Example Scripts](docs/EXAMPLES.md)
- Read the [API Documentation](docs/API.md)

---

Happy Automating! 🤖✨
