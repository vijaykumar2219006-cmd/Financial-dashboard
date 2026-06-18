# Personal Finance Dashboard

A modern, responsive financial dashboard built with React, Vite, and Tailwind CSS. Features real-time analytics, interactive charts, and a beautiful dark/light mode interface.

## Features

- 📊 **Interactive Charts** - Income, expenses, and spending trends visualization using Recharts
- 🎨 **Dark/Light Mode** - Seamless theme switching with persistent storage
- 📱 **Fully Responsive** - Optimized for mobile, tablet, and desktop screens
- 💳 **Analytics Cards** - Key financial metrics with trend indicators
- ⚡ **Built with Vite** - Lightning-fast development and build times
- 🎯 **Tailwind CSS** - Modern, utility-first styling

## Tech Stack

- **React 18** - UI framework
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling framework
- **Recharts** - Charts library
- **Lucide React** - Icon library
- **JavaScript (ES6+)** - Core language

## Project Structure

```
src/
├── components/
│   ├── Header.jsx          # Navigation header with theme toggle
│   ├── AnalyticsCard.jsx   # Reusable analytics metric cards
│   └── Charts.jsx          # Chart components (Line, Area, Bar)
├── context/
│   └── ThemeContext.jsx    # Dark/Light mode state management
├── pages/
│   └── Dashboard.jsx       # Main dashboard layout
├── App.jsx                 # Root component
├── main.jsx                # Application entry point
└── index.css               # Tailwind CSS directives
```

## Getting Started

### Prerequisites

- Node.js 16+ 
- npm or yarn

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

The application will start at `http://localhost:5173`

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Features Breakdown

### Dashboard Page
- Financial overview with total income, expenses, net savings, and savings rate
- Responsive grid layout that adapts to different screen sizes

### Analytics Cards
- Display key metrics with visual icons
- Show trend indicators (up/down) with percentage changes
- Hover effects for better UX

### Charts
1. **Income vs Expenses Chart** - Line chart comparing monthly income and expenses
2. **Spending Trend Chart** - Area chart showing expense trends over time
3. **Spending by Category** - Bar chart breaking down expenses by category

### Theme System
- Automatic detection of system preferences
- Manual toggle button in header
- Persistent storage using localStorage
- Smooth transitions between light and dark modes

## Responsive Design

The dashboard is fully responsive with breakpoints:
- **Mobile**: Single column layout
- **Tablet (md)**: Two column layout for analytics cards
- **Desktop (lg)**: Four column layout for analytics cards with full-width charts

## Customization

### Colors
Edit `tailwind.config.js` to customize the color scheme:
```javascript
theme: {
  extend: {
    colors: {
      // Custom colors here
    }
  }
}
```

### Data
Sample data is currently hardcoded in components. To use real data:
1. Replace mock data in `Dashboard.jsx` and `Charts.jsx`
2. Connect to an API or state management solution
3. Update chart data arrays with real financial data

## Future Enhancements

- Integration with financial APIs
- User authentication
- Transaction history and filtering
- Budget management
- Expense categorization
- Export reports to PDF
- Mobile app version

## License

This project is open source and available under the MIT License.

## Support

For issues or questions, please open an issue in the repository.
