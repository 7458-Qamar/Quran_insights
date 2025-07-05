# 📊 Quran Insights Dashboard - Complete Islamic Data Analytics

**Comprehensive Quran dataset with 114 Surahs analysis featuring Power BI dashboards, DAX formulas for Parah names, CSV data & interactive visualizations for Islamic data analytics.**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![CSV](https://img.shields.io/badge/CSV-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

## 🕌 Overview

This repository contains a complete data analytics solution for the Holy Quran, featuring detailed information about all 114 Surahs with interactive Power BI dashboards, advanced DAX formulas, and comprehensive CSV datasets.

## ✨ Key Features

### 📈 Interactive Power BI Dashboard

**Page 1: Overview Analytics**
- Key metrics cards (Total Words, Ayahs, Surahs, Sajdas)
- Top 5 Surahs with most Ayahs (pie chart)
- Top 12 Paras with most Ayahs (Arabic names)
- Makki vs Madani distribution analysis
- Interactive filters for Revelation Type and Period

**Page 2: Detailed Analysis**
- Surah count by each Parah (30 sections)
- Total Ayahs by Revelation Type comparison
- Period-wise revelation analysis (Early/Middle/Late)
- Comprehensive revelation timeline insights

### 📊 Dataset Features

- **114 Complete Surahs** with detailed metadata
- **6,236 Total Ayahs** analyzed
- **77,874+ Words** estimated count
- **30 Parah/Juz divisions** with traditional names
- **15 Sajda locations** identified
- **Makki/Madani classification** (87 Makki, 27 Madani)
- **Chronological revelation order** tracking

### 🔧 Technical Components

- **DAX Formulas** for Parah name integration
- **CSV Export** functionality
- **Multi-language support** (Arabic/English)
- **Period classification** (Early/Middle/Late Makki/Madani)
- **Interactive filtering** and drill-down capabilities

## 📸 Screenshots

### Dashboard Page 1: Overview
![Quran Insights Dashboard Page 1](images/dashboard-page1.png)

*Main dashboard showing key metrics, top Surahs analysis, and revelation type distribution*

### Dashboard Page 2: Detailed Analytics
![Quran Insights Dashboard Page 2](images/dashboard-page2.png)

*Detailed analysis including Parah distribution, period-wise breakdown, and comprehensive charts*

## 📊 Key Insights

### Revelation Distribution
- **Makki Surahs**: 87 (76.3%) - 4,691 Ayahs
- **Madani Surahs**: 27 (23.7%) - 1,545 Ayahs

### Top 5 Longest Surahs
1. **Al-Baqarah** - 286 Ayahs
2. **Ash-Shu'ara** - 227 Ayahs  
3. **Al-A'raf** - 206 Ayahs
4. **Aal-E-Imran** - 200 Ayahs
5. **As-Saffat** - 182 Ayahs

### Period Analysis
- **Early Makki**: 38 Surahs (721 Ayahs)
- **Middle Makki**: 20 Surahs (2,153 Ayahs)
- **Late Makki**: 28 Surahs (1,622 Ayahs)
- **Early Madani**: 7 Surahs (838 Ayahs)
- **Late Madani**: 21 Surahs (902 Ayahs)

## 🚀 Getting Started

### Prerequisites
- Microsoft Power BI Desktop
- Basic knowledge of DAX formulas (optional)
- CSV viewer/editor (Excel, Google Sheets, etc.)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/quran-insights-dashboard.git
cd quran-insights-dashboard
```

2. **Open Power BI file**
   - Launch Power BI Desktop
   - Open `Quran_Insights_Dashboard.pbix`

3. **Load CSV data** (if using separately)
   - Import `quran_complete_dataset.csv`
   - Apply provided DAX formulas

### Usage

1. **Explore dashboards** using interactive filters
2. **Filter by Revelation Type** (Makki/Madani)
3. **Analyze by Period** (Early/Middle/Late)
4. **Export data** for further analysis
5. **Customize visualizations** as needed

## 🔧 DAX Formulas Included

### Parah Name Integration
```dax
Parah_Full_Name = 
"Para " & QuranData[Starting_Juz] & " - " &
SWITCH(
    QuranData[Starting_Juz],
    1, "Alif Lam Mim (الم)",
    2, "Sayaqul (سيقول)",
    // ... continues for all 30 Parah
)
```

### Advanced Analytics
- Revelation type calculations
- Period-wise aggregations  
- Ayah distribution metrics
- Sajda counting formulas

## 📁 File Structure
```
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
```

## 📖 Data Dictionary

| Column | Description | Type |
|--------|-------------|------|
| Surah_Number | Sequential number (1-114) | Integer |
| Surah_Name_Arabic | Arabic name | Text |
| Surah_Name_English | English transliteration | Text |
| Total_Ayahs | Number of verses | Integer |
| Revelation_Type | Makki or Madani | Text |
| Sajdas_Count | Number of prostration verses | Integer |
| Starting_Juz | Starting Parah number | Integer |
| Ending_Juz | Ending Parah number | Integer |
| English_Meaning | Translation of Surah name | Text |
| Revelation_Order | Chronological order (1-114) | Integer |
| Period_of_Revelation | Early/Middle/Late classification | Text |
| Approximate_Words | Estimated word count | Integer |

## 🎯 Use Cases

### For Researchers
- **Academic studies** on Quranic structure
- **Statistical analysis** of revelation patterns
- **Comparative studies** between Makki/Madani periods

### For Educators  
- **Teaching aids** for Islamic studies
- **Visual learning** tools for students
- **Interactive exploration** of Quranic data

### For Data Analysts
- **Power BI template** for Islamic data
- **DAX formula examples** for text analysis
- **Dashboard design** inspiration

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### How to Contribute

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Areas for Contribution

- Additional visualizations
- Enhanced DAX formulas
- Multi-language translations
- Mobile-responsive dashboards
- API integration features

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Data compiled from authentic Islamic sources
- Traditional Parah names preserved with Arabic text
- Inspired by the need for accessible Quranic data analytics
- Community feedback and Islamic scholarly review

## 📧 Contact

For questions, suggestions, or collaborations:
- **Email**: your.email@example.com
- **LinkedIn**: [Your LinkedIn Profile]
- **Issues**: [GitHub Issues Page]

---

**⭐ If this project helps you, please give it a star! ⭐**

*"And We have certainly made the Qur'an easy for remembrance, so is there any who will remember?" - Quran 54:17*
