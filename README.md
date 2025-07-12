# Gemini Clone

A modern, responsive web application that replicates the Google Gemini AI interface using React and the Google Generative AI API. This project provides a clean, intuitive chat interface for interacting with AI-powered conversations.

## 🚀 Features

- **AI Chat Interface**: Seamless conversation with Google's Gemini 2.0 Flash model
- **Responsive Design**: Modern UI that works on desktop and mobile devices
- **Chat History**: Save and access previous conversations
- **Real-time Typing Effect**: Dynamic text animation for AI responses
- **Quick Prompts**: Pre-built suggestion cards for common use cases
- **Collapsible Sidebar**: Clean navigation with expandable menu
- **New Chat Functionality**: Start fresh conversations anytime
- **Safety Settings**: Built-in content filtering and safety measures

## 🛠️ Tech Stack

- **Frontend**: React 19.1.0
- **Build Tool**: Vite 6.3.5
- **Styling**: CSS3 with modern design patterns
- **AI Integration**: Google Generative AI (@google/generative-ai)
- **State Management**: React Context API
- **Development**: ESLint for code quality

## 📋 Prerequisites

Before running this project, make sure you have:

- Node.js (version 16 or higher)
- npm or yarn package manager
- Google AI Studio API key

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd gemini-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up your API key**
   
   **Option 1: Direct replacement (for development)**
   - Open `src/config/gemini.js`
   - Replace the `API_KEY` value with your Google AI Studio API key
   
   **Option 2: Environment variable (recommended for production)**
   - Create a `.env` file in the root directory
   - Add: `VITE_GEMINI_API_KEY=your_api_key_here`
   - Update `src/config/gemini.js` to use: `process.env.VITE_GEMINI_API_KEY`

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5173` to see the application

## 🎯 Usage

### Getting Started
1. The app opens with a welcome screen and suggestion cards
2. Click on any suggestion card to start a conversation
3. Or type your own prompt in the input field at the bottom

### Features
- **New Chat**: Click the "+" button in the sidebar to start a fresh conversation
- **Chat History**: Expand the sidebar to see and access previous conversations
- **Voice Input**: Use the microphone icon for voice input (UI ready)
- **Image Upload**: Use the gallery icon to upload images (UI ready)

### Quick Prompts
The app includes several pre-built suggestion cards:
- Travel recommendations
- Concept summaries
- Team bonding ideas
- Code improvement suggestions

## 📁 Project Structure

```
gemini-clone/
├── src/
│   ├── components/
│   │   ├── Main/
│   │   │   ├── Main.jsx          # Main chat interface
│   │   │   └── Main.css          # Main component styles
│   │   └── Sidebar/
│   │       ├── Sidebar.jsx       # Navigation sidebar
│   │       └── Sidebar.css       # Sidebar styles
│   ├── Context/
│   │   └── Context.jsx           # React Context for state management
│   ├── config/
│   │   └── gemini.js             # Google AI API configuration
│   ├── assets/
│   │   └── assets.js             # Static assets and icons
│   ├── App.jsx                   # Main app component
│   ├── main.jsx                  # App entry point
│   └── index.css                 # Global styles
├── public/                       # Static assets
├── package.json                  # Dependencies and scripts
└── vite.config.js               # Vite configuration
```

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint for code quality

## 🔒 Security Notes

- **API Key Security**: Never commit your API key to version control
- **Environment Variables**: Use `.env` files for sensitive data in production
- **Rate Limiting**: Be aware of Google AI API rate limits
- **Content Filtering**: The app includes safety settings to filter harmful content

## 🎨 Customization

### Styling
- Modify CSS files in respective component directories
- Global styles can be updated in `src/index.css`
- The app uses a modern, clean design that's easy to customize

### Features
- Add new suggestion cards in `Main.jsx`
- Modify AI response formatting in `Context.jsx`
- Update safety settings in `gemini.js`

## 🚀 Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add your API key as an environment variable
4. Deploy

### Netlify
1. Build the project: `npm run build`
2. Upload the `dist` folder to Netlify
3. Add environment variables in Netlify dashboard

### Other Platforms
The app can be deployed to any static hosting service that supports React applications.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Google AI Studio for providing the Gemini API
- React team for the amazing framework
- Vite for the fast build tool
- The open-source community for inspiration and tools

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Issues](https://github.com/your-repo/issues) page
2. Create a new issue with detailed information
3. Include your Node.js version and any error messages

---

**Note**: This is a clone/educational project. For production use of Google's AI services, please refer to Google's official documentation and terms of service.
