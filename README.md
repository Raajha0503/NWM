# Barclays Network Management Portal

A comprehensive web application for managing Barclays network operations, account creation, workflow processing, and data reconciliation.

## 🚀 Features

### Core Functionality
- **Account Management**: Create and manage agent bank accounts with LEI validation
- **Workflow Processing**: Handle pending account requests and document assignments
- **Data Reconciliation**: Compare CSV files and identify mismatches
- **Admin Dashboard**: Monitor system statistics and interconnection metrics
- **User Authentication**: Secure Firebase-based authentication system
- **Audit Logging**: Comprehensive audit trail for all operations

### Technical Features
- **Responsive Design**: Modern UI with Tailwind CSS
- **Real-time Updates**: Firebase Firestore integration
- **Data Visualization**: Chart.js integration for analytics
- **CSV Processing**: PapaParse for file handling
- **Dark/Light Mode**: Toggle between themes
- **Progress Indicators**: Enhanced user experience with loading states

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Tailwind CSS
- **Backend**: Firebase (Firestore, Authentication)
- **Charts**: Chart.js
- **CSV Processing**: PapaParse
- **Development**: Live Server

## 📋 Prerequisites

- Node.js (>= 14.0.0)
- npm (>= 6.0.0)
- Modern web browser
- Firebase project setup

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/barclays/network-management-portal.git
cd network-management-portal
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Start Development Server
```bash
npm start
```

The application will open automatically in your default browser at `http://localhost:3000`.

## 🔧 Available Scripts

- `npm start` - Start development server with live reload
- `npm run dev` - Start development server with file watching
- `npm run serve` - Start Python HTTP server
- `npm run serve-node` - Start Node.js HTTP server
- `npm run lint` - Run ESLint for code quality
- `npm run format` - Format code with Prettier

## 📁 Project Structure

```
NWM/
├── index.html              # Main application file
├── package.json            # Project dependencies and scripts
├── README.md              # Project documentation
└── .gitignore             # Git ignore rules
```

## 🔐 Firebase Configuration

The application requires Firebase configuration. Update the Firebase config in `index.html`:

```javascript
const firebaseConfig = {
  apiKey: "your-api-key",
  authDomain: "your-project.firebaseapp.com",
  projectId: "your-project-id",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "your-sender-id",
  appId: "your-app-id",
  measurementId: "your-measurement-id"
};
```

## 🗄️ Database Collections

### Firestore Collections
- `accounts` - Agent bank account information
- `requests` - Account creation requests
- `workflow` - Workflow processing data
- `reconciliation` - Data reconciliation records
- `audit_logs` - System audit trail
- `users` - User authentication data
- `counters` - Auto-increment counters

## 🔑 Admin Access

Admin functionality requires the passkey: `barclays2024`

## 🎨 UI Components

### Color Scheme
- **Primary Blue**: `#00AEEF`
- **Dark Blue**: `#0077A3`
- **Cyan**: `#00C1D5`
- **Background**: `#10151A`
- **Surface**: `#1A222B`
- **Text**: `#E6F6FB`

### Status Indicators
- **Active**: Green gradient
- **Inactive**: Red gradient
- **Pending**: Yellow gradient
- **Closed**: Gray gradient

## 📊 Features Overview

### Account Management
- Create new agent bank accounts
- Auto-generate account IDs (BARC-C0001 format)
- LEI validation and storage
- Account status tracking
- Bulk operations support

### Workflow Processing
- Pending request management
- Document assignment
- Status tracking
- Unified data processing

### Data Reconciliation
- CSV file comparison
- Visual diff display
- Batch processing
- Mismatch highlighting

### Admin Dashboard
- System statistics
- Interconnection metrics
- Recent activity tracking
- Performance monitoring

## 🔒 Security Features

- Firebase Authentication
- Role-based access control
- Admin passkey protection
- Audit logging
- Input validation

## 🚀 Deployment

### Static Hosting
The application can be deployed to any static hosting service:

1. **Firebase Hosting**
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

2. **Netlify**
- Connect your repository
- Set build command: `echo "No build required"`
- Set publish directory: `.`

3. **Vercel**
- Import your repository
- Framework preset: Other
- Build command: `echo "No build required"`

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support and questions:
- Create an issue in the GitHub repository
- Contact the development team
- Check the Firebase console for backend issues

## 🔄 Version History

- **v1.0.0** - Initial release with core functionality
  - Account management
  - Workflow processing
  - Data reconciliation
  - Admin dashboard
  - User authentication

---

**Note**: This application is designed for Barclays internal use and contains sensitive business logic. Ensure proper security measures are in place before deployment. 