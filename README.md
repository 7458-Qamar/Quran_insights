Quran Insights Dashboard - Complete Islamic Data Analytics
Comprehensive Quran dataset with 114 Surahs analysis featuring Power BI dashboards, DAX formulas for Parah names, CSV data & interactive visualizations for Islamic data analytics.
Show Image
Show Image
Show Image
🕌 Overview
This repository contains a complete data analytics solution for the Holy Quran, featuring detailed information about all 114 Surahs with interactive Power BI dashboards, advanced DAX formulas, and comprehensive CSV datasets.
✨ Key Features
📈 Interactive Power BI Dashboard
Page 1: Overview Analytics

Key metrics cards (Total Words, Ayahs, Surahs, Sajdas)
Top 5 Surahs with most Ayahs (pie chart)
Top 12 Paras with most Ayahs (Arabic names)
Makki vs Madani distribution analysis
Interactive filters for Revelation Type and Period

Page 2: Detailed Analysis

Surah count by each Parah (30 sections)
Total Ayahs by Revelation Type comparison
Period-wise revelation analysis (Early/Middle/Late)
Comprehensive revelation timeline insights

📊 Dataset Features

114 Complete Surahs with detailed metadata
6,236 Total Ayahs analyzed
77,874+ Words estimated count
30 Parah/Juz divisions with traditional names
15 Sajda locations identified
Makki/Madani classification (87 Makki, 27 Madani)
Chronological revelation order tracking

🔧 Technical Components

DAX Formulas for Parah name integration
CSV Export functionality
Multi-language support (Arabic/English)
Period classification (Early/Middle/Late Makki/Madani)
Interactive filtering and drill-down capabilities

📸 Screenshots
Dashboard Page 1: Overview
Show Image
Main dashboard showing key metrics, top Surahs analysis, and revelation type distribution
Dashboard Page 2: Detailed Analytics
Show Image
Detailed analysis including Parah distribution, period-wise breakdown, and comprehensive charts
📊 Key Insights
Revelation Distribution

Makki Surahs: 87 (76.3%) - 4,691 Ayahs
Madani Surahs: 27 (23.7%) - 1,545 Ayahs

Top 5 Longest Surahs

Al-Baqarah - 286 Ayahs
Ash-Shu'ara - 227 Ayahs
Al-A'raf - 206 Ayahs
Aal-E-Imran - 200 Ayahs
As-Saffat - 182 Ayahs

Period Analysis

Early Makki: 38 Surahs (721 Ayahs)
Middle Makki: 20 Surahs (2,153 Ayahs)
Late Makki: 28 Surahs (1,622 Ayahs)
Early Madani: 7 Surahs (838 Ayahs)
Late Madani: 21 Surahs (902 Ayahs)

🚀 Getting Started
Prerequisites

Microsoft Power BI Desktop
Basic knowledge of DAX formulas (optional)
CSV viewer/editor (Excel, Google Sheets, etc.)

Installation

Clone the repository

bashgit clone https://github.com/yourusername/quran-insights-dashboard.git
cd quran-insights-dashboard

Open Power BI file

Launch Power BI Desktop
Open Quran_Insights_Dashboard.pbix


Load CSV data (if using separately)

Import quran_complete_dataset.csv
Apply provided DAX formulas



Usage

Explore dashboards using interactive filters
Filter by Revelation Type (Makki/Madani)
Analyze by Period (Early/Middle/Late)
Export data for further analysis
Customize visualizations as needed

🔧 DAX Formulas Included
Parah Name Integration
daxParah_Full_Name = 
"Para " & QuranData[Starting_Juz] & " - " &
SWITCH(
    QuranData[Starting_Juz],
    1, "Alif Lam Mim (الم)",
    2, "Sayaqul (سيقول)",
    // ... continues for all 30 Parah
)
Advanced Analytics

Revelation type calculations
Period-wise aggregations
Ayah distribution metrics
Sajda counting formulas

📁 File Structure
quran-insights-dashboard/
├── README.md
├── Quran_Insights_Dashboard.pbix
├── data/
│   ├── quran_complete_dataset.csv
│   └── parah_lookup_table.csv
├── dax-formulas/
│   ├── parah_names.dax
│   └── advanced_calculations.dax
├── images/
│   ├── dashboard-page1.png
│   └── dashboard-page2.png
└── docs/
    ├── data_dictionary.md
    └── installation_guide.md
📖 Data Dictionary
ColumnDescriptionTypeSurah_NumberSequential number (1-114)IntegerSurah_Name_ArabicArabic nameTextSurah_Name_EnglishEnglish transliterationTextTotal_AyahsNumber of versesIntegerRevelation_TypeMakki or MadaniTextSajdas_CountNumber of prostration versesIntegerStarting_JuzStarting Parah numberIntegerEnding_JuzEnding Parah numberIntegerEnglish_MeaningTranslation of Surah nameTextRevelation_OrderChronological order (1-114)IntegerPeriod_of_RevelationEarly/Middle/Late classificationTextApproximate_WordsEstimated word countInteger
🎯 Use Cases
For Researchers

Academic studies on Quranic structure
Statistical analysis of revelation patterns
Comparative studies between Makki/Madani periods

For Educators

Teaching aids for Islamic studies
Visual learning tools for students
Interactive exploration of Quranic data

For Data Analysts

Power BI template for Islamic data
DAX formula examples for text analysis
Dashboard design inspiration

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
How to Contribute

Fork the repository
Create your feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request

Areas for Contribution

Additional visualizations
Enhanced DAX formulas
Multi-language translations
Mobile-responsive dashboards
API integration features

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
🙏 Acknowledgments

Data compiled from authentic Islamic sources
Traditional Parah names preserved with Arabic text
Inspired by the need for accessible Quranic data analytics
Community feedback and Islamic scholarly review

📧 Contact
For questions, suggestions, or collaborations:

Email: your.email@example.com
LinkedIn: [Your LinkedIn Profile]
Issues: [GitHub Issues Page]


⭐ If this project helps you, please give it a star! ⭐
"And We have certainly made the Qur'an easy for remembrance, so is there any who will remember?" - Quran 54:17
