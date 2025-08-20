# 🚀 Quick.ai - AI SaaS Platform

A comprehensive AI-powered SaaS application that provides multiple AI services including content generation, image processing, and professional tools. Built with modern technologies and designed for scalability.

## 🛠️ Technologies Used

### Frontend
- **React 18** - Modern UI framework with hooks
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide React** - Beautiful icon library
- **React Markdown** - Markdown rendering for AI content
- **React Router** - Client-side routing
- **Axios** - HTTP client for API calls
- **React Hot Toast** - Toast notifications

### Backend
- **Node.js** - Server runtime environment
- **Express.js** - Web application framework
- **PostgreSQL** - Relational database
- **Clerk** - Authentication and user management
- **Multer** - File upload handling
- **PDF-Parse** - PDF text extraction
- **CORS** - Cross-origin resource sharing

### AI & External Services
- **Google Gemini API** - Text generation and analysis
- **ClipDrop API** - AI image generation
- **Cloudinary** - Image storage and transformations
- **OpenAI SDK** - AI service integration

### Development Tools
- **Vite** - Fast build tool and development server
- **ESLint** - Code linting and formatting
- **Git** - Version control
- **Environment Variables** - Secure configuration management

## 🚀 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- PostgreSQL database
- Clerk account for authentication
- API keys for AI services

### Environment Variables

Create `.env` files in both client and server directories:

#### Server `.env`
```env
# Database
DATABASE_URL=your_postgresql_connection_string

# Authentication
CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

# AI Services
GEMINI_API_KEY=your_google_gemini_api_key
CLIPDROP_API_KEY=your_clipdrop_api_key

# Image Storage
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

# Server Configuration
PORT=3000
```

#### Client `.env`
```env
VITE_BASE_URL=http://localhost:5000
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

### Installation Steps

1. **Clone the repository**
```bash
git clone https://github.com/Ajay-Sapkal/easyprompt-app.git
cd easyprompt-app
```

2. **Install server dependencies**
```bash
cd server
npm install
```

3. **Install client dependencies**
```bash
cd ../client
npm install
```

4. **Set up database**
```bash
# Create PostgreSQL database and tables
# Run migration scripts if available
```

5. **Start development servers**

Terminal 1 (Server):
```bash
cd server
npm run server
```

Terminal 2 (Client):
```bash
cd client
npm run dev
```

6. **Access the application**
- Frontend: `http://localhost:5173`
- Backend: `http://localhost:3000`


## 🏗️ Project Structure

```
quick.ai-app/
├── client/                 # React frontend
│   ├── public/            # Static assets
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Main application pages
│   │   ├── assets/        # Images and static files
│   │   └── main.jsx       # Application entry point
│   ├── package.json
│   └── vite.config.js
├── server/                # Node.js backend
│   ├── controllers/       # Route controllers
│   ├── middleware/        # Custom middleware
│   ├── routes/           # API route definitions
│   ├── uploads/          # File upload directory
│   ├── package.json
│   └── server.js         # Server entry point
└── README.md
```

