# Revolt Motors AI Voice Assistant

A real-time AI voice assistant specifically designed for Revolt Motors, an Indian electric motorcycle company. The assistant provides information about Revolt's electric bikes, features, pricing, dealerships, and more through natural voice conversations.

## 🚀 Features

- **Real-time Voice Interaction**: Speak naturally with the AI assistant
- **Revolt Motors Focus**: Specialized knowledge about Revolt electric motorcycles
- **WebSocket Communication**: Real-time audio streaming between frontend and backend
- **Google Gemini AI Integration**: Powered by Google's latest AI model
- **Modern React Frontend**: Clean, responsive user interface
- **Express.js Backend**: Robust server with WebSocket support

## 🏗️ Project Structure

```
revolt_task_submission/
├── backend/                 # Express.js server with WebSocket
│   ├── server.js           # Main server file
│   ├── package.json        # Backend dependencies
│   └── .env               # Environment variables
├── frontend/               # React application
│   ├── src/               # React source code
│   ├── public/            # Static assets
│   └── package.json       # Frontend dependencies
└── README.md              # This file
```

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18 or higher)
- **npm** (comes with Node.js)
- **Google Gemini API Key** (for AI functionality)

## 🛠️ Installation & Setup

### 1. Clone or Download the Project

```bash
# If you have the project files, navigate to the project directory
cd revolt_task_submission
```

### 2. Backend Setup

```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Set up environment variables
# Create or edit .env file with your Gemini API key
echo "GEMINI_API_KEY=your_gemini_api_key_here" > .env
```

**Important**: Replace `your_gemini_api_key_here` with your actual Google Gemini API key.

### 3. Frontend Setup

```bash
# Navigate to frontend directory (from project root)
cd ../frontend

# Install dependencies
npm install
```

## 🚀 Running the Application

### 1. Start the Backend Server

```bash
# From the backend directory
cd backend
npm start
```

The backend server will start on `http://localhost:3001` (or the port specified in your environment).

### 2. Start the Frontend Application

```bash
# From the frontend directory (in a new terminal)
cd frontend
npm start
```

The React application will start on `http://localhost:3000` and automatically open in your browser.

## 🔧 Configuration

### Environment Variables

Create a `.env` file in the `backend` directory with the following variables:

```env
GEMINI_API_KEY=your_actual_gemini_api_key_here
```

### API Key Setup

1. Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Copy the API key and paste it in the `.env` file

## 🎯 Usage

1. **Open the Application**: Navigate to `http://localhost:3000` in your browser
2. **Start Voice Interaction**: Click the microphone button to begin speaking
3. **Ask Questions**: Ask about Revolt Motors products, such as:
   - "What are the features of the RV400?"
   - "How much does the RV1 cost?"
   - "Where can I find a dealership?"
   - "How do I book a test ride?"

## 🔍 Troubleshooting

### Common Issues

1. **Backend Connection Error**
   - Ensure the backend server is running on port 3001
   - Check that the `.env` file contains a valid API key

2. **Audio Not Working**
   - Ensure your browser has microphone permissions
   - Check that your microphone is properly connected and working

3. **API Key Issues**
   - Verify your Gemini API key is valid and has sufficient quota
   - Check the backend console for API-related errors

### Port Conflicts

If you encounter port conflicts:

- **Backend**: The server runs on port 3001 by default
- **Frontend**: React runs on port 3000 by default

You can change these by modifying the respective configuration files.

## 📚 Dependencies

### Backend Dependencies
- `express`: Web framework
- `ws`: WebSocket library
- `@google/genai`: Google Gemini AI SDK
- `cors`: Cross-origin resource sharing
- `dotenv`: Environment variable management
- `wavefile`: Audio file processing

### Frontend Dependencies
- `react`: UI library
- `react-dom`: React DOM rendering
- `react-scripts`: Create React App scripts
- `wavefile`: Audio file processing

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the ISC License.

## 🆘 Support

For issues or questions:
1. Check the troubleshooting section above
2. Review the console logs for error messages
3. Ensure all dependencies are properly installed
4. Verify your API key is valid and has sufficient quota

---

**Note**: This application is specifically designed for Revolt Motors queries. The AI assistant will redirect users to relevant Revolt Motors topics if they ask about unrelated subjects.
