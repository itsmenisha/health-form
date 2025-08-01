# 🧠 Mental Health Assessment Platform

A comprehensive web application for mental health screening and assessment, developed for Kathmandu Metropolitan City's Health Department. This Flask-based platform provides standardized mental health assessment tools in Nepali language.

## 🌟 Features

### Mental Health Assessment Tools
- **WHO-5 Well-being Index** - Measures psychological well-being over the past two weeks
- **GAD-7 Anxiety Scale** - Screens for generalized anxiety disorder
- **PHQ-9 Depression Scale** - Assesses depression severity

### Key Capabilities
- ✅ **Multilingual Support** - Complete Nepali language interface
- ✅ **Data Collection** - Secure storage of assessment results in Excel format
- ✅ **PDF Reports** - Downloadable assessment reports with interpretations
- ✅ **Privacy Protection** - Confidential handling of personal information
- ✅ **Responsive Design** - Mobile-friendly interface
- ✅ **Educational Content** - Mental health information and resources
- ✅ **Support System** - Emergency helpline numbers and service locations

## 🏗️ Project Structure

```
wellbeing/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── data/                 # Excel files for storing assessment results
│   ├── who5.xlsx
│   ├── gad7.xlsx
│   └── phq9.xlsx
├── photo/               # Static images and assets
│   ├── mental.jpg
│   ├── wellbeing.png
│   └── ...
└── templates/           # HTML templates
    ├── frontpage.html   # Homepage
    ├── about.html       # Mental health information
    ├── services.html    # Available services
    ├── faq.html         # Frequently asked questions
    └── forms/           # Assessment forms
        ├── who5.html    # WHO-5 Well-being assessment
        ├── gad7.html    # GAD-7 Anxiety assessment
        └── phq9.html    # PHQ-9 Depression assessment
```

## 🛠️ Technology Stack

- **Backend**: Flask (Python web framework)
- **Data Storage**: Excel files via openpyxl
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **PDF Generation**: html2pdf.js, jsPDF, html2canvas
- **Styling**: Custom CSS with responsive design

## 📋 Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

## 🚀 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/itsmenisha/health-form.git
   cd health-form/wellbeing
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   python app.py
   ```

4. **Access the application**
   - Open your web browser
   - Navigate to `http://localhost:5000`

## 📊 Assessment Tools Details

### WHO-5 Well-being Index
- **Purpose**: Measures psychological well-being
- **Questions**: 5 items about mood, energy, and life satisfaction
- **Scoring**: 0-25 raw score, converted to 0-100 percentage
- **Interpretation**: 
  - <52%: Low well-being, possible depression
  - 52-80%: Moderate well-being
  - >80%: Good well-being

### GAD-7 (Generalized Anxiety Disorder-7)
- **Purpose**: Screens for anxiety disorders
- **Questions**: 7 items about anxiety symptoms
- **Scoring**: 0-21 total score
- **Interpretation**:
  - 0-4: Minimal anxiety
  - 5-9: Mild anxiety
  - 10-14: Moderate anxiety
  - 15-21: Severe anxiety

### PHQ-9 (Patient Health Questionnaire-9)
- **Purpose**: Assesses depression severity
- **Questions**: 9 items about depressive symptoms
- **Scoring**: 0-27 total score
- **Interpretation**:
  - 0-4: Minimal depression
  - 5-9: Mild depression
  - 10-14: Moderate depression
  - 15-19: Moderately severe depression
  - 20-27: Severe depression

## 🔐 Data Privacy & Security

- All personal information is kept confidential
- Data is stored locally in Excel files
- No public use or distribution of personal data
- Secure handling of assessment results
- Privacy notice displayed on all assessment forms

## 🏥 Mental Health Services Integration

The platform provides information about:
- **Local Health Centers**: 32 ward-level health centers in Kathmandu Metropolitan City
- **Specialist Services**: Urban Health Promotion Center, Babarmahal
- **Emergency Helplines**:
  - National Suicide Prevention: **1166**
  - Kathmandu Metropolitan: **1180**
  - Kanti Children's Hospital Mental Health: **16600110666**
  - Nepal Police: **100**
  - Telemedicine: **1098**

## 🌐 API Endpoints

### Page Routes
- `GET /` - Homepage
- `GET /about` - Mental health information
- `GET /services` - Available services
- `GET /faq` - Frequently asked questions
- `GET /who5` - WHO-5 assessment form
- `GET /gad7` - GAD-7 assessment form
- `GET /phq9` - PHQ-9 assessment form

### Data Submission
- `POST /submit/<form_type>` - Submit assessment results
  - Accepts JSON data with personal info and scores
  - Stores data in corresponding Excel file
  - Returns success/error message

### Static Files
- `GET /photo/<filename>` - Serve static images

## 📱 Responsive Design

The application is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones
- Various screen sizes and orientations

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## 📄 License & Attribution

- **WHO-5**: Licensed under CC-BY-NC-SA 3.0 IGO
- **Source**: World Health Organization. The World Health Organization-Five Well-Being Index (WHO-5). Geneva: World Health Organization; 2024.
- This translation was not created by WHO. WHO is not responsible for the content or accuracy of this translation.

## 🆘 Support & Resources

For mental health emergencies or support:
- **National Suicide Prevention Helpline**: 1166
- **Kathmandu Metropolitan Health**: 1180
- **Nepal Police Emergency**: 100

## 👥 Developed By

**Kathmandu Metropolitan City - Health Department**
© 2025 Kathmandu Metropolitan City | Health Division

---

For technical support or questions about this application, please contact the development team or create an issue in this repository.
