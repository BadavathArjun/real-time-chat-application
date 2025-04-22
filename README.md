Real-Time Chat Application - README

![image](https://github.com/user-attachments/assets/056492ca-863f-4e3a-9a19-f4c723cecc24)


## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

✨ **Modern UI/UX Design**
- Clean, professional interface with responsive layout
- Sidebar showing active users with real-time updates
- Beautiful message bubbles with timestamps
- Connection status indicators

⚡ **Real-Time Functionality**
- Instant message delivery with Socket.IO
- Typing indicators showing when others are typing
- Active user tracking and notifications
- Optimistic UI updates for smooth experience

🔒 **Reliable Infrastructure**
- Automatic reconnection logic
- Input validation and error handling
- Graceful server shutdown
- Cross-browser compatibility

## Technologies Used

**Frontend:**
- HTML5, CSS3 (with CSS Variables)
- Vanilla JavaScript (ES6+)
- Socket.IO client library
- Font Awesome for icons
- Google Fonts (Roboto)

**Backend:**
- Node.js
- Express.js
- Socket.IO server
- Built-in HTTP server

## Installation

### Prerequisites
- Node.js (v14 or higher)
- npm (comes with Node.js)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/BadavathArjun/real-time-chat-application.git
   cd real-time-chat-application
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   node server.js
   ```

4. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

## Usage

1. **Join the Chat**
   - Enter your desired username in the input field
   - Click "Join Chat" or press Enter

2. **Send Messages**
   - Type your message in the input field at the bottom
   - Press Enter or click the send button to submit

3. **Features**
   - See who's online in the sidebar
   - Get notifications when users join/leave
   - See typing indicators when others are composing messages
   - View message timestamps

## Configuration

The application can be configured by modifying the following:

1. **Port Number**  
   Change the port in `server.js`:
   ```javascript
   const PORT = process.env.PORT || 3000; // Change 3000 to your preferred port
   ```

2. **CORS Settings**  
   Adjust in `server.js` if needed:
   ```javascript
   const io = require('socket.io')(http, {
       cors: {
           origin: "*", // Change to specific domain in production
           methods: ["GET", "POST"]
       }
   });
   ```

3. **UI Colors**  
   Modify CSS variables in `styles.css`:
   ```css
   :root {
       --primary-color: #4361ee;
       --primary-dark: #3a56d4;
       /* Other color variables */
   }
   ```

## Project Structure

```
professional-chat-app/
├── public/
│   ├── index.html          # Main HTML file
│   ├── styles.css          # All CSS styles
│   └── script.js           # Client-side JavaScript
├── server.js               # Node.js server code
├── package.json            # Project dependencies
└── README.md               # This file
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

**Happy Chatting!** 🎉
