# 📄 Google Docs to Overleaf LaTeX Converter

A powerful web-based tool that converts Google Docs (`.docx` files) into professional LaTeX projects ready for Overleaf. No installation required - just open the HTML file in your browser!

![Converter Interface](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)


## 🌟 Features

### Multiple Academic Formats
- **📖 Dissertation/Thesis** - Complete PhD dissertation with chapters, frontmatter, and backmatter
- **📊 IEEE Conference Paper** - Standard IEEE two-column format
- **📄 Academic Article** - Clean journal article layout
- **📝 Technical Report** - Professional report with executive summary

### Smart Conversion
- ✅ Automatic document structure detection
- ✅ LaTeX-formatted tables
- ✅ Image extraction and inclusion
- ✅ Bibliography generation
- ✅ Proper cross-referencing setup
- ✅ Sample content and placeholders

### User-Friendly Interface
- 🎨 Beautiful gradient UI
- 📤 Drag & drop file upload
- 👁️ Real-time LaTeX preview
- 💾 One-click download as ZIP
- 📱 Responsive design

## 🚀 Quick Start

### Method 1: Download and Use (Easiest)

1. **Download the tool:**
   - Click the green "Code" button above
   - Select "Download ZIP"
   - Extract the ZIP file

2. **Open the converter:**
   - Navigate to the extracted folder
   - Double-click `gdocs-to-overleaf.html`
   - The tool opens in your default browser

3. **Convert your document:**
   - Upload your `.docx` file (from Google Docs → File → Download → Microsoft Word)
   - Select your desired format
   - Click "Convert to LaTeX"
   - Download the Overleaf package

