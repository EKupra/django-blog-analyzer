# Boosty - AI-Powered Blog Analyzer

A powerful Django-based blog analysis tool that provides actionable insights on SEO, Content Quality, Visual Design, UX, Engagement, and Topic Fit. Perfect for bloggers and content creators who want to optimize their content for better reach and engagement.

## 📺 Demo & Presentation

### 🎥 Video Demo
Watch a quick walkthrough of Boosty in action:

https://youtu.be/4VfoYLZEkbM


### 📊 Presentation
View the detailed presentation about Boosty:

[Boosty_Final.pdf](https://github.com/user-attachments/files/23832945/Boosty_Final.pdf)


---

## 🎯 Features

### Core Analysis
- **AI Summarization**: Automatically generates concise summaries using LSA (Latent Semantic Analysis)
- **SEO Optimization**: Meta descriptions, H1 tags, keyword analysis with specific recommendations
- **Content Quality**: Word count, readability, grammar checking with detailed issue detection
- **Visual Design**: Image count, alt text validation, mobile responsiveness checks
- **Topic Detection**: Identifies your blog topic (Travel, Food, Sport, Music, Literature, Art)

### Premium Features
- **User Experience (UX)**: Navigation and flow analysis
- **Engagement Metrics**: Content stickiness and reader retention insights
- **Topic Fit**: Deep relevance analysis for your niche
- **Detailed Recommendations**: Specific, actionable fixes with AI-generated solutions

### Freemium Model
- **Free Tier**: Basic analysis with 3 visible recommendations
- **Premium Tier**: Full access to all metrics, unlimited recommendations, and advanced insights
- **Seamless Upgrade Flow**: One-click registration to unlock full report

### User Experience
- **Gamification**: Progress tracking, achievement badges, seasonal challenges
- **Leaderboards**: See top-performing blogs and track improvements
- **Confetti Celebrations**: Animated rewards for high scores
- **Social Sharing**: Share on X (Twitter), LinkedIn, or email
- **Export Options**: Print reports or save for later

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- pip package manager
- Virtual environment (recommended)

### Installation

## 🚀 Installation Guide

Follow these steps to run WebBoost — Boosty locally on your machine.

### 📌 Prerequisites
You need the following installed on your system:
- Python 3.8 or higher
- pip (Python package manager)
- virtualenv or Python’s built-in venv module

### 🔧 Step 1: Clone the Repository
Clone the project and enter the project folder:
git clone https://github.com/EKupra/WebBoost---Boosty.git
cd WebBoost---Boosty

### 🌱 Step 2: Create and Activate a Virtual Environment
Create and activate a virtual environment depending on your operating system.

On macOS / Linux:
python3 -m venv venv
source venv/bin/activate

On Windows (PowerShell):
python -m venv venv
venv\Scripts\Activate.ps1

On Windows (CMD):
venv\Scripts\activate.bat

### 📦 Step 3: Install Dependencies
Install all required packages:
pip install -r requirements.txt

### 📚 Step 4: Download NLP Datasets
Download necessary corpora for TextBlob and NLTK:
python -m textblob.download_corpora
python -m nltk.downloader vader_lexicon punkt

### 🗄️ Step 5: Apply Migrations
Set up the database:
python manage.py migrate

### ▶️ Step 6: Run the Server
Start the local development server:
python manage.py runserver 8001

### 🌐 Step 7: Open in Browser
Open your browser and go to:
http://127.0.0.1:8001

You can now use WebBoost — Boosty to analyze any blog for SEO insights, sentiment, readability, and more.


## 💡 Usage

1. **Enter a Blog URL**: Paste any blog post URL (e.g., `https://example.com/my-blog-post`)
2. **Get Free Analysis**: View overall score, topic detection, and 3 free recommendations
3. **Unlock Full Report**: Register to see all premium insights and detailed recommendations
4. **Share Results**: Use the Share dropdown to export or share on social media

## 📁 Project Structure

```
boosty/
├── analyzer_app/
│   ├── logic.py              # Core analysis engine (SEO, grammar, summaries)
│   ├── views.py              # Django views (analyze, register, pricing, logout)
│   ├── urls.py               # URL routing
│   ├── topic_trainer.py      # Topic model training
│   └── templates/
│       └── analyzer_app/
│           ├── index.html          # Landing page with FAQ
│           ├── result.html         # Analysis results page
│           ├── pricing.html        # Pricing tiers
│           ├── register.html       # Registration page
│           └── premium_dashboard.html
├── website_analyzer/          # Django project settings
├── benchmarks.json            # Topic category benchmarks
├── topic_models.json          # Trained topic detection models
└── requirements.txt           # Python dependencies
```

## 🛠 Technologies

- **Backend**: Django 4.x, Python 3.12
- **NLP Libraries**: 
  - NLTK (VADER sentiment analysis, tokenization)
  - TextBlob (grammar and spell checking)
  - Sumy (LSA summarization)
  - NumPy (numerical computations)
- **Web Scraping**: BeautifulSoup4, Requests
- **Frontend**: Tailwind CSS, Vanilla JavaScript
- **Animations**: Canvas Confetti

## 📚 Documentation

For detailed feature documentation and implementation details, see:
- [documentation.md](documentation.md) - Complete feature guide
- [benchmarks.json](benchmarks.json) - Topic category reference scores

## 🎨 UI Features

- **Expandable FAQ**: Accordion-style questions on landing page
- **Interactive Dropdowns**: Share options and Personal Cabinet menu
- **Responsive Design**: Mobile-first with Tailwind CSS
- **Before/After Toggle**: See original issues and AI-generated fixes
- **Premium Gates**: Beautiful blur effects for locked content

## 🔐 Freemium Flow

1. **Free Analysis** → Blurred premium sections with "Unlock Full Report" CTA
2. **Register** → Simple registration form (simulated)
3. **Full Report** → Session-based premium access with all insights unlocked
4. **Logout** → Clear session and return to free tier

## 📊 Benchmarks

Boosty includes benchmark data for 5 topic categories:
- **Travel**: [Walking the World](https://walkingtheworld.substack.com/)
- **Food**: [What to Cook](https://whattocook.substack.com/)
- **Sport**: [Bill and Doug OSU](https://billanddougosu.substack.com/)
- **Music**: [Honest Broker](https://www.honest-broker.com/)
- **Literature**: [A Little Blog of Books](https://alittleblogofbooks.com/)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

### Development Setup

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

MIT License - feel free to use this project for personal or commercial purposes.


**Made with ❤️ for bloggers and content creators worldwide**

---

### 🎯 Roadmap

- [ ] Integration with WordPress and Medium APIs
- [ ] Advanced AI content suggestions using GPT
- [ ] Multi-language support
- [ ] Browser extension for quick analysis
- [ ] Analytics dashboard for tracking improvements over time
