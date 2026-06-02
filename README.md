# Enhanced Indian Railways

A comprehensive full-stack dashboard application for managing and visualizing Indian Railways data. This project combines a modern React + TypeScript frontend with an Express.js backend API, providing analytics, user management, and data processing capabilities.

## 🎯 Project Overview

The Enhanced Indian Railways application is built with:

- **Frontend**: React 19 with TypeScript, Vite, and Tailwind CSS
- **Backend**: Express.js with MySQL database and Supabase integration
- **Architecture**: Full-stack MERN-style application with file upload and JWT authentication

### Key Features

- 📊 **Analytics Dashboard**: Interactive charts and metrics using ApexCharts
- 🗺️ **Geographic Visualization**: Interactive India map with location data
- 📅 **Calendar Integration**: FullCalendar for event management
- 👥 **User Management**: User profiles, authentication, and role-based access
- 📁 **File Upload**: Excel file processing and data import
- 🔒 **Authentication**: JWT-based secure authentication
- 🎨 **Responsive UI**: Beautiful, responsive dashboard with Tailwind CSS
- 📱 **Mobile Compatible**: Fully responsive design across all devices

## 📁 Project Structure

```
Enhanced-Indian-Railways/
├── frontend/                    # React + TypeScript application
│   ├── src/
│   │   ├── components/         # Reusable React components
│   │   ├── pages/              # Page components
│   │   ├── context/            # React context (Theme, Sidebar)
│   │   ├── hooks/              # Custom React hooks
│   │   ├── layout/             # Layout components
│   │   ├── icons/              # Icon definitions
│   │   ├── App.tsx             # Main App component
│   │   └── main.tsx            # Entry point
│   ├── public/                 # Static assets
│   ├── package.json            # Frontend dependencies
│   ├── vite.config.ts          # Vite configuration
│   └── tsconfig.json           # TypeScript configuration
│
└── backend/                     # Express.js server
    ├── server.js               # Main server file
    ├── mysqlServer.js          # MySQL database configuration
    └── package.json            # Backend dependencies
```

## 🚀 Getting Started

### Prerequisites

- **Node.js**: v18 or higher
- **npm**: v9 or higher
- **MySQL**: v8.0 or higher
- **.env file**: Required for environment variables (see setup below)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Yuvrajg2107/railways-bform.git
   cd Enhanced-Indian-Railways
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd frontend
   npm install
   cd ..
   ```

3. **Install Backend Dependencies**
   ```bash
   cd backend
   npm install
   cd ..
   ```

### Configuration

1. **Create `.env` file in the backend folder**
   ```
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=root@123
   DB_NAME=Railways
   JWT_SECRET=your_secret_key_here
   SUPABASE_URL=your_supabase_url
   SUPABASE_KEY=your_supabase_key
   PORT=3002
   ```

2. **Create `.env` file in the frontend folder**
   ```
   VITE_API_URL=http://localhost:3002
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_KEY=your_supabase_key
   ```

3. **Setup MySQL Database**
   ```bash
   mysql -u root -p
   CREATE DATABASE Railways;
   ```

### Development

1. **Start Backend Server**
   ```bash
   cd backend
   npm start
   # Server runs on http://localhost:3002
   ```

2. **Start Frontend Development Server** (in a new terminal)
   ```bash
   cd frontend
   npm run dev
   # Application runs on http://localhost:5173
   ```

### Build for Production

1. **Build Frontend**
   ```bash
   cd frontend
   npm run build
   ```

2. **Run Backend in Production**
   ```bash
   cd backend
   npm start
   ```

## 🛠️ Technologies & Dependencies

### Frontend
- **React 19** - UI framework
- **TypeScript** - Type safety
- **Vite** - Fast build tool
- **Tailwind CSS** - Utility-first CSS
- **React Router v7** - Client-side routing
- **ApexCharts** - Data visualization
- **FullCalendar** - Calendar functionality
- **react-jvectormap** - Interactive maps
- **Framer Motion** - Animations
- **React Hook Form** - Form management
- **Axios** - HTTP client

### Backend
- **Express.js** - Web framework
- **MySQL2** - MySQL database driver
- **JWT** - Authentication
- **Multer** - File upload handling
- **Supabase** - Backend-as-a-service
- **CORS** - Cross-origin resource sharing
- **XLSX** - Excel file processing
- **Node Cache** - In-memory caching

## 📚 API Documentation

### Authentication Endpoints
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `POST /api/auth/logout` - User logout

### File Upload
- `POST /api/upload` - Upload Excel files

### Data Endpoints
- `GET /api/data` - Fetch data
- `POST /api/data` - Create data
- `PUT /api/data/:id` - Update data
- `DELETE /api/data/:id` - Delete data

## 🧪 Testing

```bash
# Frontend linting
cd frontend
npm run lint

# Build frontend
npm run build

# Preview production build
npm run preview
```

## 📝 Scripts

### Frontend Scripts
```json
{
  "dev": "Start development server",
  "build": "Build for production",
  "lint": "Run ESLint",
  "preview": "Preview production build"
}
```

### Backend Scripts
```bash
npm start   # Start the server
npm dev     # Start with nodemon (if configured)
```

## 🔐 Security Features

- **JWT Authentication** - Secure token-based authentication
- **CORS Protection** - Cross-origin request validation
- **File Upload Validation** - Only Excel files allowed
- **Environment Variables** - Sensitive data in .env files
- **Password Protection** - Database password encryption

## 📊 Database Schema

The application uses MySQL with the following main tables:
- **users** - User accounts and authentication
- **railways** - Railway station and line data
- **bookings** - Passenger bookings
- **transactions** - Payment transactions
- **analytics** - Dashboard metrics and statistics

## 🚢 Deployment

### Frontend Deployment (Vercel/Netlify)
```bash
cd frontend
npm run build
# Deploy the 'dist' folder
```

### Backend Deployment (Heroku/Railway.app)
```bash
cd backend
# Configure environment variables on deployment platform
npm start
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Yuvraj Gupta**
- GitHub: [@Yuvrajg2107](https://github.com/Yuvrajg2107)
- Repository: [railways-bform](https://github.com/Yuvrajg2107/railways-bform)

## 🙏 Acknowledgments

- **TailAdmin** - React Tailwind Admin Dashboard Template
- **React** - JavaScript library for building user interfaces
- **Tailwind CSS** - Utility-first CSS framework
- **Express.js** - Fast and flexible Node.js framework

## 📧 Support & Contact

For issues, questions, or suggestions, please:
1. Check existing [GitHub Issues](https://github.com/Yuvrajg2107/railways-bform/issues)
2. Create a new issue with detailed description
3. Submit a pull request with improvements

## 🗺️ Roadmap

- [ ] Mobile app version
- [ ] Real-time notifications
- [ ] Advanced analytics
- [ ] Multi-language support
- [ ] Payment gateway integration
- [ ] API documentation (Swagger)
- [ ] Unit and integration tests
- [ ] Docker containerization

## 📈 Project Stats

- **Technologies**: 20+
- **Components**: 30+
- **Pages**: 10+
- **API Endpoints**: 15+
- **Lines of Code**: 5000+

---

**Last Updated**: June 2, 2026
**Version**: 1.0.0
