# 📚 SSC Vocabulary Flashcards

An interactive, mobile-friendly vocabulary learning application designed specifically for SSC (Staff Selection Commission) exam preparation.

## 🌐 Live Demo

**[Click here to use the app](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/Index-Clean.html)**

Replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your actual GitHub username and repository name.

## ✨ Features

### 🎯 Learning Modes
- **Flashcard Mode**: Interactive flip cards with Hindi and English meanings
- **Quiz Mode**: Test your knowledge with multiple-choice questions
- **Progress Tracking**: Track remembered vs. not-remembered words
- **History**: View detailed performance analytics of past quizzes

### 📊 Content Coverage
- **957+ Vocabulary Words**
- **Synonyms & Antonyms**
- **Idioms & Phrases**
- **One-Word Substitutes**

### 📱 Exam-Specific Sections
- **SSC CGL** (Combined Graduate Level)
- **SSC CHSL** (10+2 Level)
- **SSC MTS** (Multi Tasking Staff)
- **SSC CPO** (Central Police Organisation)
- **SSC GD** (General Duty Constable)
- **SSC Stenographer** (Grade C & D)
- **SSC JE** (Junior Engineer)

### 🎨 User Experience
- ✅ Mobile-responsive design
- ✅ Swipe gestures for flashcards
- ✅ Filter by exam and word type
- ✅ Shuffle mode for random practice
- ✅ Dark/light theme support
- ✅ Offline-capable (after first load)
- ✅ LocalStorage for progress persistence

## 🚀 Quick Start

### For Users
1. Simply visit the live link above
2. Select your target exam (CGL, CHSL, etc.)
3. Choose flashcard or quiz mode
4. Start learning!

### For Developers

#### Local Development
```bash
# Clone the repository
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME

# Start a local server (choose one):
python -m http.server 8000        # Python 3
python -m SimpleHTTPServer 8000   # Python 2
npx http-server                   # Node.js

# Open in browser
http://localhost:8000/Index-Clean.html
```

## 📁 Project Structure

```
ssc-vocabulary/
├── Index-Clean.html          # Main application file
├── vocab.html                # Vocabulary database (HTML format)
├── vocab-data-loader.js      # Data extraction script (optional)
├── README.md                 # This file
├── QUICK_START.md           # Quick start guide
└── GITHUB_DEPLOYMENT.md     # GitHub Pages deployment guide
```

## 📝 Adding New Vocabulary

To add new words to the database:

1. Open `vocab.html`
2. Find the appropriate exam section (e.g., `<div class="exam-section exam-cgl">`)
3. Add a new word using this template:

```html
<div class="q">
    <div class="q-head">
        <span class="q-num"></span>
        <span class="q-word">Your Word</span>
        <span class="q-hindi"> - हिंदी अर्थ</span>
        <span class="q-eng"> (English meaning)</span>
    </div>
    <div class="opts">
        <div class="opt"><b>A)</b> <strong>option1</strong> – <em>अर्थ1</em></div>
        <div class="opt"><b>B)</b> <strong>option2</strong> – <em>अर्थ2</em></div>
        <div class="opt"><b>C)</b> <strong>correct</strong> – <em>सही अर्थ ✓ (s)</em></div>
        <div class="opt"><b>D)</b> <strong>option4</strong> – <em>अर्थ4</em></div>
    </div>
    <div class="notes"><small>NOTES:</small><hr></div>
</div>
```

4. Mark the correct answer with ✓ in the `<em>` tag
5. Commit and push your changes
6. GitHub Pages will automatically update in 1-2 minutes!

## 🛠️ Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with responsive design
- **Data Format**: Semantic HTML (structured in vocab.html)
- **Data Loading**: Dynamic parsing via DOMParser API
- **Storage**: LocalStorage for progress and history
- **Hosting**: GitHub Pages (free static hosting)

## 🎯 Design Philosophy

### Why Separate Data from Application?

This project follows the principle of **separation of concerns**:

- **vocab.html**: Single source of truth for all vocabulary data
- **Index-Clean.html**: Application logic and user interface
- **Result**: Easy maintenance, no data duplication

### Benefits:
- ✅ Update vocabulary in ONE place only
- ✅ Smaller application file (78% reduction)
- ✅ Easier for contributors to add words
- ✅ Clear separation of data and logic

## 📈 Performance

- **Initial Load**: ~1.2 MB (includes all 957 words)
- **Subsequent Loads**: Cached (instant)
- **Data Parsing**: <200ms for 957 items
- **Memory Usage**: ~5 MB (browser dependent)

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Add Vocabulary**: Submit words via pull request to `vocab.html`
2. **Report Bugs**: Open an issue with details
3. **Suggest Features**: Propose new features via issues
4. **Fix Typos**: Correct any mistakes in vocabulary

### Contribution Guidelines

1. Fork the repository
2. Create a new branch (`git checkout -b feature/add-words`)
3. Make your changes
4. Test locally
5. Commit (`git commit -m 'Add 50 new CGL words'`)
6. Push (`git push origin feature/add-words`)
7. Open a Pull Request

## 📄 License

This project is available for free use for educational purposes. Feel free to:
- Use it for your SSC exam preparation
- Share it with friends and students
- Modify it for your needs
- Host your own version

## 🙏 Acknowledgments

- Vocabulary sourced from SSC previous year papers
- Inspired by the need for accessible exam preparation tools
- Built with ❤️ for SSC aspirants

## 📧 Support

Having issues or suggestions?

- **Report Bugs**: [Open an issue](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME/issues)
- **Ask Questions**: Use the [Discussions tab](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME/discussions)
- **Email**: your-email@example.com (optional)

## 🌟 Show Your Support

If this app helps you in your SSC preparation:
- ⭐ Star this repository
- 🔀 Fork it to create your own version
- 📢 Share it with fellow aspirants

## 📚 Related Resources

- [SSC Official Website](https://ssc.nic.in/)
- [SSC CGL Syllabus](https://ssc.nic.in/)
- [More SSC Resources](#) (add your links)

## 🗺️ Roadmap

Future enhancements planned:
- [ ] Add pronunciation guide
- [ ] Include example sentences
- [ ] Add more exams (IBPS, Railways, etc.)
- [ ] Spaced repetition algorithm
- [ ] Export/import progress
- [ ] Dark mode toggle
- [ ] Voice pronunciation
- [ ] PDF export of vocabulary

---

**Made with 💙 for SSC Aspirants**

*Star ⭐ this repo if it helped you!*

Last Updated: February 2026
