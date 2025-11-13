# 🏠 Mortgage Calculator

A comprehensive mortgage calculation tool built with Streamlit that helps users estimate their monthly mortgage payments, understand amortization schedules, and make informed decisions about home financing.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://mortgage-calculato4.streamlit.app/)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [How It Works](#how-it-works)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 Overview

This Mortgage Calculator is designed to help prospective homebuyers, real estate investors, and financial planners calculate mortgage payments with precision. The application provides detailed breakdowns of principal, interest, taxes, insurance, and total monthly payments.

### Key Benefits

- **Easy to Use**: Intuitive interface requiring no financial expertise
- **Comprehensive Calculations**: Detailed breakdowns of all payment components
- **Visual Analytics**: Charts and graphs for better understanding
- **Instant Results**: Real-time calculations as you adjust parameters
- **Accessible**: Web-based application accessible from any device

## ✨ Features

### Core Functionality

- **Monthly Payment Calculator**: Calculate monthly mortgage payments based on:
  - Loan amount (principal)
  - Interest rate
  - Loan term (years)
  - Down payment

- **Amortization Schedule**: 
  - Detailed payment breakdown over the life of the loan
  - Principal vs. interest visualization
  - Year-by-year summary
  - Cumulative interest paid

- **Additional Costs**:
  - Property taxes
  - Home insurance
  - HOA fees
  - PMI (Private Mortgage Insurance)

- **Visual Representations**:
  - Interactive charts showing payment distribution
  - Amortization graphs
  - Total cost comparison
  - Equity buildup visualization

- **Comparison Tools**:
  - Compare different loan scenarios
  - Rent vs. buy analysis
  - Impact of extra payments
  - Different down payment scenarios

## 🚀 Demo

Visit the live application: [https://mortgage-calculato4.streamlit.app/](https://mortgage-calculato4.streamlit.app/)

## 🔧 Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Local Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/mortgage-calculator.git
cd mortgage-calculator
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Run the application:
```bash
streamlit run app.py
```

5. Open your browser and navigate to:
```
http://localhost:8501
```

## 📦 Requirements

Create a `requirements.txt` file with the following dependencies:

```
streamlit>=1.28.0
pandas>=2.0.0
numpy>=1.24.0
plotly>=5.14.0
matplotlib>=3.7.0
```

## 💻 Usage

### Basic Calculation

1. **Enter Loan Details**:
   - Home price
   - Down payment ($ or %)
   - Loan term (years)
   - Interest rate (%)

2. **Add Optional Costs**:
   - Property tax (annual)
   - Home insurance (annual)
   - HOA fees (monthly)
   - PMI (if down payment < 20%)

3. **View Results**:
   - Monthly payment breakdown
   - Total cost over loan term
   - Amortization schedule
   - Visual charts

### Advanced Features

- **Extra Payments**: Calculate how additional monthly or annual payments affect your loan
- **Scenario Comparison**: Compare multiple loan scenarios side-by-side
- **Export Data**: Download amortization schedule as CSV
- **Share Results**: Generate shareable calculation links

## 🛠️ Technologies Used

- **[Streamlit](https://streamlit.io/)**: Web application framework
- **[Python](https://www.python.org/)**: Core programming language
- **[Pandas](https://pandas.pydata.org/)**: Data manipulation and analysis
- **[NumPy](https://numpy.org/)**: Numerical computing
- **[Plotly](https://plotly.com/)**: Interactive visualizations
- **[Matplotlib](https://matplotlib.org/)**: Additional plotting capabilities

## 📊 How It Works

### Mortgage Payment Formula

The calculator uses the standard mortgage payment formula:

```
M = P [ i(1 + i)^n ] / [ (1 + i)^n – 1 ]
```

Where:
- **M** = Monthly payment
- **P** = Principal loan amount
- **i** = Monthly interest rate (annual rate / 12)
- **n** = Number of payments (years × 12)

### Amortization Calculation

For each payment period:
1. Calculate interest: `Previous Balance × Monthly Interest Rate`
2. Calculate principal: `Monthly Payment - Interest`
3. Update balance: `Previous Balance - Principal`

## 📸 Screenshots

<img width="1918" height="857" alt="Image" src="https://github.com/user-attachments/assets/c9642f97-30bf-4884-af57-2e59b7f9155d" />

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines

- Follow PEP 8 style guidelines
- Add comments for complex calculations
- Update documentation for new features
- Test thoroughly before submitting

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Contact

**Your Name**
- GitHub: https://github.com/heerr2005
- Email: heerchotaliya78@gmail.com
- LinkedIn: www.linkedin.com/in/heerchotaliya

## 🙏 Acknowledgments

- Streamlit team for the amazing framework
- Contributors and users who provide feedback
- Financial formulas reference from [Wikipedia](https://en.wikipedia.org/wiki/Mortgage_calculator)

## 📈 Future Enhancements

- [ ] Multi-currency support
- [ ] Export to PDF reports
- [ ] Mobile app version
- [ ] Integration with real estate APIs
- [ ] Refinancing calculator
- [ ] Tax deduction calculations
- [ ] Comparison with historical rates
- [ ] Email report functionality

## 🐛 Known Issues

- None currently reported

## 📚 Additional Resources

- [How Mortgages Work](https://www.investopedia.com/mortgage-4689703)
- [Understanding Amortization](https://www.investopedia.com/terms/a/amortization.asp)
- [Streamlit Documentation](https://docs.streamlit.io/)

---

**⭐ If you find this project helpful, please consider giving it a star on GitHub!**

*Last Updated: November 2025*
