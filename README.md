# 💰 Expense Tracker

A **modern, full-stack expense management application** built with **React** (frontend) and **Node.js + Express + MongoDB** (backend). Track, manage, and categorize your expenses with an intuitive interface and powerful backend API.


## 📋 Project Overview

**Expense Tracker** is a comprehensive web application designed to help users efficiently manage their personal and business expenses. The application features:

- **Frontend:** A responsive React.js interface with Bootstrap styling for a modern user experience
- **Backend:** RESTful API built with Node.js and Express for robust server-side operations
- **Database:** MongoDB for flexible and scalable data storage

### Key Objectives:
- ✅ Provide seamless expense management across all devices
- ✅ Real-time data synchronization between frontend and backend
- ✅ Secure user authentication and authorization
- ✅ Scalable architecture for future enhancements

---

## 🚀 Features

### Frontend Features
- ✅ **Add Expenses** — Create new expense entries with name, amount, and category
- ✅ **Edit Expenses** — Modify existing expense details
- ✅ **Delete Expenses** — Remove unwanted expenses
- ✅ **Real-time Updates** — Instant UI updates without page refresh
- ✅ **Category Management** — Personal, Stocks, Financial, Banking categories
- ✅ **Responsive Design** — Side-by-side layout for desktop, stacked for mobile
- ✅ **Modern UI** — Bootstrap styling with custom CSS animations
- ✅ **Form Validation** — Client-side validation for user inputs
- ✅ **Color-Coded Categories** — Visual distinction with color badges

### Backend Features (To be implemented)
- 🔐 **User Authentication** — Secure login and registration with JWT
- 💾 **Expense CRUD Operations** — Create, Read, Update, Delete expenses via API
- 🔍 **Search & Filter** — Find expenses by date, category, or amount
- 📊 **Analytics** — Monthly/yearly expense summaries and reports
- 📤 **Data Export** — Export expenses as CSV/PDF
- 🔔 **Notifications** — Alert users about budget limits
- 👤 **User Profiles** — Manage user information and preferences

---

## 🛠️ Tech Stack

### Frontend
| Technology | Version | Purpose |
|-----------|---------|---------|
| React.js | 19.1.1 | UI framework |
| Bootstrap | 5.x | CSS framework |
| React Bootstrap | Latest | Bootstrap React components |
| Vite | 7.1.7 | Build tool & dev server |
| ESLint | 9.36.0 | Code quality |
| CSS3 | Latest | Custom styling & animations |

### Backend (To be implemented)
| Technology | Version | Purpose |
|-----------|---------|---------|
| Node.js | 16+ | JavaScript runtime |
| Express.js | 4.x | Web framework |
| MongoDB | 4.4+ | NoSQL database |
| Mongoose | 6.x | MongoDB ODM |
| JWT | 8.x | Authentication |
| Bcrypt | 5.x | Password encryption |
| Cors | Latest | Cross-origin requests |
| Dotenv | Latest | Environment variables |

---

## 📂 Project Structure

```
Expense-Tracker/
├── Frontend/                           # React frontend application
│   ├── src/
│   │   ├── components/
│   │   │   ├── ExpenseFrom.jsx        # Expense form component
│   │   │   ├── ExpenseList.jsx        # Expense list display
│   │   │   └── ExpenseItem.jsx        # Individual expense item with edit/delete
│   │   ├── App.jsx                    # Main app component
│   │   ├── main.jsx                   # Entry point
│   │   ├── index.css                  # Global styles & responsive design
│   │   └── App.css
│   ├── public/
│   │   └── index.html
│   ├── package.json
│   ├── vite.config.js
│   ├── eslint.config.js
│   └── README.md                      # Frontend documentation
│
├── Backend/                            # Node.js/Express backend (To be created)
│   ├── src/
│   │   ├── models/
│   │   │   ├── User.js               # User schema
│   │   │   └── Expense.js            # Expense schema
│   │   ├── routes/
│   │   │   ├── auth.js               # Authentication routes
│   │   │   ├── expenses.js           # Expense CRUD routes
│   │   │   └── users.js              # User routes
│   │   ├── controllers/
│   │   │   ├── authController.js     # Authentication logic
│   │   │   ├── expenseController.js  # Expense logic
│   │   │   └── userController.js     # User logic
│   │   ├── middleware/
│   │   │   ├── auth.js               # Authentication middleware
│   │   │   ├── errorHandler.js       # Error handling middleware
│   │   │   └── validation.js         # Input validation
│   │   ├── config/
│   │   │   └── db.js                 # MongoDB connection
│   │   ├── app.js                    # Express app setup
│   │   └── server.js                 # Server entry point
│   ├── .env.example
│   ├── .gitignore
│   ├── package.json
│   └── README.md                      # Backend documentation
│
└── README.md                           # Project root documentation (This file)
```

---

## 💻 Frontend Setup

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

```bash
# Navigate to Frontend directory
cd Frontend

# Install dependencies
npm install

# Install Bootstrap and React Bootstrap (if not already installed)
npm install react-bootstrap bootstrap
```

### Running Frontend Development Server

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run ESLint
npm run lint
```

**Frontend will be available at:** `http://localhost:5174/`

### Frontend Features
- Modern, responsive UI with Bootstrap
- Side-by-side layout (form left, list right) on desktop
- Mobile-optimized stacked layout on tablets and phones
- Real-time expense updates
- Edit and delete functionality
- Category-based organization

---

## 🔧 Backend Setup (To be implemented)

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- MongoDB (Local or MongoDB Atlas)

### Installation

