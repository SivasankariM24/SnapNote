# 📝 SnapNote App

> A modern, full-stack note-taking application built with React, Node.js, Express, and MongoDB. Create, organize, and manage your notes with a clean, responsive interface.

![QuickNote Demo](https://img.shields.io/badge/Status-Active-brightgreen)
![Version](https://img.shields.io/badge/Version-1.0.0-blue)

## ✨ Features

- 📄 **Full CRUD Operations** - Create, Read, Update, Delete notes
- ⏰ **Smart Timestamps** - Automatic creation and update tracking
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile
- 🎨 **Modern UI** - Clean, intuitive interface with smooth animations
- ⚡ **Real-time Updates** - Instant note management without page refresh
- ✅ **Form Validation** - Input validation with user-friendly error messages
- 🔒 **Data Persistence** - Secure MongoDB storage
- 🚀 **Fast Performance** - Optimized React components and API calls

## 🛠 Tech Stack

### Frontend
- **React** - UI library for building interactive interfaces
- **Axios** - HTTP client for API requests
- **CSS3** - Modern styling with flexbox and grid
- **JavaScript ES6+** - Modern JavaScript features

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database for data storage
- **Mongoose** - MongoDB object modeling

## 📋 Prerequisites

Before running this application, make sure you have:

- **Node.js** (v14.0.0 or higher) - [Download Here](https://nodejs.org/)
- **MongoDB** (v4.4 or higher) - [Download Here](https://www.mongodb.com/try/download/community)
- **npm** or **yarn** - Package manager (comes with Node.js)

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/SivasankariM24/SnapNote.git
cd quicknote-app
```

### 2. Backend Setup
```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Create environment file
cp .env.example .env

# Start the backend server
npm run dev
```

The backend server will start on `http://localhost:5000`

### 3. Frontend Setup
```bash
# Open new terminal and navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Start the React development server
npm start
```

The frontend application will start on `http://localhost:3000`

### 4. Database Setup
Make sure MongoDB is running on your system:

```bash
# Start MongoDB (varies by OS)
# Windows/Mac: MongoDB Compass or mongod command
# Linux: sudo systemctl start mongod
mongod
```

## 📁 Project Structure

```
quicknote-app/
├── 📂 backend/
│   ├── 📂 config/
│   │   └── database.js          # MongoDB connection
│   ├── 📂 models/
│   │   └── Note.js              # Note schema
│   ├── 📂 routes/
│   │   └── notes.js             # API routes
│   ├── server.js                # Express server
│   ├── package.json             # Backend dependencies
│   └── .env                     # Environment variables
├── 📂 frontend/
│   ├── 📂 public/
│   │   └── index.html           # HTML template
│   ├── 📂 src/
│   │   ├── 📂 components/
│   │   │   ├── NoteForm.js      # Note creation/editing form
│   │   │   ├── NoteItem.js      # Individual note component
│   │   │   └── NoteList.js      # Notes container
│   │   ├── 📂 services/
│   │   │   └── api.js           # API service layer
│   │   ├── App.js               # Main app component
│   │   ├── App.css              # Styles
│   │   └── index.js             # React entry point
│   └── package.json             # Frontend dependencies
└── README.md                    # Project documentation
```

## 🔧 Configuration

### Environment Variables (.env)
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/quicknote
NODE_ENV=development
```

### API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/notes` | Get all notes |
| GET | `/api/notes/:id` | Get single note |
| POST | `/api/notes` | Create new note |
| PUT | `/api/notes/:id` | Update existing note |
| DELETE | `/api/notes/:id` | Delete note |

## 📸 Screenshots

### Desktop View
- Clean, modern interface with sidebar form
- Responsive grid layout for notes
- Smooth hover animations

### Mobile View
- Optimized for touch interactions
- Stacked layout for better mobile experience
- Easy-to-tap buttons and forms

## 🎯 Usage

1. **Creating Notes**: Fill in the title and description, then click "Create Note"
2. **Editing Notes**: Click the "Edit" button on any note to modify it
3. **Deleting Notes**: Click "Delete" and confirm to remove a note
4. **Viewing Notes**: All notes are displayed with creation and update timestamps

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow existing code style and conventions
- Add comments for complex logic
- Test your changes thoroughly
- Update documentation as needed

## 🚧 Roadmap

- [ ] **User Authentication** - Login/register functionality
- [ ] **Categories/Tags** - Organize notes with labels
- [ ] **Search & Filter** - Find notes quickly
- [ ] **Rich Text Editor** - Formatting options
- [ ] **File Attachments** - Add images and documents
- [ ] **Export/Import** - Backup and restore notes
- [ ] **Dark Mode** - Theme switching
- [ ] **Offline Support** - PWA capabilities

## 🐛 Troubleshooting

### Common Issues

**MongoDB Connection Failed**
```bash
# Make sure MongoDB is running
mongod
# Or check if it's running as a service
sudo systemctl status mongod
```

**Port Already in Use**
```bash
# Kill process using the port
lsof -ti:5000 | xargs kill -9
# Or change port in .env file
```

**CORS Errors**
- Ensure backend CORS is configured properly
- Check API base URL in frontend configuration

**Dependencies Issues**
```bash
# Clear npm cache and reinstall
rm -rf node_modules package-lock.json
npm cache clean --force
npm install
```

## 👨‍💻 Author

**Your Name**
- GitHub: [SivasankariM24](https://github.com/SivasankariM24)

## 🙏 Acknowledgments

- [React Documentation](https://reactjs.org/docs) - For excellent React guidance
- [Express.js](https://expressjs.com/) - Fast, unopinionated web framework
- [MongoDB](https://www.mongodb.com/) - Document database platform
- [Mongoose](https://mongoosejs.com/) - Elegant MongoDB object modeling

## 📊 Project Stats

- **Lines of Code**: ~1,500+
- **Components**: 4 React components
- **API Endpoints**: 5 RESTful routes
- **Dependencies**: 10+ npm packages
- **Build Size**: ~200KB (gzipped)

---

<div align="center">

**⭐ If you found this project helpful, please give it a star! ⭐**

Made by [Sivasankari M]

</div>
