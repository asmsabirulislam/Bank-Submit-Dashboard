# 📊 Enterprise Power BI Style Dashboard

A **premium, professional Streamlit dashboard** inspired by **Microsoft Power BI Premium**. This enterprise-grade analytics platform features glassmorphism design, dynamic KPIs, advanced visualizations, and AI-powered insights.

![Dashboard Preview](https://img.shields.io/badge/Streamlit-1.35+-red?style=flat-square)
![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## ✨ Features

### 🎨 **Design & UI**
- ✅ **Glassmorphism Cards** - Modern frosted glass aesthetic
- ✅ **Dark/Light Theme Toggle** - Seamless theme switching
- ✅ **Gradient KPI Cards** - Eye-catching animated metric displays
- ✅ **Smooth Animations** - Professional transitions and effects
- ✅ **Responsive Layout** - Mobile-friendly & fully adaptable
- ✅ **Professional Color Palette** - Corporate enterprise colors
- ✅ **Custom Scrollbars** - Styled UI elements
- ✅ **Shadow Effects** - Depth and dimension

### 📊 **Navigation & Tabs**
12 comprehensive tabs covering all analytics dimensions:

1. **🏠 Executive Dashboard** - High-level KPIs and executive summary
2. **📅 Daily Analysis** - Day-by-day performance metrics
3. **📈 Monthly Analysis** - Monthly trends and patterns
4. **📊 Weekly Analysis** - Weekly breakdowns and heatmaps
5. **🏦 Bank Analysis** - Bank-specific performance metrics
6. **🏢 Firm Analysis** - Firm performance rankings (Sunburst)
7. **👤 Sales Person Analysis** - Sales team leaderboards
8. **👥 Party Analysis** - Party distribution (Treemap)
9. **💰 Payment Analysis** - Payment status & aging analysis
10. **📋 Data Explorer** - Interactive data table with export options
11. **🤖 AI Insights** - Auto-generated insights & 30-day forecast
12. **📄 PDF Report** - Report generation interface

### 🎯 **KPI Cards**
- Total Invoice Value
- Total Submitted
- Total Parties
- Total Banks
- Payment Received
- Pending Payment
- Rejected
- Acceptance Rate
- Average Invoice
- Highest Invoice

Each with:
- Dynamic trend indicators (📈 📉 ➡️)
- Growth percentages
- Gradient backgrounds
- Hover effects

### 🔍 **Sidebar Filters**
- 📅 Date Range Selection
- 🏦 Bank Multi-select
- 🏢 Firm Multi-select
- 👥 Party Selection
- 🛍️ Buyer Selection
- 👤 Sales Person Selection
- ✅ Status Filtering
- 💳 Payment Status
- 💰 Invoice Amount Range
- 🔎 Search Box
- 🔄 Reset Filters Button

### 📈 **Visualizations**
Professional Plotly charts:
- **Line Charts** - Trend analysis with gradient fills
- **Bar Charts** - Comparative metrics
- **Area Charts** - Time series with shading
- **Pie/Donut Charts** - Distribution analysis
- **Heatmaps** - Multi-dimensional patterns
- **Sunburst Charts** - Hierarchical data
- **Treemaps** - Size-based distribution
- **Scatter Plots** - Correlation analysis
- **Funnel Charts** - Process flow analysis

### 📊 **Advanced Analytics**
- **Executive Summary** - Auto-generated key insights
- **Leaderboards** - Top performers ranking
- **Aging Analysis** - Payment aging buckets (0-30, 31-60, 61-90, 90+)
- **Forecasting** - 30-day linear regression forecast
- **Heatmaps** - Day vs Invoice Amount patterns
- **Month vs Firm** - Cross-dimensional analysis
- **Growth Analysis** - Period-over-period comparison

### 🤖 **AI Insights**
Automatically generated intelligence:
- Highest/Lowest performing months
- Top banks and firms
- Top 5 parties and buyers
- Growth trends & declines
- Acceptance percentages
- Payment recovery rates
- Pending/Rejected ratios
- Largest and average invoices

### 💾 **Export & Download**
- 📄 CSV Export
- 📊 Excel (XLSX) Export
- 📋 Interactive Data Explorer
- Column sorting & filtering
- Row customization
- Custom formatting

### ⚡ **Performance**
- ✅ Streamlit Caching (@st.cache_data)
- ✅ Fast loading times
- ✅ Session state management
- ✅ Lazy loading optimization
- ✅ Responsive design
- ✅ Auto-refresh capability

---

## 🚀 Installation

### Prerequisites
- Python 3.9+
- pip package manager

### Step 1: Clone/Download
```bash
# If you have git
git clone <repository-url>
cd powerbi-dashboard

# Or download directly and extract
```

### Step 2: Create Virtual Environment (Optional but Recommended)
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

**Or install manually:**
```bash
pip install streamlit pandas plotly numpy scipy scikit-learn openpyxl
```

**Optional (for PDF export):**
```bash
pip install reportlab
```

### Step 4: Run Dashboard
```bash
streamlit run powerbi_enterprise_dashboard.py
```

The dashboard will open at `http://localhost:8501` in your default browser.

---

## 📋 Requirements

Create a `requirements.txt` file:
```
streamlit>=1.35.0
pandas>=2.0.0
plotly>=5.17.0
numpy>=1.24.0
scipy>=1.10.0
scikit-learn>=1.3.0
openpyxl>=3.1.0
reportlab>=4.0.0
```

---

## 🎯 Usage Guide

### Starting the Dashboard
```bash
streamlit run powerbi_enterprise_dashboard.py
```

### Theme Toggle
- Use the **Theme** radio button in the sidebar
- Choose between "dark" and "light" modes
- Refreshes instantly with new color scheme

### Applying Filters
1. **Date Range**: Select start and end dates
2. **Banks**: Multi-select specific banks
3. **Firms**: Choose relevant firms
4. **Status**: Filter by Accepted/Pending/Rejected
5. **Payment Status**: Received/Pending/Rejected
6. **Advanced**: Click "Advanced Filters" expander
   - Invoice amount range slider
   - Party selection
   - Buyer selection
   - Sales person selection
7. **Search**: Type to search parties or banks
8. **Reset**: Click "Reset All Filters" to clear all

### Navigating Tabs
- Click any tab name to view that analysis
- All filters apply across all tabs
- Each tab auto-updates when filters change

### Tab-Specific Features

#### Executive Dashboard
- View all KPIs at a glance
- See payment distribution donut chart
- Monthly, weekly, and status trends
- Quick performance summary

#### Daily/Weekly/Monthly Analysis
- Trend lines showing performance over time
- Transaction counts
- Distribution charts
- Statistical tables

#### Bank/Firm Analysis
- Comparative performance metrics
- Sunburst and treemap visualizations
- Leaderboards
- Rankings tables

#### Sales Person Analysis
- Sales team leaderboards
- Performance metrics
- Acceptance rates
- Top performer highlighted

#### Payment Analysis
- Payment status breakdown
- Aging analysis (0-30, 31-60, 61-90, 90+ days)
- Payment trends over time
- Recovery rate tracking

#### Data Explorer
- View raw filtered data
- Sort by any column
- Select number of rows to display
- **Export options**:
  - Download CSV
  - Download Excel XLSX

#### AI Insights
- Auto-generated key intelligence
- Monthly performance analysis
- Top performers identification
- Growth/decline metrics
- 30-day forecast chart
- Summary statistics

#### PDF Report
- Custom report title
- Custom description
- Formatted output
- (Requires reportlab library)

### Data Export
1. Navigate to **Data Explorer** tab
2. Customize rows and sorting
3. Click **Download CSV** or **Download Excel**
4. File downloads to your default folder

---

## 🎨 Design System

### Color Palette

**Dark Theme:**
- Primary: `#00d4ff` (Cyan)
- Secondary: `#00ff88` (Neon Green)
- Success: `#2ed573` (Green)
- Warning: `#ffa502` (Orange)
- Danger: `#ff4757` (Red)
- Background: `#0a0e27` (Deep Blue-Black)
- Card: `#15192e` (Dark Blue)

**Light Theme:**
- Primary: `#0066ff` (Blue)
- Secondary: `#00aa44` (Green)
- Success: `#00cc44` (Bright Green)
- Warning: `#ff8800` (Orange)
- Danger: `#ff4444` (Red)
- Background: `#f5f7fb` (Light Gray)
- Card: `#ffffff` (White)

### Typography
- Display: Segoe UI, sans-serif
- Size Scale: 12px (labels) → 32px (values)
- Weight: 600 (medium) → 700 (bold)
- Letter Spacing: 0.05em - 0.1em for labels

### Components
- **Cards**: 16px border radius, glassmorphism effect
- **Buttons**: Gradient background, hover elevation
- **Inputs**: 8px border radius, semi-transparent background
- **Charts**: No background fill, transparent overlays

---

## 📊 Data Structure

The dashboard generates sample data automatically. To use your own data:

1. **Load Your Data**:
   ```python
   data = pd.read_csv('your_data.csv')
   # or
   data = pd.read_excel('your_data.xlsx')
   ```

2. **Required Columns**:
   - `Date` (datetime)
   - `Bank` (string)
   - `Firm` (string)
   - `Party` (string)
   - `Buyer` (string)
   - `Sales Person` (string)
   - `Invoice Value` (numeric)
   - `Status` (Accepted/Pending/Rejected)
   - `Payment Status` (Received/Pending/Rejected)

3. **Replace Data Loading**:
   Look for `generate_sample_data()` function and modify:
   ```python
   @st.cache_data
   def generate_sample_data():
       # Replace with your data loading logic
       data = pd.read_excel('your_file.xlsx')
       return data
   ```

---

## 🔧 Customization

### Change Colors
1. Edit the `THEMES` dictionary in the script
2. Modify hex color codes
3. Update `COLORS_PALETTE` for chart colors

### Add New Metrics
In the KPI cards section:
```python
metric_card("Your Metric", value, change, "icon", "gradient_type")
```

### Add New Charts
Use Plotly's extensive chart library:
```python
fig = go.Figure(data=[...])
fig.update_layout(**get_plotly_config())
st.plotly_chart(fig, use_container_width=True)
```

### Modify Filters
Edit the sidebar filter section to add/remove filter options

---

## 📈 Performance Tips

1. **Caching**: The `@st.cache_data` decorator speeds up data loading
2. **Filter Early**: Apply filters in the SQL query, not in Python
3. **Lazy Loading**: Large datasets benefit from pagination
4. **Session State**: Use `st.session_state` for expensive computations
5. **Columnwise Operations**: Use pandas `.agg()` for multiple aggregations

### Memory Management
```python
# Good - uses memory efficiently
data = data[data['Date'] > threshold]

# Avoid - creates full copy
data_copy = data.copy()  # Only when necessary
```

---

## 🐛 Troubleshooting

### Dashboard Won't Load
```bash
# Clear Streamlit cache
streamlit cache clear

# Run with verbose output
streamlit run powerbi_enterprise_dashboard.py --logger.level=debug
```

### Charts Not Displaying
- Check data columns match expected names
- Verify data types (numeric, datetime)
- Check for null/NaN values

### Theme Not Changing
- Hard refresh browser (Ctrl+Shift+R / Cmd+Shift+R)
- Clear browser cache
- Check JavaScript console for errors

### Memory Issues with Large Data
- Filter data before dashboard load
- Use `.head()` or `.sample()` for testing
- Consider database queries instead of loading all data

---

## 🌐 Deployment

### Streamlit Cloud
1. Push code to GitHub
2. Go to [share.streamlit.io](https://share.streamlit.io)
3. Connect repository
4. Deploy with one click

### Docker
```dockerfile
FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["streamlit", "run", "powerbi_enterprise_dashboard.py"]
```

### Requirements for Deployment
```bash
streamlit>=1.35.0
pandas>=2.0.0
plotly>=5.17.0
numpy>=1.24.0
scipy>=1.10.0
scikit-learn>=1.3.0
openpyxl>=3.1.0
```

---

## 📚 API Reference

### Utility Functions

#### `format_currency(value)`
Formats numbers with K/M notation
```python
format_currency(50000)  # Returns "$50.0K"
```

#### `metric_card(title, value, change, icon, gradient_type)`
Displays a KPI card
```python
metric_card("Revenue", "$1.5M", 15.3, "💵", "success")
```

#### `calculate_change(current, previous)`
Calculates percentage change
```python
calculate_change(100, 80)  # Returns 25.0
```

#### `get_plotly_config()`
Returns consistent Plotly theming
```python
fig.update_layout(**get_plotly_config())
```

---

## 🎓 Learning Resources

- **Streamlit Docs**: [docs.streamlit.io](https://docs.streamlit.io)
- **Plotly Docs**: [plotly.com/python](https://plotly.com/python)
- **Pandas Docs**: [pandas.pydata.org](https://pandas.pydata.org)
- **Power BI Design**: [Microsoft Docs](https://docs.microsoft.com/en-us/power-bi/)

---

## 📄 License

MIT License - Feel free to use and modify for your projects.

---

## 🤝 Contributing

Contributions are welcome! Areas for enhancement:
- Additional chart types
- Real-time data streaming
- Advanced ML forecasting
- Database integration
- Multi-language support
- Performance optimization

---

## 💡 Future Enhancements

- [ ] Real-time data updates
- [ ] Custom metric builder
- [ ] Scheduled report emails
- [ ] Advanced forecasting (Prophet, ARIMA)
- [ ] Data anomaly detection
- [ ] Comparison mode (period-over-period)
- [ ] Bookmark/dashboard sharing
- [ ] Custom filters as URL parameters
- [ ] Dark mode animations
- [ ] Accessibility (WCAG 2.1)

---

## 📞 Support

For issues, questions, or suggestions:
1. Check the Troubleshooting section
2. Review the code comments
3. Check Streamlit community forums
4. Open an issue in the repository

---

## 🎉 Credits

Built with:
- **Streamlit** - App framework
- **Plotly** - Interactive visualizations
- **Pandas** - Data manipulation
- **NumPy/SciPy** - Scientific computing
- **Scikit-learn** - Machine learning

Inspired by **Microsoft Power BI Premium** design language.

---

**Version**: 1.0.0  
**Last Updated**: 2024  
**Status**: Production Ready ✅

---

<div align="center">

### Made with ❤️ for Data-Driven Decision Making

**Star ⭐ if you find this helpful!**

</div>
