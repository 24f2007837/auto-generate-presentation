# Auto-Generate Presentation 📊

Transform your text into professional PowerPoint presentations using AI and custom templates.

[![Demo](https://img.shields.io/badge/Demo-Live%20App-blue)](https://presentation-generator-ai.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## ✨ Features

- **Smart Text Analysis**: AI intelligently breaks down your text into logical slide structures
- **Template Integration**: Extracts and applies styles, colors, fonts, and images from your PowerPoint templates
- **Multiple AI Providers**: Supports OpenAI GPT-4, Anthropic Claude, and Google Gemini
- **Custom Guidance**: Optional tone and structure guidance for your presentation
- **Secure Processing**: API keys are never stored or logged
- **Professional Output**: Generates complete .pptx files ready for use

## 🚀 Quick Start

### Online Demo
Visit the [live demo](https://presentation-generator-ai.vercel.app) - no installation required!

### Local Development

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/auto-generate-presentation.git
cd auto-generate-presentation
```

2. **Open in browser**
```bash
# Simply open index.html in your web browser
open index.html
# or
python -m http.server 8000  # for local server
```

That's it! The app runs entirely in the browser with no backend required.

## 📖 Usage

1. **Prepare Your Content**
   - Paste your text, markdown, or prose into the input area
   - Add optional guidance (e.g., "make it an investor pitch deck")

2. **Configure AI**
   - Select your preferred AI provider (OpenAI, Anthropic, or Google)
   - Enter your API key (get one from [OpenAI](https://platform.openai.com/api-keys), [Anthropic](https://console.anthropic.com/), or [Google AI](https://makersuite.google.com/app/apikey))

3. **Upload Template**
   - Upload a PowerPoint template (.pptx or .potx file)
   - The app will extract styles, colors, and images from your template

4. **Generate**
   - Click "Generate Presentation"
   - Wait for AI processing (usually 30-60 seconds)
   - Download your generated presentation

## 🛠️ Technical Details

### Architecture
- **Frontend-Only**: Pure HTML/CSS/JavaScript with no backend required
- **AI Integration**: Direct API calls to OpenAI, Anthropic, or Google
- **File Processing**: Client-side PowerPoint manipulation using JSZip
- **Security**: API keys processed in-browser only, never transmitted to our servers

### Dependencies
- [JSZip](https://stuk.github.io/jszip/) - PowerPoint file manipulation
- [FileSaver.js](https://github.com/eligrey/FileSaver.js/) - File download functionality

### Browser Support
- Chrome 60+ (recommended)
- Firefox 55+
- Safari 12+
- Edge 79+

## 🎯 How It Works

### Text Analysis & Slide Mapping
The application uses advanced AI models to parse and structure your input text:

1. **Content Analysis**: AI identifies main topics, subtopics, and key points
2. **Slide Structure**: Creates logical hierarchy (title slides, content slides, section headers)
3. **Content Distribution**: Optimally distributes content across 5-12 slides based on volume
4. **Speaker Notes**: Generates helpful speaker notes for each slide

### Template Style Application
The app preserves your brand identity by:

1. **Theme Extraction**: Parses theme XML to extract color schemes and fonts
2. **Asset Reuse**: Identifies and reuses images from the template's media folder
3. **Style Inheritance**: Applies extracted colors and fonts to generated content
4. **Layout Preservation**: Maintains template layout structures where possible

## 🔧 Configuration

### API Keys
You'll need an API key from one of these providers:

- **OpenAI**: [Get API Key](https://platform.openai.com/api-keys) - Uses GPT-4 model
- **Anthropic**: [Get API Key](https://console.anthropic.com/) - Uses Claude 3 Sonnet
- **Google AI**: [Get API Key](https://makersuite.google.com/app/apikey) - Uses Gemini Pro

### Supported File Formats
- **Input**: Plain text, Markdown, or any prose
- **Templates**: .pptx or .potx PowerPoint files
- **Output**: Standard .pptx PowerPoint files

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Limitations

- **File Size**: Recommended max template size of 50MB
- **API Costs**: You pay for your own AI API usage
- **Internet Required**: Needs internet connection for AI processing
- **Modern Browsers**: Requires recent browser with ES6+ support

## 🆘 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/auto-generate-presentation/issues)
- **Documentation**: This README and inline code comments
- **Examples**: Check the `/examples` folder for sample templates and input text

## 🏆 Acknowledgments

- OpenAI for GPT-4 API
- Anthropic for Claude API  
- Google for Gemini API
- JSZip library for PowerPoint file handling
- The open-source community for inspiration and tools

---

**Made with ❤️ for better presentations**