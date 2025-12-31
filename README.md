#  Urban Umami: End-to-End NLP Pipeline for NYC Restaurant Feedback

##  Project Overview

A comprehensive sentiment analysis and data mining project analyzing **8,886 restaurant reviews** from TripAdvisor to extract actionable business insights using Natural Language Processing (NLP) techniques.

##  Project Objectives

- Perform comprehensive sentiment analysis on restaurant reviews
- Identify patterns and trends in customer satisfaction
- Extract actionable insights for restaurant owners, customers, and platform operators
- Create data-driven recommendations for business improvement

## Dataset Description

- **Source**: TripAdvisor Restaurant Reviews (NYC)
- **Size**: 8,886 reviews
- **Columns**:
  - `Title`: Restaurant name
  - `Number of review`: Total review count
  - `Category`: Cuisine type
  - `Review Comment`: Customer review text
  - `Popular food`: Signature dishes
  - `Online Order`: Online ordering capability (Yes/No)

##  Technologies Used

### Core Libraries
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **matplotlib & seaborn** - Data visualization
- **plotly** - Interactive visualizations

### NLP & Text Analysis
- **nltk** - Natural language processing
- **TextBlob** - Sentiment analysis
- **WordCloud** - Visual text representation

### Machine Learning
- **scikit-learn** - Data preprocessing and analysis
- **xgboost** - Advanced modeling (prepared for future extensions)
- **scipy** - Statistical analysis

##  Analysis Phases

### Phase 1: Data Exploration & Preparation 
- Comprehensive data quality check
- Distribution analysis for all variables
- Outlier detection and handling
- Data cleaning and preprocessing

### Phase 2: Sentiment Analysis (Core) 
- TextBlob-based sentiment scoring (-1 to +1 scale)
- Classification: Positive/Negative/Neutral
- Subjectivity and intensity metrics
- Validation with sample reviews

### Phase 3: Analytical Deep Dives 
- **3A**: Category performance analysis
- **3B**: Review length correlation studies
- **3C**: Online ordering impact assessment
- **3D**: Popular food item analysis
- **3E**: Review volume patterns
- **3F**: Text mining and keyword extraction

### Phase 4: Multi-Dimensional Insights 
- Restaurant performance scorecard
- Composite performance metrics
- 2x2 performance matrix (Sentiment × Volume)
- Hidden gems identification

### Phase 5-7: Advanced Analytics 
- Pattern detection algorithms
- Professional visualization dashboard
- Word clouds for positive/negative reviews

### Phase 8: Business Recommendations 
- Actionable insights for restaurant owners
- Customer guidance for best experiences
- Platform optimization strategies
- Strategic market opportunities

### Phase 9: Executive Summary 
- Comprehensive findings report
- Key statistics overview
- Surprising insights
- Risk identification and mitigation

##  Quick Start

### Prerequisites
```bash
# Install required packages
pip install -r requirements.txt
```

### Running the Analysis
```bash
# Open Jupyter Notebook
jupyter notebook app.ipynb

# Or run in VS Code with Jupyter extension
# Simply open app.ipynb and run all cells
```

##  Key Findings

### Overall Sentiment Landscape
- **Positive Reviews**: ~60-70% of total reviews
- **Negative Reviews**: ~15-25% of total reviews
- **Neutral Reviews**: ~10-20% of total reviews

### Top Insights
1. **Category Matters**: Significant sentiment variation across cuisine types
2. **Digital Advantage**: Online ordering correlates with better customer satisfaction
3. **Hidden Gems**: Many high-quality restaurants have low visibility
4. **Quality vs Volume**: Popularity doesn't guarantee satisfaction
5. **Service is Key**: Most negative reviews mention service-related issues

##  Output Files

After running the analysis, the following files are generated:

- `restaurant_analysis_with_sentiment.csv` - Enhanced dataset with sentiment scores
- `restaurant_analysis_dashboard.png` - Comprehensive visualization dashboard
- Various inline visualizations in the notebook

##  New Features Added to Dataset

The analysis enriches the original dataset with:
- `sentiment_score`: Polarity score (-1 to +1)
- `sentiment_class`: Positive/Negative/Neutral classification
- `subjectivity_score`: Objectivity measure (0 to 1)
- `sentiment_intensity`: Absolute sentiment strength
- `word_count`: Number of words per review
- `length_quartile`: Review length category
- `performance_category`: Restaurant performance quadrant

##  Use Cases

### For Restaurant Owners
- Identify strengths and weaknesses
- Benchmark against category standards
- Understand customer sentiment drivers
- Make data-driven improvement decisions

### For Customers
- Discover top-rated restaurants by category
- Find hidden gem establishments
- Understand common pros and cons
- Make informed dining choices

### For Platform Operators
- Optimize restaurant recommendations
- Identify quality indicators
- Detect market gaps
- Enhance user experience

### For Investors
- Assess restaurant performance
- Identify market opportunities
- Evaluate digital transformation potential
- Risk assessment

##  Project Structure

```
UrbanUmami-An-End-to-End-NLP-Pipeline-for-NYC-Restaurant-Feedback/
│
├── app.ipynb                          # Main analysis notebook
├── requirements.txt                   # Python dependencies
├── README.md                         # Project documentation
├── LICENSE                           # Project license
│
├── trip advisor restaurents 10k - trip_rest_neywork_1.csv  # Original dataset
│
└── Generated outputs:
    ├── restaurant_analysis_with_sentiment.csv
    └── restaurant_analysis_dashboard.png
```

##  Methodology

### Sentiment Analysis Approach
- **Tool**: TextBlob (NLTK-based)
- **Scale**: -1 (very negative) to +1 (very positive)
- **Classification Thresholds**:
  - Positive: score > 0.1
  - Negative: score < -0.1
  - Neutral: -0.1 ≤ score ≤ 0.1

### Statistical Methods
- Correlation analysis (Pearson)
- Independent t-tests for group comparisons
- IQR-based outlier detection
- Min-Max normalization for composite scores

### Text Mining Techniques
- Stopword removal (NLTK English corpus)
- Keyword frequency analysis
- Word cloud visualization
- N-gram extraction (bigrams, trigrams)

##  Limitations

- **Temporal Data**: No time-series analysis (review dates not available)
- **Pricing**: No cost/value analysis
- **Platform Bias**: Single source (TripAdvisor only)
- **Sentiment Nuance**: May miss sarcasm or cultural context
- **Review Authenticity**: Potential fake reviews not filtered

##  Future Enhancements

1. **Predictive Modeling**: Forecast restaurant success based on features
2. **Aspect-Based Sentiment**: Separate scores for food, service, ambiance, etc.
3. **Topic Modeling**: LDA/NMF for theme extraction
4. **Deep Learning**: Transformer-based sentiment (BERT, RoBERTa)
5. **Time-Series Analysis**: Trend detection when temporal data available
6. **Multi-Platform Integration**: Combine Yelp, Google Reviews, etc.
7. **Recommendation System**: Personalized restaurant suggestions

##  Contributing

This is an educational and analytical project. Contributions, suggestions, and feedback are welcome!

##  License

See LICENSE file for details.

##  Acknowledgments

- **Data Source**: TripAdvisor Restaurant Reviews
- **NLP Libraries**: NLTK, TextBlob
- **Visualization**: Matplotlib, Seaborn, WordCloud
- **Analysis Framework**: Pandas, NumPy, SciPy

##  Contact

For questions, suggestions, or collaboration opportunities, please open an issue in the repository.

---

**Built with  for data-driven restaurant intelligence**
