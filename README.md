# SmartCV 🚀

An AI-powered resume optimization tool designed to streamline the job application process. Features include professional template building, ATS-friendly analysis, keyword and skills gap insights, and AI-driven content optimization. Enables creation of tailored, recruiter-ready resumes from scratch or imported documents.

![SmartCV Banner](https://img.shields.io/badge/SmartCV-AI%20Resume%20Optimizer-blue?style=for-the-badge&logo=artificial-intelligence)

## ✨ Features

### 🤖 AI-Powered Analysis
- **Advanced Resume Analysis** using Google Gemini AI
- **ATS Compatibility Check** to ensure your resume passes applicant tracking systems
- **Content Optimization** with AI-driven suggestions for better impact
- **Skills Gap Analysis** to identify missing skills for target roles

### 📝 Professional Resume Builder
- **4 Premium Templates**: Modern, Professional, Minimal, and Creative
- **Real-time Preview** with instant formatting
- **Export Options**: PDF and DOCX formats
- **Template Customization** with professional styling

### 🎯 Smart Job Matching
- **LinkedIn Integration** for job discovery
- **Multi-Portal Search** across various job platforms
- **Location-based Filtering** with smart suggestions
- **Company Insights** and market analysis

### 📊 Analytics & Insights
- **Comprehensive Dashboard** with usage metrics
- **Performance Tracking** for resume improvements
- **Success Rate Analytics** and optimization suggestions
- **Export Reports** for detailed analysis

### 🔧 Additional Tools
- **Document Import** support for existing resumes (PDF/DOCX)
- **Keyword Optimization** for better searchability
- **Course Recommendations** based on skill gaps
- **Feedback System** for continuous improvement

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Google API Key (for AI analysis)
- Chrome browser (for job search features)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/smartcv.git
cd smartcv
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Set up environment variables**
Create a `.env` file in the root directory:
```env
GOOGLE_API_KEY=your_google_api_key_here
OPENROUTER_API_KEY=your_openrouter_api_key_here  # Optional
```

4. **Initialize the database**
```bash
python -c "from config.database import init_database; init_database()"
```

5. **Run the application**
```bash
# Using the run script (recommended)
python run_app.py

# Or directly with Streamlit
streamlit run app.py
```

6. **Access the application**
Open your browser and navigate to `http://localhost:8501`

## 🎯 Usage Guide

### 1. Resume Analysis
- Upload your existing resume (PDF/DOCX)
- Select target job role from 50+ predefined roles
- Get AI-powered analysis with:
  - Overall score and recommendations
  - Skills gap identification
  - ATS compatibility check
  - Content optimization suggestions

### 2. Resume Building
- Choose from 4 professional templates
- Fill in your information using the guided form
- Real-time preview with instant updates
- Export as PDF or DOCX

### 3. Job Search
- Search across multiple job portals
- Use LinkedIn scraper for targeted opportunities
- Filter by location, experience, and salary
- Get company insights and market data

### 4. Analytics Dashboard
- Track your resume performance
- Monitor improvement metrics
- Export detailed reports
- View usage statistics

## 🏗️ Project Structure

```
smartcv/
├── app.py                 # Main Streamlit application
├── run_app.py            # Application launcher
├── requirements.txt      # Python dependencies
├── config/               # Configuration files
│   ├── database.py      # Database setup and management
│   ├── job_roles.py     # Job role definitions
│   └── courses.py       # Course recommendations
├── utils/               # Utility modules
│   ├── ai_resume_analyzer.py  # AI analysis engine
│   ├── resume_builder.py      # Resume generation
│   ├── resume_analyzer.py     # Traditional analysis
│   └── resume_parser.py       # Document parsing
├── jobs/                # Job search functionality
│   ├── job_search.py    # Main job search interface
│   ├── linkedin_scraper.py    # LinkedIn integration
│   └── job_portals.py   # Multi-portal search
├── dashboard/           # Analytics and reporting
│   └── dashboard.py     # Dashboard management
├── feedback/            # User feedback system
│   └── feedback.py      # Feedback collection
└── style/              # UI styling
    └── style.css       # Custom CSS
```

## 🤖 AI Models

SmartCV leverages advanced AI models for intelligent resume analysis:

- **Google Gemini**: Primary AI model for content analysis and optimization
- **Natural Language Processing**: For skills extraction and keyword matching
- **Machine Learning**: For ATS compatibility scoring

### API Setup

1. **Google Gemini API**:
   - Visit [Google AI Studio](https://makersuite.google.com/)
   - Generate your API key
   - Add to `.env` file as `GOOGLE_API_KEY`

## 📋 Supported Job Roles

SmartCV supports 50+ job roles across various industries:

- **Software Development**: Frontend, Backend, Full Stack, Mobile
- **Data Science**: Data Analyst, Data Scientist, ML Engineer
- **Cloud & DevOps**: Cloud Architect, DevOps Engineer, SRE
- **Design**: UI/UX Designer, Graphic Designer
- **Management**: Project Manager, Product Manager
- **And many more...**

## 🎨 Resume Templates

### 1. Modern Template
- Clean, contemporary design
- Emphasis on visual hierarchy
- Perfect for tech roles

### 2. Professional Template
- Traditional corporate style
- Conservative formatting
- Ideal for business roles

### 3. Minimal Template
- Simple, distraction-free layout
- Focus on content over design
- Great for academic positions

### 4. Creative Template
- Unique, eye-catching design
- Creative industry focused
- Perfect for design roles

## 🛠️ Technical Features

### ATS Optimization
- Keyword density analysis
- Format compatibility check
- Section structure validation
- Font and styling recommendations

### AI Analysis Engine
- Content quality assessment
- Skills gap identification
- Industry-specific recommendations
- Performance scoring (0-100)

### Export Capabilities
- High-quality PDF generation
- Microsoft Word compatibility
- Multiple format options
- Professional formatting

## 🚀 Deployment

### Local Development
```bash
python run_app.py
```

### Production Deployment

#### Using Docker
```bash
docker build -t smartcv .
docker run -p 8501:8501 smartcv
```

#### Using Streamlit Cloud
1. Fork this repository
2. Connect to Streamlit Cloud
3. Add environment variables
4. Deploy automatically

#### Using Heroku
```bash
git add .
git commit -m "Deploy to Heroku"
git push heroku main
```

## 📊 Analytics & Metrics

SmartCV provides comprehensive analytics:

- **Usage Statistics**: Track application usage
- **Resume Performance**: Monitor improvement over time
- **Success Metrics**: Measure optimization effectiveness
- **User Feedback**: Continuous improvement insights

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Setup
```bash
# Install development dependencies
pip install -r requirements.txt

# Run tests
python -m pytest tests/

# Format code
black .
flake8 .
```

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

### Common Issues

**Chrome Driver Issues**:
```bash
python setup_chromedriver.py
```

**Database Errors**:
```bash
python -c "from config.database import init_database; init_database()"
```

**API Key Issues**:
- Ensure your `.env` file is properly configured
- Verify API key validity
- Check API quotas and limits

### Getting Help

- 📧 Email: support@smartcv.com
- 💬 Discord: [Join our community](https://discord.gg/smartcv)
- 📖 Documentation: [Full docs](https://docs.smartcv.com)
- 🐛 Issues: [GitHub Issues](https://github.com/yourusername/smartcv/issues)

## 🙏 Acknowledgments

- Google Gemini AI for intelligent analysis
- Streamlit for the amazing web framework
- The open-source community for various tools and libraries

## 📈 Roadmap

- [ ] Multi-language support
- [ ] Advanced ATS scoring algorithms
- [ ] Integration with more job portals
- [ ] Mobile app development
- [ ] Team collaboration features
- [ ] Advanced analytics dashboard

---

<div align="center">

**Made with ❤️ for job seekers worldwide**

[Website](https://smartcv.com) • [Documentation](https://docs.smartcv.com) • [Community](https://discord.gg/smartcv)

</div>