```bash
# Create Backend directory
mkdir Backend
cd Backend

# Initialize Node.js project
npm init -y

# Install dependencies
npm install express mongoose cors dotenv bcryptjs jsonwebtoken
npm install --save-dev nodemon

# Create folder structure
mkdir -p src/models src/routes src/controllers src/middleware src/config
```

### Required Dependencies

```json
{
  "dependencies": {
    "express": "^4.18.2",
    "mongoose": "^6.8.0",
    "cors": "^2.8.5",
    "dotenv": "^16.0.3",
    "bcryptjs": "^2.4.3",
    "jsonwebtoken": "^9.0.0"
  },
  "devDependencies": {
    "nodemon": "^2.0.20"
  }
}
```

### Package.json Scripts

```json
{
  "scripts": {
    "start": "node src/server.js",
    "dev": "nodemon src/server.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  }
}
```

### Backend Features (To be implemented)
- User authentication with JWT
- CRUD operations for expenses
- MongoDB integration for data persistence
- Input validation and error handling
- CORS configuration for frontend communication

---

## 🔌 API Endpoints

### Authentication Endpoints (Backend)
```
POST   /api/auth/register          Create new user account
POST   /api/auth/login             User login with credentials
POST   /api/auth/logout            User logout
POST   /api/auth/refresh-token     Refresh JWT token
GET    /api/auth/verify            Verify JWT token validity
```

### Expense Endpoints (Backend)
```
GET    /api/expenses               Get all expenses for user
GET    /api/expenses/:id           Get specific expense details
POST   /api/expenses               Create new expense
PUT    /api/expenses/:id           Update expense details
DELETE /api/expenses/:id           Delete expense
GET    /api/expenses/filter        Filter expenses by date/category
```

### User Endpoints (Backend)
```
GET    /api/users/profile          Get user profile
PUT    /api/users/profile          Update user profile
DELETE /api/users/profile          Delete user account
POST   /api/users/change-password  Change password
```

---


## 📝 Frontend Components Overview

### App.jsx
- Main application component
- Manages global expense state
- Handles API communication (will be implemented with backend)
- Props: addExpense, deleteExpense, updateExpense

### ExpenseForm.jsx
- Form for adding new expenses
- Input fields: Name, Amount, Category
- Form validation
- Props: addExpense callback

### ExpenseList.jsx
- Displays all expenses in a scrollable container
- Shows expense details with category badges
- Handles edit and delete operations
- Props: expenses array, edit/delete callbacks

### ExpenseItem.jsx
- Individual expense item with action buttons
- Edit button: Shows inline input for editing
- Delete button: Removes expense
- Save button: Confirms edit

---

## 🎨 Frontend Styling

### Color Scheme
- **Primary:** #6366f1 (Indigo)
- **Success:** #10b981 (Green)
- **Danger:** #ef4444 (Red)
- **Background:** Purple to violet gradient

### Responsive Breakpoints
- **Desktop (>768px):** 2-column layout
- **Tablet (768px):** Single column, stacked
- **Mobile (<480px):** Mobile-optimized

### CSS Classes
```css
.form-container      /* Main form wrapper */
.list-container      /* Expenses list wrapper */
.expense-card        /* Individual expense item */
.btn-add            /* Add expense button */
.btn-edit           /* Edit button */
.btn-delete         /* Delete button */
.btn-save           /* Save edit button */
.expense-type       /* Category badge */
```

---

## 🔐 Security Features (Backend)

- ✅ JWT-based authentication
- ✅ Password encryption with bcryptjs
- ✅ CORS configuration for frontend communication
- ✅ Input validation and sanitization
- ✅ Error handling and logging
- ✅ Environment variables for sensitive data
- ✅ Rate limiting (to be implemented)
- ✅ Data encryption (to be implemented)

---

## 📈 Performance Optimization

### Frontend
- React hooks optimization (useCallback, useMemo)
- Lazy loading components
- CSS minification
- Image optimization
- Vite's fast build process

### Backend (To be implemented)
- Database indexing
- Pagination for large datasets
- Caching strategies
- API response compression
- Query optimization

---

## 📚 Future Enhancements

- [ ] User authentication system
- [ ] Multi-user support
- [ ] Budget tracking and alerts
- [ ] Expense categories with custom icons
- [ ] Monthly/yearly reports and analytics
- [ ] Data export (CSV, PDF)
- [ ] Dark mode toggle
- [ ] Expense receipts/attachments
- [ ] Recurring expenses
- [ ] Multi-currency support
- [ ] Mobile app (React Native)
- [ ] Email notifications
- [ ] Integration with payment gateways
- [ ] Advanced filtering and search
- [ ] Social sharing features

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Write clean, readable code
- Follow the existing project structure
- Comment complex logic
- Test your changes before submitting
- Update documentation as needed

---

## 📄 License

This project is open source and available under the MIT License.

---

## 👨‍💻 Author

**Mukul Singh**
- GitHub: [@mukulsingh24](https://github.com/mukulsingh24)
- Email: your.email@example.com

---

## 📞 Support

For issues, questions, or suggestions, please create an issue on GitHub or contact the author.

---

## 🙏 Acknowledgments

- React.js community
- Bootstrap documentation
- MongoDB documentation
- Express.js guides
- Contributors and users

---

**Last Updated:** October 30, 2025

**Status:** 🟡 Frontend Complete | 🔴 Backend Pending

---

## Quick Links

- [Frontend README](./Frontend/README.md)
- [Backend README](./Backend/README.md) (To be created)
- [GitHub Repository](https://github.com/mukulsingh24/Expense-Tracker)
- [Live Demo](https://expense-tracker-demo.netlify.app) (When deployed)
