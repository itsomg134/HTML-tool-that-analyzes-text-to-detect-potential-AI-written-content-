# HTML-tool-that-analyzes-text-to-detect-potential-AI-written-content

# 🤖 AI Text Detector

A lightweight, client-side tool for analyzing text to detect potential AI-generated content. This tool uses pattern recognition and linguistic analysis to provide confidence scores on whether text was likely written by AI or humans.

![AI Text Detector Demo](https://img.shields.io/badge/demo-live-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![HTML](https://img.shields.io/badge/HTML-5-orange)
![CSS](https://img.shields.io/badge/CSS-3-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)

## ✨ Features

- **Real-time Analysis**: Instant detection results as you paste text
- **Visual Confidence Score**: Color-coded circular gauge showing AI likelihood (0-100%)
- **Multiple Indicators**: Analyzes 5 key linguistic patterns
- **No Server Required**: Runs entirely in the browser
- **Privacy-First**: All analysis happens locally, no data sent to servers
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Beautiful UI**: Modern gradient design with smooth animations

## 🔍 Detection Indicators

The tool analyzes text based on the following criteria:

1. **Sentence Length Consistency**: AI models often produce uniformly-sized sentences
2. **Common AI Phrases**: Detects overused expressions like "delve into," "leverage," "it's worth noting"
3. **Vocabulary Diversity**: Measures word repetition and uniqueness ratio
4. **Grammar Perfection**: Identifies unnaturally flawless writing patterns
5. **Transition Word Density**: Checks for excessive use of "however," "moreover," "therefore," etc.

## 🚀 Getting Started

### Prerequisites

No dependencies required! Just a modern web browser.

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-text-detector.git
```

2. Navigate to the project directory:
```bash
cd ai-text-detector
```

3. Open `index.html` in your browser:
```bash
open index.html
# or
start index.html
# or simply double-click the file
```

## 💻 Usage

1. **Paste Text**: Enter or paste text into the text area (minimum 50 characters)
2. **Click Analyze**: Press the "Analyze Text" button
3. **Review Results**: 
   - View the AI likelihood percentage
   - Check the color-coded verdict:
     - 🟢 **Green (0-39%)**: Likely human-written
     - 🟠 **Orange (40-69%)**: Possibly AI-generated
     - 🔴 **Red (70-100%)**: Likely AI-generated
   - Examine specific indicators that triggered detection

## 📊 How It Works

The detector uses a scoring system where each indicator contributes points to the total AI likelihood score:

- Uniform Sentence Length: +20 points
- Common AI Phrases (3+): +25 points
- High Word Repetition: +15 points
- Perfect Grammar: +20 points
- Excessive Transitions: +20 points

**Maximum Score**: 100%

## ⚠️ Limitations

This tool provides **estimates** and should not be considered definitive proof. Consider these limitations:

- Simple heuristic-based detection (not machine learning)
- Can produce false positives with formal academic writing
- May miss sophisticated AI-generated content
- Works best with English text over 200 characters
- Cannot detect AI content that has been heavily edited by humans

## 🛠️ Customization

### Adjusting Sensitivity

You can modify detection thresholds in the JavaScript code:

```javascript
// Adjust AI phrase threshold
if (phraseCount >= 3) { // Change this number
    aiScore += 25;
}

// Modify score interpretation
if (analysis.score >= 70) { // Change threshold
    verdict.textContent = 'Likely AI-Generated';
}
```

### Adding More AI Phrases

Expand the detection dictionary:

```javascript
const aiPhrases = [
    'it is important to note',
    'delve into',
    // Add your phrases here
];
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Ideas for Contribution

- Add support for multiple languages
- Implement machine learning-based detection
- Create browser extension version
- Add more linguistic indicators
- Improve UI/UX
- Write comprehensive tests

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by research on AI-generated text detection
- Built with vanilla JavaScript for maximum compatibility
- UI design inspired by modern web design trends

## 📧 Contact

Name: Om Gedam

GitHub: @itsomg134

Email: omgedam123098@gmail.com

Twitter (X): @omgedam

LinkedIn: Om Gedam

Portfolio: https://ogworks.lovable.app

## 🔮 Future Enhancements

- [ ] Multi-language support
- [ ] API endpoint for programmatic access
- [ ] Chrome/Firefox browser extension
- [ ] Integration with popular writing tools
- [ ] Machine learning model integration
- [ ] Batch text analysis
- [ ] Export reports as PDF
- [ ] Historical analysis tracking

---

⭐ **Star this repo** if you find it useful!
