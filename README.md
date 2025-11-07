# 💰 Expense Tracker

A **modern, full-stack expense management application** built with **React** (frontend) and **Node.js + Express + MongoDB** (backend). Track, manage, and categorize your expenses with an intuitive interface and powerful backend API.
<<<<<<< HEAD

=======
---
>>>>>>> d3e1bcce3ff269a39ab8f1207a756f0089d13494

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

**Frontend will be available at:** `expensetracker9.vercel.app/`

### Frontend Features
- Modern, responsive UI with Bootstrap
- Side-by-side layout (form left, list right) on desktop
- Mobile-optimized stacked layout on tablets and phones
- Real-time expense updates
- Edit and delete functionality
- Category-based organization

---

<<<<<<< HEAD
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

=======
>>>>>>> d3e1bcce3ff269a39ab8f1207a756f0089d13494
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



## 👨‍💻 Author

**Mukul Singh**
- GitHub: [@mukulsingh24](https://github.com/mukulsingh24)
- Email: rmks1004@example.com

---

## 📞 Support

For issues, questions, or suggestions, please create an issue on GitHub or contact the author.

---


**Last Updated:** October 30, 2025

**Status:** 🟡 Frontend Complete | 🔴 Backend Pending
