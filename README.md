# 💬 ModernChat - Real-time Chat Application

A modern, feature-rich real-time chat application built with Node.js, Socket.io, and Tailwind CSS.

## ✨ Features

- 🔥 **Real-time messaging** with Socket.io
- 😊 **Emoji picker** with categories
- 📎 **File sharing** (images, documents, etc.)
- 🎨 **Modern UI** with Tailwind CSS
- 📱 **Responsive design** for mobile and desktop
- 🔊 **Audio notifications** (toggle-able)
- 👥 **User management** with join/leave notifications
- ⚡ **Fast and lightweight**

## 🚀 Quick Start

### Local Development

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd chat-app-modified
   ```

2. **Install dependencies**
   ```bash
   cd nodeServer
   npm install
   ```

3. **Start the server**
   ```bash
   npm start
   ```

4. **Open the application**
   - Open `index.html` in a browser or
   - Use Live Server extension in VS Code
   - Access: `http://localhost:5500`

## 🌐 Deployment

### Option 1: Render + Netlify (Recommended - FREE)

#### Backend (Render):
1. Push your code to GitHub
2. Go to [render.com](https://render.com) and create an account
3. Create a new "Web Service"
4. Connect your GitHub repository
5. Configure:
   - **Build Command**: `cd nodeServer && npm install`
   - **Start Command**: `cd nodeServer && npm start`
   - **Environment**: Node
6. Deploy and copy the generated URL

#### Frontend (Netlify):
1. Update the backend URL in `js/client.js`:
   ```javascript
   const BACKEND_URL = 'https://your-app-name.onrender.com';
   ```
2. Go to [netlify.com](https://netlify.com)
3. Drag and drop your project folder (excluding nodeServer)
4. Your chat app is live! 🎉

### Option 2: Railway (Easy)
```bash
npm install -g @railway/cli
railway login
railway init
railway up
```

### Option 3: DigitalOcean, AWS, Google Cloud
See `HOSTING_GUIDE.md` for detailed instructions.

## 📁 Project Structure

```
chat-app-modified/
├── index.html              # Main HTML file
├── css/
│   └── style.css          # Custom styles (legacy)
├── js/
│   └── client.js          # Frontend JavaScript
├── images/                # Static assets
├── nodeServer/
│   ├── index.js          # Express server
│   ├── package.json      # Dependencies
│   └── .env.example      # Environment variables
├── HOSTING_GUIDE.md      # Detailed hosting instructions
└── FEATURES_TESTING.md   # Feature testing guide
```

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the `nodeServer` directory:
```env
PORT=8080
NODE_ENV=production
CORS_ORIGIN=https://your-frontend-domain.com
```

### Custom Domain
1. Purchase a domain
2. Configure DNS settings
3. Update CORS_ORIGIN in your environment variables

## 🧪 Testing

1. **Start the server**: `npm start` in `nodeServer/`
2. **Open multiple browser tabs** to test real-time chat
3. **Test features**:
   - Send messages
   - Share files/images
   - Use emoji picker
   - Toggle audio notifications

## 🛡️ Security Features

- CORS protection
- Input validation
- File type restrictions
- XSS protection

## 🎨 Customization

- **Colors**: Modify Tailwind classes in HTML/JS
- **Emojis**: Update emoji categories in `client.js`
- **File types**: Modify file validation in upload functions
- **Styling**: Add custom CSS or modify Tailwind config

## 📱 Browser Support

- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

MIT License - feel free to use for personal or commercial projects.

## 🆘 Support

Having issues? Check:
1. `FEATURES_TESTING.md` for testing guidelines
2. `HOSTING_GUIDE.md` for deployment help
3. Browser console for error messages
4. Ensure server is running before opening frontend

## 🎯 Live Demo

- **Frontend**: https://your-app.netlify.app
- **Backend**: https://your-app.onrender.com

---

**Built with ❤️ using Node.js, Socket.io, and Tailwind CSS**
