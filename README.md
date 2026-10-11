# 💰 Student Budget Assistant

A smart expense tracker and budget management tool built for students. Track your spending, set budget limits, and get intelligent alerts when you're overspending.

## Features

✨ Core Features:
- 📝 Track expenses and income
- 🎯 Set monthly budget limits by category
- 📊 Real-time spending dashboard
- 💡 Smart alerts for overspending
- 📈 Analytics and spending insights
- 💾 Local SQLite database (no cloud required)

✨ Smart Insights:
- Automatic budget overspending alerts
- Spending category breakdown
- Budget status tracking
- Spending trends
- Money-saving tips by category

## Quick Start

### 1. Clone and Setup

```bash
git clone https://github.com/Grig-Grigorop/student-budget-assistant.git
cd student-budget-assistant
```

### 2. Create Virtual Environment

```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

The app will be available at `http://localhost:5000`

## Usage

### Dashboard
- View your total income, expenses, and balance
- See smart budget alerts
- Track spending by category
- Monitor budget status

### Expenses
- Add daily expenses with category
- Track spending details
- View expense history
- Delete incorrect entries

### Income
- Log income from various sources
- Track payment dates
- View income history

### Budget
- Set monthly budget limits per category
- Available categories:
  - 🍕 Food
  - 🚗 Transport
  - 🎬 Entertainment
  - 📚 Study
  - 💡 Utilities
  - 📦 Other

### Analytics
- View spending distribution
- Analyze spending patterns
- Get money-saving tips
- Track category trends

## Project Structure

```text
student-budget-assistant/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── .gitignore             # Standard ignore rules
├── budget.db             # SQLite database (created automatically)
├── templates/
│   ├── base.html         # Base template with styling
│   ├── dashboard.html    # Dashboard view
│   ├── expenses.html     # Expense tracking
│   ├── income.html       # Income tracking
│   ├── budget.html       # Budget management
│   └── analytics.html    # Analytics and insights
└── README.md
```

## Database Schema

### Expense Table
- `id`: Primary key
- `category`: Expense category
- `amount`: Expense amount
- `description`: Optional description
- `date`: Transaction date

### Income Table
- `id`: Primary key
- `source`: Income source
- `amount`: Income amount
- `date`: Transaction date

### Budget Table
- `id`: Primary key
- `category`: Budget category
- `limit`: Monthly budget limit
- `month`: Month (YYYY-MM format)

## Technology Stack

- Backend: Flask (Python web framework)
- Database: SQLite
- Frontend: HTML, CSS, JavaScript
- Libraries:
  - Flask-SQLAlchemy
  - Pandas
  - Plotly

## Future Enhancements

- 📱 Mobile-responsive design improvements
- 📊 Advanced charts and visualizations
- 🔔 Email/SMS notifications
- 📁 CSV export functionality
- 👤 User authentication and multi-user support
- 📅 Recurring expense tracking
- 🎯 Savings goals
- 💳 Bank account integration
- 📈 Predictive spending analytics
- 🏷️ Transaction tags and custom categories

## Tips for Students

1. Set realistic budgets based on your actual spending
2. Review your dashboard every week
3. Track even small purchases
4. Use category-based budgeting to identify spending patterns
5. Act on alerts early
6. Set aside part of your income for savings

## License

MIT License

## Support

If you find bugs or want to improve the project, feel free to open an issue or contribute via pull request.