4. **Import to Overleaf:**
   - Go to [Overleaf](https://www.overleaf.com)
   - Click "New Project" → "Upload Project"
   - Upload the downloaded ZIP file
   - Click on `main.tex` and compile!


### Method 2: Host Locally

```bash
# Clone the repository
git clone https://github.com/kcl17/DOCX_TO_LATEX.git

# Navigate to the folder
cd DOCX_TO_LATEX

# Open with any browser
# On Windows:
start gdocs-to-overleaf.html

# On Mac:
open gdocs-to-overleaf.html

# On Linux:
xdg-open gdocs-to-overleaf.html
```

## 📋 How It Works

### Step-by-Step Process

1. **Export from Google Docs:**
   - Open your Google Doc
   - File → Download → Microsoft Word (.docx)
   - Save the file to your computer

2. **Upload to Converter:**
   - Drag & drop the `.docx` file, or
   - Click "Choose File" to browse

3. **Select Format:**
   - Choose from: Dissertation, IEEE, Article, or Report
   - Toggle conversion options as needed

4. **Convert:**
   - Click "Convert to LaTeX"
   - Preview the generated LaTeX code
   - Review the structure

5. **Download Package:**
   - Click "Download Overleaf Package"
   - Get a complete ZIP file with all necessary files

6. **Upload to Overleaf:**
   - Create new project on Overleaf
   - Upload the ZIP file
   - Compile and edit!

## 📦 What You Get

### Dissertation Format Structure
```
overleaf_dissertation_[timestamp].zip
├── main.tex                    # Main compilation file
├── bibliography.bib            # References database
├── README.md                   # Project documentation
├── frontmatter/
│   ├── titlepage.tex          # University title page
│   ├── declaration.tex        # Declaration page
│   ├── acknowledgements.tex   # Acknowledgements
│   └── abstract.tex           # Abstract with keywords
├── chapters/
│   ├── chapter1_introduction.tex
│   ├── chapter2_literature_review.tex
│   ├── chapter3_methodology.tex
│   ├── chapter4_results.tex
│   ├── chapter5_discussion.tex
│   └── chapter6_conclusion.tex
├── backmatter/
│   └── appendix_a.tex         # Appendices
├── figures/                    # Place images here
└── tables/                     # Table data
```

### IEEE Conference Format
```
overleaf_ieee_[timestamp].zip
├── main.tex                    # Complete conference paper
├── figures/                    # Images directory
└── README.md                   # Instructions
```

### Other Formats
Similar structure optimized for each format type.

## 🎯 Supported Formats

| Format | Use Case | Key Features |
|--------|----------|--------------|
| **Dissertation** | PhD Thesis, Master's Thesis | Full frontmatter, 6 chapters, appendices, bibliography |
| **IEEE Conference** | Conference Papers | Two-column, IEEE style, compact format |
| **Academic Article** | Journal Papers | Abstract, keywords, standard sections |
| **Technical Report** | Industry Reports | Executive summary, recommendations |

## ⚙️ Conversion Options

- **Include LaTeX Comments** - Adds helpful hints throughout the code
- **Extract Images** - Prepares image placeholders and includes
- **Convert Tables** - Transforms tables to LaTeX format
- **Generate Bibliography** - Creates sample `.bib` file with entries

## 🔧 Technical Details

### Technologies Used
- Pure HTML5, CSS3, JavaScript
- [Mammoth.js](https://github.com/mwilliamson/mammoth.js) - DOCX parsing
- [JSZip](https://stuk.github.io/jszip/) - ZIP file creation
- [FileSaver.js](https://github.com/eligrey/FileSaver.js) - File downloads

### Browser Compatibility
- ✅ Chrome/Edge (Recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

### File Requirements
- Input: `.docx` files (Microsoft Word format)
- Output: `.zip` file containing LaTeX project

## 📖 Usage Examples

### Example 1: PhD Dissertation
```
1. Write your dissertation in Google Docs
2. Download as .docx
3. Upload to converter
4. Select "Dissertation" format
5. Enable all conversion options
6. Convert and download
7. Upload to Overleaf
8. Customize chapter content
9. Add your figures to figures/
10. Update bibliography.bib
11. Compile!
```

### Example 2: IEEE Conference Paper
```
1. Write your paper in Google Docs
2. Download as .docx
3. Upload to converter
4. Select "IEEE Conference" format
5. Convert and download
6. Upload to Overleaf
7. Fill in author information
8. Add experimental results
9. Update references
10. Compile!
```

## 🎨 Customization

### Modifying Templates
The converter generates standard LaTeX templates. After conversion, you can:

- Adjust margins in `\geometry{}` settings
- Change fonts and sizes
- Modify chapter titles
- Add/remove sections
- Update bibliography style
- Customize headers/footers

### Adding Your Content
1. Replace placeholder text with your actual content
2. Add images to `figures/` directory
3. Update `bibliography.bib` with real references
4. Adjust formatting as needed

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch:** `git checkout -b feature/AmazingFeature`
3. **Commit your changes:** `git commit -m 'Add some AmazingFeature'`
4. **Push to the branch:** `git push origin feature/AmazingFeature`
5. **Open a Pull Request**

### Ideas for Contributions
- Add more format templates (ACM, Springer, etc.)
- Improve document parsing
- Better image handling
- Style customization options
- Dark mode support
- Multi-language support

## 🐛 Known Issues & Limitations

- Complex tables may need manual adjustment
- Equations are converted as plain text (need manual LaTeX formatting)
- Advanced Word formatting might not convert perfectly
- Images are referenced but need to be manually added to the project
- Best results with simple, well-structured documents

## 📝 Tips for Best Results

1. **Structure your Google Doc clearly:**
   - Use heading styles (Heading 1, 2, 3)
   - Keep formatting simple
   - One space between paragraphs

2. **Before converting:**
   - Check for special characters
   - Verify table structure
   - Note image locations

3. **After converting:**
   - Review generated LaTeX
   - Test compile on Overleaf
   - Adjust spacing and formatting
   - Add real images
   - Update bibliography

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Mammoth.js](https://github.com/mwilliamson/mammoth.js) for DOCX parsing
- [JSZip](https://stuk.github.io/jszip/) for ZIP generation
- [FileSaver.js](https://github.com/eligrey/FileSaver.js) for file downloads
- LaTeX community for format standards

## 📧 Support

- 🐛 **Bug Reports:** Open an issue on GitHub
- 💡 **Feature Requests:** Open an issue with the "enhancement" label
- 📖 **Documentation:** Check the wiki (if available)
- ❓ **Questions:** Open a discussion on GitHub

## 🔗 Useful Links

- [Overleaf](https://www.overleaf.com) - Online LaTeX editor
- [LaTeX Documentation](https://www.latex-project.org/help/documentation/)
- [CTAN](https://www.ctan.org) - Comprehensive TeX Archive Network
- [IEEE LaTeX Guide](https://www.ieee.org/conferences/publishing/templates.html)

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/[your-username]/[repo-name]?style=social)
![GitHub forks](https://img.shields.io/github/forks/[your-username]/[repo-name]?style=social)
![GitHub issues](https://img.shields.io/github/issues/[your-username]/[repo-name])

---

**Made with ❤️ for the academic community**

*Star ⭐ this repository if you find it helpful!*