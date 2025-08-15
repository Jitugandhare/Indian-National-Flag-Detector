# 🇮🇳 Indian National Flag Detector

A web-based tool to validate Indian national flag images against Bureau of Indian Standards (BIS) specifications. This application checks aspect ratio, colors, stripe proportions, and Ashoka Chakra details to ensure flag compliance.

## 🌐 Live Demo

**[Try it here](https://lustrous-truffle-0f84b0.netlify.app/)**

## 📋 Features

- **🖼️ Image Upload**: Drag & drop or browse to upload flag images
- **📏 Aspect Ratio Validation**: Checks if flag dimensions meet 3:2 ratio requirement
- **🎨 Color Accuracy**: Validates saffron, white, green, and chakra blue colors
- **📐 Stripe Proportions**: Ensures equal thirds for the three horizontal bands
- **⚫ Chakra Analysis**: Validates Ashoka Chakra position and spoke count (24 spokes)
- **📊 Detailed Results**: Comprehensive validation report with pass/fail indicators
- **📱 Responsive Design**: Works seamlessly on desktop and mobile devices

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with modern design principles
- **Image Processing**: HTML5 Canvas API for pixel analysis
- **Deployment**: Netlify
- **No external dependencies or frameworks**

## 🚀 Getting Started

### Prerequisites
- Modern web browser with JavaScript enabled
- No additional software installation required

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Jitugandhare/Indian-National-Flag-Detector.git
   cd Indian-National-Flag-Detector
   ```

2. **Open in browser**
   - Simply open `index.html` in any modern web browser
   - Or use a local development server

3. **Local Development Server** (Optional)
   ```bash
   # Using Node.js
   npx serve .
   
   # Using JavaScript (if you have Node.js installed)
   node -e "require('http').createServer((req, res) => { require('fs').readFile('.' + req.url, (err, data) => { res.writeHead(200, {'Content-Type': 'text/html'}); res.end(data || require('fs').readFileSync('./index.html')); }); }).listen(8000, () => console.log('Server running at http://localhost:8000/'));"
   ```

## 📖 Usage

1. **Upload Image**: Drag and drop a flag image or click to browse
2. **Supported Formats**: PNG, JPG, SVG (Max file size: 5MB)
3. **Click Validate**: Analyze the uploaded flag image
4. **Review Results**: Check detailed validation report for each criterion

## 🔍 Validation Criteria

### Aspect Ratio
- **Required**: 3:2 (1.50)
- **Tolerance**: Configurable deviation allowance

### Colors (RGB Values)
- **Saffron (Top)**: Deep saffron orange
- **White (Middle)**: Pure white
- **Green (Bottom)**: India green
- **Chakra Blue**: Navy blue for Ashoka Chakra

### Stripe Proportions
- **Equal thirds**: Each horizontal band should be 1/3 of total height

### Ashoka Chakra
- **Position**: Centered on white band
- **Spokes**: Exactly 24 spokes
- **Color**: Navy blue

## 🏗️ Project Structure

```
Indian-National-Flag-Detector/
├── index.html          # Main application file (HTML + CSS + JavaScript)
├── README.md           # Project documentation
└── .gitignore          # Git ignore file
```

## 🔧 Customization

### Modifying BIS Specifications
Edit the `BIS_SPECS` object in the JavaScript code to adjust:
- Color tolerances
- Aspect ratio requirements
- Validation thresholds

### Adding New Validation Rules
Extend the `runValidation()` function to include additional checks:
```javascript
function runValidation() {
    const results = {
        // Existing validations...
        new_validation: checkNewValidation()
    };
    return results;
}
```

## 🌟 Key Features

- **Real-time Analysis**: Instant validation results
- **Visual Feedback**: Color-coded pass/fail indicators
- **Progress Animation**: Loading states with progress bars
- **Error Handling**: Graceful error messages for invalid files
- **Cross-browser Compatibility**: Works on all modern browsers

## 🚀 Deployment

### Netlify (Current)
- **URL**: https://lustrous-truffle-0f84b0.netlify.app/
- **Automatic deployment** from GitHub repository

### Other Platforms
- **GitHub Pages**: Enable in repository settings
- **Vercel**: Connect repository for automatic deployment
- **Firebase Hosting**: Deploy using Firebase CLI

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Jitu Gandhare**
- GitHub: [@Jitugandhare](https://github.com/Jitugandhare)
- Project: [Indian National Flag Detector](https://github.com/Jitugandhare/Indian-National-Flag-Detector)

## 🙏 Acknowledgments

- Bureau of Indian Standards (BIS) for flag specifications
- Indian Constitution for flag design guidelines
- Open source community for inspiration and tools

## 📞 Support

If you have any questions or suggestions:
- Open an [issue](https://github.com/Jitugandhare/Indian-National-Flag-Detector/issues)
- Star the repository if you find it helpful
- Share with others who might benefit from this tool

---

**Made with ❤️ for India** 🇮🇳
