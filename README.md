# ConvertFlow - Universal Document Suite

A powerful client-side document conversion tool that transforms multiple file formats into unified PDF or Word documents with zero server dependencies.

## 🚀 Live Demo
**URL**: https://asankhua.github.io/ConvertFlow-PDF-Doc-Generator/

## ✨ Key Features

### 📁 File Support
- **Images**: All image formats (JPG, PNG, GIF, SVG, WebP, etc.)
- **Documents**: TXT, DOCX, DOC, JSON, JS, HTML, CSS, TS, TSX, PY, Java, C++
- **Spreadsheets**: XLSX, XLS, CSV
- **PDF**: PDF files (for PDF merging only)

### 🎯 Core Capabilities
- **Multi-format Conversion**: Convert various file types to PDF or DOCX
- **PDF Merging**: Combine multiple PDFs into a single document
- **Drag & Drop Interface**: Intuitive file management
- **File Reordering**: Drag handles to arrange files before conversion
- **Theme Customization**: Dark/Light modes with 5 accent color themes
- **Smart Validation**: Prevents incompatible conversions (e.g., PDF to DOCX)
- **100% Client-side**: All processing happens locally in your browser
- **Privacy First**: No server uploads, complete data security

### 🎨 User Experience
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Real-time Progress**: Detailed progress indicators during conversion
- **Error Handling**: Graceful error messages with specific feedback
- **Modern UI**: Clean, professional interface with smooth animations
- **Accessibility**: ARIA labels and keyboard navigation support

## 🛠️ Technology Stack

### Frontend Framework
- **React 18.2.0** - Modern UI framework with hooks
- **Tailwind CSS** - Utility-first CSS framework
- **Babel Standalone** - In-browser JSX compilation

### External Libraries
- **jsPDF 2.5.1** - PDF generation and manipulation
- **docx 7.8.2** - Word document creation
- **mammoth 1.6.0** - DOCX text extraction
- **XLSX 0.18.5** - Excel/CSV processing
- **Lucide React 0.292.0** - Icon library

### Development Tools
- **ES Modules** - Modern JavaScript module system
- **Dynamic Script Loading** - On-demand library loading
- **Thread Yielding** - Prevents UI freezing on large files

## 📋 Supported Formats

### Input Formats
| Category | Formats |
|----------|---------|
| **Images** | JPG, JPEG, PNG, GIF, SVG, WebP, BMP, TIFF, ICO, HEIC, HEIF |
| **Documents** | TXT, DOCX, DOC, JSON, JS, HTML, CSS, TS, TSX, PY, Java, C++ |
| **Spreadsheets** | XLSX, XLS, CSV |
| **PDF** | PDF (for merging only) |

### Output Formats
- **PDF Document** - Universal format with full compatibility
- **Word Document (DOCX)** - Editable Microsoft Word format

## 🚀 Quick Start

1. **Visit**: [ConvertFlow Live Demo](https://asankhua.github.io/ConvertFlow-PDF-Doc-Generator/)
2. **Upload Files**: Drag & drop or click to select files
3. **Configure**: Choose output format and page orientation
4. **Convert**: Click generate button to create unified document
5. **Download**: Automatic download of converted document

## 🏗️ Architecture

### Client-Only Architecture
```
┌─────────────────────────────────────────────────────────────┐
│                    Browser Environment                     │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────────┐  ┌─────────────────┐  ┌──────────────┐ │
│  │   React App     │  │   File Manager  │  │   Converter  │ │
│  │                 │  │                 │  │              │ │
│  │ • UI Components │  │ • Drag & Drop   │  │ • PDF Engine │ │
│  │ • State Mgmt    │  │ • File Queue    │  │ • DOCX Engine│ │
│  │ • Theme System  │  │ • Validation    │  │ • Processing │ │
│  └─────────────────┘  └─────────────────┘  └──────────────┘ │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────────┐  ┌─────────────────┐  ┌──────────────┐ │
│  │   PDF Library   │  │   DOCX Library  │  │   Utils      │ │
│  │   (jsPDF)       │  │   (docx)        │  │              │ │
│  │ • Generation    │  │ • Creation      │  │ • Text Ext.  │ │
│  │ • Merging       │  │ • Formatting    │  │ • Excel Proc │ │
│  │ • Styling       │  │ • Layout        │  │ • Error Hdl  │ │
│  └─────────────────┘  └─────────────────┘  └──────────────┘ │
└─────────────────────────────────────────────────────────────┘
```

### Data Flow
1. **File Input** → Validation → Queue Management
2. **Content Extraction** → Format-specific processing
3. **Document Assembly** → Layout and formatting
4. **Export Generation** → Download delivery

## 🔧 Configuration Options

### Export Settings
- **Output Format**: PDF or DOCX
- **Page Orientation**: Portrait or Landscape
- **Page Size**: A4 (default)

### Theme Options
- **Dark/Light Mode**: Toggle between themes
- **Accent Colors**: Indigo, Emerald, Rose, Amber, Cyan
- **Custom Styling**: Consistent color theming throughout

## 🔒 Security & Privacy

### Data Protection
- **100% Client-side Processing**: No server uploads
- **Local File Handling**: Files never leave your browser
- **Memory Management**: Automatic cleanup of file previews
- **Secure Libraries**: All dependencies from trusted CDNs

### Privacy Features
- **No Tracking**: No analytics or tracking scripts
- **No Data Collection**: Zero user data collection
- **Temporary Processing**: Files processed in memory only
- **Secure Connection**: HTTPS for all external resources

## 🌐 Browser Compatibility

### Supported Browsers
- **Chrome/Chromium**: 90+
- **Firefox**: 88+
- **Safari**: 14+
- **Edge**: 90+

### Required Features
- **ES6 Modules**: Modern JavaScript support
- **File API**: Local file access
- **Blob API**: File generation
- **Canvas API**: Image processing

## 📝 Usage Examples

### Basic Conversion
```javascript
// Files are automatically processed when user clicks generate
// No coding required - everything handled by the UI
```

### Advanced Features
- **Batch Processing**: Convert multiple files simultaneously
- **PDF Merging**: Combine multiple PDFs into one
- **Image Integration**: Embed images directly in documents
- **Text Extraction**: Extract content from various formats

## 🤝 Contributing

### Development Setup
1. Clone the repository
2. Open `index.html` in a modern browser
3. No build process required - runs directly

### File Structure
```
ConvertFlow-PDF-Doc-Generator/
├── index.html          # Main application file
├── README.md           # This documentation
├── ARCHITECTURE.md     # Technical architecture details
└── .gitignore         # Git ignore rules
```

## 📄 License

This project is open source and available under the MIT License.

## 🆘 Support

### Common Issues
- **Large Files**: Use thread yielding for better performance
- **Memory Usage**: Automatic cleanup prevents memory leaks
- **Browser Compatibility**: Ensure modern browser support

### Error Handling
- **Format Validation**: Clear messages for unsupported formats
- **Processing Errors**: Graceful fallbacks and user feedback
- **Network Issues**: Retry mechanisms for external libraries

## 🚀 Future Roadmap

### Planned Features
- [ ] Additional output formats (EPUB, Markdown)
- [ ] Advanced PDF editing capabilities
- [ ] Cloud storage integration
- [ ] Batch processing improvements
- [ ] OCR for scanned documents
- [ ] Template system for document formatting

### Performance Enhancements
- [ ] Web Workers for heavy processing
- [ ] Progressive loading for large files
- [ ] Caching mechanisms for repeated operations
- [ ] Memory optimization for file processing

---

**ConvertFlow** - Transform your documents with ease and privacy. 🚀
