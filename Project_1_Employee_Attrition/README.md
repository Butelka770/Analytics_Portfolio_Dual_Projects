# 📊 Employee Attrition & Retention Analysis

**Quick Snapshot:**

- Explore **employee attrition patterns** using workforce demographics, compensation, and tenure data
- Demonstrate end-to-end workforce analytics: **EDA, statistical analysis, interactive visualization, and actionable HR insights**

### **🔗 Live Interactive Dashboard**
View the full interactive experience on [Tableau Public](https://public.tableau.com/shared/FF83FP5W4?:display_count=n&:origin=viz_share_link) 

---

## 📌 Project Overview

This project applies statistical analysis and data visualization to examine workforce dynamics and identify factors influencing employee attrition at Company A. Using employee demographic, compensation, and tenure data, it uncovers high-risk employee segments and generates actionable HR insights through Python-based EDA and an interactive Tableau dashboard.


**This project focuses on:**
- Workforce demographic and compensation analysis
- Income distribution and tenure-based trends
- Identification of high-risk attrition segments
- Interactive visualization of attrition patterns using Tableau
- Translation of analytical findings into HR recommendations

---

## 🎯 Background

Employee attrition analysis is critical for:
- **Talent retention strategy** – Reduce turnover costs
- **HR planning** – Predict workforce needs
- **Compensation optimization** – Ensure fair pay structures
- **Employee satisfaction** – Identify improvement areas

Understanding attrition drivers helps organizations:
- **Save costs** – Replacement costs average 50-200% of annual salary
- **Retain top talent** – Targeted interventions for high-risk groups
- **Improve culture** – Address systemic issues affecting morale

---

## 🗂️ Dataset Overview

**Source:** Provided by Data Science Bootcamp (1,470 records)

**Description:** Employee data including demographics, job information, compensation, and attrition status

**Key Features:**
- **Demographics:** Age, Gender, Marital Status, Education
- **Job Information:** Department, Job Role, Job Level
- **Compensation:** Monthly Income, Stock Options, Percent Salary Hike
- **Tenure Metrics:** Years at Company, Years in Role, Years Since Last Promotion
- **Work Environment:** Work-Life Balance, Overtime, Distance from Home
- **Attrition Status:** Binary indicator (Yes/No)

**Problem Type:** Exploratory Data Analysis + Predictive Insights

> **⚠️ Disclaimer**  
> This dataset was provided by Data Science Bootcamp for educational purposes only. The analysis and recommendations are based on this specific dataset and are intended to demonstrate analytical techniques rather than represent any real organization.

---

## 🛠️ Tools I Used

**Programming & Libraries:**
- **Python** – Data manipulation and analysis
- **Pandas, NumPy** – Data processing
- **Matplotlib, Seaborn** – Statistical visualization
- **Scipy** – Statistical analysis
- **Tableau Public** – Interactive dashboards

**Development Environment:**
- **Jupyter Notebook** – Interactive development and analysis
- **Google Colab** – Optional cloud-based notebook environment

---

## 🚀 Getting Started

### Prerequisites

* Python 3.x or higher
* Jupyter Notebook
* Tableau Public (for dashboard viewing)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/NadiaRozman/analytics-portfolio-dual-projects.git
   cd analytics-portfolio-dual-projects/project-1-employee-attrition
   ```

2. **Install dependencies:**

   ```bash
   pip install pandas numpy matplotlib seaborn scipy jupyter
   ```

3. **Open and run the notebook**

   * Navigate to `attrition_analysis.ipynb`
   * Ensure `employee_data.csv` exists in the same directory
   * Run all cells sequentially

4. **View Tableau Dashboard**

   * **Live Dashboard:** [Employee Attrition Analysis](https://public.tableau.com/shared/FF83FP5W4?:display_count=n&:origin=viz_share_link) 

---

## 🔬 Analysis Implementation

### **Statistical Analysis (Python)**

**1. Data Exploration:**
   - Dataset dimensions and structure
   - Missing value analysis
   - Descriptive statistics for key metrics

**2. Income Analysis:**
   - Distribution analysis with histogram and KDE
   - Skewness calculation and interpretation
   - Salary range and concentration patterns

**3. Correlation Analysis:**
   - Pearson correlation between tenure and income
   - Multi-variable correlation matrix
   - Scatter plot visualization with job level encoding

**4. Key Metrics Calculated:**
   - Average Age: **36.92 years**
   - Average Monthly Income: **$6,502.93**
   - Average Tenure: **7.01 years**
   - Income Range: **$1,009 - $19,999**
   - Tenure-Income Correlation: **r = 0.51** (moderate positive)

### **Interactive Dashboard (Tableau)**

**Dashboard Components:**

1. **Summary View:**
   - Total headcount and attrition metrics
   - Work-life balance impact visualization
   - Age demographics and attrition rates
   - Commute distance analysis
   - Tenure-based attrition trends

2. **Department Deep Dive:**
   - Attrition by department
   - High-risk roles identification
   - Career stagnation vs retention status
   - Interactive filtering and drill-down

---

## 📊 Key Findings

### **Income Structure Analysis**

**1. Workforce Demographics**
- Average age: **36.92 years**
- Average tenure: **7.01 years**
- Wide income range reflects hierarchical structure

**2. Income Distribution Pattern**
- **Right-skewed distribution** – Most employees in lower-to-middle income bands
- Most frequent income range: **$2,000 - $5,000**
- High earners (>$15,000) represent small percentage

**3. Tenure-Income Relationship**
- **Moderate positive correlation (r = 0.51)**
- Longer tenure generally associates with higher income
- However, relationship is NOT perfectly linear
- Job level is a stronger predictor than tenure alone

**Visualization:**

![Monthly Income Distribution](images/1_income_distribution.png)
*Figure 1: Right-skewed income distribution with concentration in $2,000-$5,000 range*

![Tenure vs Income](images/2_tenure_income_relationship.png)
*Figure 2: Scatter plot showing relationship between years at company and income, colored by job level*


### **Attrition Insights (Tableau Dashboard)**

**Critical Metrics:**
- **Total Headcount:** 1,470 employees
- **Lost Talent:** 237 employees
- **Overall Attrition Rate:** 16.12%

**Key Attrition Drivers:**

| Risk Factor | Impact | Finding |
|-------------|--------|---------|
| **Work-Life Balance** | +45.5% | Poor balance increases attrition risk dramatically |
| **Age Demographics** | 3x higher | Employees under 20 show 58.8% attrition rate |
| **Commute Distance** | 25.6% | Long commutes (20km+) correlate with turnover |
| **Early Tenure** | Peak risk | Years 0-2 show highest attrition (onboarding critical) |
| **Career Stagnation** | High risk | 5+ years without promotion increases departures |

**Dashboard Visualizations:**

![Tableau Dashboard Summary](images/3_tableau_main_dashboard.png)
*Figure 4: Interactive dashboard showing attrition rate and key risk factors*

![Department Deep Dive](images/4_tableau_department_view.png)
*Figure 5: Detailed analysis by department, role, and career stagnation patterns*

**Department-Specific Findings:**

| Department | Attrition Rate | Key Insight |
|------------|----------------|-------------|
| **Sales** | 20.63% | Highest departmental attrition |
| **Human Resources** | 19.05% | Second highest turnover |
| **Research & Development** | 13.84% | Below average attrition |

**Role-Specific Findings:**

| Job Role | Attrition Rate | Priority |
|----------|----------------|----------|
| **Sales Representatives** | 39.76% | 🔴 Critical |
| **Laboratory Technicians** | 23.94% | 🟡 High |
| **Human Resources** | 23.08% | 🟡 High |
| **Research Directors** | 2.50% | 🟢 Low |

---

## 💡 Strategic Recommendations

### **High-Priority Actions (🔴)**

#### 1. Enhance Work-Life Balance
**Issue:** Poor work-life balance increases attrition risk by 45.5%

**Actions:**
- Implement flexible work arrangements (hybrid/remote options)
- Monitor and reduce excessive overtime
- Create clear boundaries for after-hours communication
- Conduct regular work-life balance surveys

**Expected Impact:** 15-20% reduction in attrition

---

#### 2. Strengthen Early Career Support
**Issue:** Peak attrition in years 0-2 (onboarding phase)

**Actions:**
- Enhanced onboarding program with structured 90-day milestones
- Assign mentors to all new hires
- Regular check-ins at 30, 60, 90, and 180 days
- Create peer support networks for new employees

**Expected Impact:** 25% reduction in early-tenure attrition

---

#### 3. Address Sales Department Challenges
**Issue:** Sales shows 20.63% attrition, Sales Representatives at 39.76%

**Actions:**
- Review compensation structure and commission plans
- Assess quota reasonableness and territory assignments
- Improve sales support systems and resources
- Conduct exit interviews to identify specific pain points

**Expected Impact:** Reduce Sales attrition to company average

---

### **Medium-Priority Actions (🟡)**

#### 1. Geographic Flexibility
**Issue:** Long commutes (20km+) lead to 25.6% attrition

**Actions:**
- Offer remote/hybrid work options
- Consider satellite offices in high-employee-density areas
- Provide transportation subsidies or relocation assistance

**Expected Impact:** Improved retention for remote employees

---

#### 2. Career Development Programs
**Issue:** High concentration of departures among employees with 5+ years since last promotion

**Actions:**
- Create transparent promotion pathways and timelines
- Implement annual career development discussions
- Offer skill development programs aligned with advancement
- Ensure promotions occur within reasonable timeframes

**Expected Impact:** Reduced career stagnation-related attrition

---

#### 3. Young Employee Retention
**Issue:** Employees under 20 have 3x higher attrition (58.8%)

**Actions:**
- Develop specialized early-career programs
- Provide competitive entry-level compensation
- Create clear growth trajectories for junior roles
- Offer education assistance programs

**Expected Impact:** 30% reduction in under-20 attrition

---

### **Ongoing Initiatives (🟢)**

#### Role-Based Compensation Progression
**Finding:** Job level drives income more than tenure

**Actions:**
- Ensure pay equity within job levels
- Communicate compensation philosophy transparently
- Focus on clear role advancement rather than tenure-based increases

**Expected Impact:** Improved perception of fair compensation

---

## 📈 Implementation Roadmap

| Priority | Action | Target Metric | Timeline | Owner |
|----------|--------|---------------|----------|-------|
| 🔴 | Flexible work policy | -15% attrition | 2-3 months | HR/Leadership |
| 🔴 | Enhanced onboarding | -25% yr 0-2 attrition | 1-2 months | HR/Managers |
| 🔴 | Sales dept review | Reduce to 16% | 3-6 months | Sales Leadership |
| 🟡 | Remote work expansion | -20% commute attrition | 2-4 months | HR/IT |
| 🟡 | Career development | 5+ yrs promo rate | 3-6 months | HR/Management |
| 🟡 | Young employee programs | -30% <20 attrition | 3-4 months | HR |
| 🟢 | Compensation transparency | Employee satisfaction | Ongoing | HR/Finance |

---

## 📚 What I Learned

### **Technical Skills**
- Exploratory data analysis with pandas and NumPy
- Statistical correlation analysis and interpretation
- Data visualization with matplotlib and seaborn
- Interactive dashboard creation in Tableau
- Translating technical findings into business insights

### **Domain Knowledge**
- HR metrics and workforce analytics
- Attrition cost calculation and impact
- Compensation structure analysis
- Employee lifecycle management
- Retention strategy development

### **Analytical Thinking**
- How to identify patterns in workforce data
- Correlation vs causation in HR analytics
- The importance of segmentation (department, role, demographics)
- How multiple factors interact to influence attrition

---

## 🔮 Future Enhancements

- **Predictive modeling** – Build ML model to predict attrition risk
- **Survival analysis** – Time-to-attrition modeling with Cox regression
- **Sentiment analysis** – Analyze exit interview text data
- **Real-time dashboard** – Automated data refresh and alerting
- **A/B testing** – Measure impact of retention interventions
- **External benchmarking** – Compare metrics with industry standards

---

### ✨ Created by Nadia Rozman | January 2026

📂 **Project Structure**
```
Project_1_Employee_Attrition/
│
├── employee_data.csv              
├── Attrition_Analysis.ipynb       
├── README.md                       
│
└── images/                         
    ├── 1_income_distribution.png
    ├── 2_tenure_income_relationship.png
    ├── 3_tableau_main_dashboard.png
    └── 4_tableau_department_view.png
```

**🔗 Connect with me**
- GitHub: [@NadiaRozman](https://github.com/NadiaRozman)
- LinkedIn: [Nadia Rozman](https://www.linkedin.com/in/nadia-rozman-4b4887179/)

**⭐ If you found this project helpful, please consider giving it a star!**

---

**Part of:** [Analytics Portfolio - Dual Projects](https://github.com/NadiaRozman/Analytics_Portfolio_Dual_Projects) 
