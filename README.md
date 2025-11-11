# 🔍 Glossaire Médical - Search Application

A powerful, real-time search application for medical terminology glossaries, featuring advanced search capabilities and a mobile-responsive design.

## ✨ Features

- **⚡ Real-time search** - Results appear as you type with intelligent debouncing
- **🎯 Advanced search algorithms** - Fuzzy matching and relevance scoring
- **📱 Mobile-responsive** - Beautiful UX optimized for all devices
- **🔍 Multi-field search** - Searches across terms, meanings, and references
- **🏷️ Smart filtering** - Filter by compound forms or endings
- **💡 Intelligent highlighting** - Visual emphasis on matching terms
- **📊 Live statistics** - Real-time count of results
- **🚀 Fast performance** - Client-side processing for instant results

## 📁 Files

- `index.html` - Main application file (standalone, no dependencies)
- `glossaire_formes_composees_A-Z.csv` - Compound forms glossary (473 entries)
- `glossaire_terminaisons_A-Z_complet.csv` - Endings glossary (128 entries)

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Create a new GitHub repository**
   ```bash
   # Create a new repo on GitHub, then:
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository settings
   - Navigate to "Pages" section
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be available at: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

### Option 2: Local Testing

Simply open `index.html` in your web browser. The application works entirely client-side!

```bash
# If you have Python installed:
python -m http.server 8000

# Or with Node.js:
npx serve

# Then open http://localhost:8000
```

## 🎨 Technology Stack

- **Pure JavaScript** - No frameworks or dependencies
- **CSS3** - Modern animations and responsive design
- **HTML5** - Semantic markup
- **CSV parsing** - Custom implementation with quote handling
- **Search algorithms**:
  - Term matching with relevance scoring
  - Fuzzy matching for approximate searches
  - Multi-term AND logic
  - Real-time debouncing (150ms)

## 🔧 Search Features Explained

### Relevance Scoring
- **Exact match in term**: 100 points (highest priority)
- **Exact match in meaning**: 50 points
- **Match in reference**: 25 points
- **Fuzzy match**: 10 points

### Search Behavior
- Searches all fields simultaneously
- Multiple words are treated as AND (all must match)
- Case-insensitive matching
- Results limited to 100 for optimal performance
- Results sorted by relevance score

## 📱 Mobile Optimization

- Touch-friendly interface
- Optimized typography for readability
- Responsive layout (adapts to screen size)
- Fast performance on mobile networks
- No external dependencies to load

## 🎯 Use Cases

- Medical students studying terminology
- Healthcare professionals looking up terms
- Translation and documentation work
- Quick reference during consultations
- Educational purposes

## 🌐 Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 CSV Format

The application expects CSV files with the following format:

**Formes composées:**
```csv
Forme,Signification,Référence
a-,"manque de, sans",1.49 et 50
```

**Terminaisons:**
```csv
Terminaison,Signification,Référence
-a,(1) nominatif féminin singulier ; (2) nominatif neutre pluriel,1.83 & 86 ; 6.23
```

## 🔄 Updating Data

To update the glossaries:
1. Replace the CSV files with your updated versions
2. Commit and push to GitHub
3. Changes will be live automatically

## 💡 Tips

- Use specific terms for more precise results
- Try different spellings if you don't find what you're looking for
- Use the filters to narrow down results by type
- The search works best with medical terminology

## 📝 License

Feel free to use and modify this application for your needs.

## 🤝 Contributing

Suggestions and improvements are welcome! The code is self-contained in `index.html` for easy modification.

---

**Built with ❤️ for medical terminology enthusiasts**
