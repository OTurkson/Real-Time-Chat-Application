# Real-Time Chat Application

A real-time chat application built with Spring Boot and WebSocket technology.

## 🚀 Features

- Real-time messaging using WebSocket
- Simple and clean user interface
- Multiple users can chat simultaneously
- Built with Spring Boot for robust backend
- Responsive web design

## 🛠️ Technologies Used

- **Backend**: Spring Boot 3.5.3
- **WebSocket**: Spring WebSocket for real-time communication
- **Frontend**: HTML, CSS, JavaScript
- **Template Engine**: Thymeleaf
- **Build Tool**: Maven
- **Java Version**: Compatible with Java 17+

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- Java 17 or higher
- Maven 3.6+
- Git

## 🏃‍♂️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/OTurkson/Real-Time-Chat-Application.git
cd Real-Time-Chat-Application
```

### 2. Build the application

```bash
./mvnw clean install
```

Or on Windows:

```cmd
mvnw.cmd clean install
```

### 3. Run the application

```bash
./mvnw spring-boot:run
```

Or on Windows:

```cmd
mvnw.cmd spring-boot:run
```

### 4. Access the application

Open your web browser and navigate to:

```
http://localhost:8080/chat
```

## 🏗️ Project Structure

```
src/
├── main/
│   ├── java/
│   │   └── com/chat/app/
│   │       ├── AppApplication.java          # Main Spring Boot application
│   │       ├── config/
│   │       │   └── WebSocketConfig.java     # WebSocket configuration
│   │       ├── controller/
│   │       │   └── ChatController.java      # Chat message controller
│   │       └── model/
│   │           └── ChatMessage.java         # Chat message model
│   └── resources/
│       ├── static/                          # Static web resources
│       ├── templates/
│       │   └── chat.html                    # Chat interface template
│       └── application.properties           # Application configuration
```

## 🔧 Configuration

The application uses default Spring Boot configurations. The main configuration file is located at `src/main/resources/application.properties` and currently contains minimal settings for the chat application to run.

## 🚀 How It Works

1. **WebSocket Connection**: The application establishes a WebSocket connection when users access the chat page
2. **Message Broadcasting**: When a user sends a message, it's broadcasted to all connected clients via the `/topic/messages` topic
3. **Real-time Updates**: All connected users receive messages instantly without page refresh

## 🔒 Security Considerations

- This is a basic implementation intended for demonstration purposes
- For production use, consider implementing:
  - User authentication and authorization
  - Message validation and sanitization
  - Rate limiting
  - HTTPS/WSS encryption
  - Proper configuration management

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**OTurkson**

- GitHub: [@OTurkson](https://github.com/OTurkson)

## 🐛 Known Issues

- No message persistence (messages are lost on server restart)
- No user identification system
- Limited to single chat room

## 🔮 Future Enhancements

- [ ] User authentication system
- [ ] Multiple chat rooms
- [ ] Message history persistence
- [ ] File sharing capabilities
- [ ] Emoji support
- [ ] Private messaging
- [ ] User online status indicators

## 📞 Support

If you encounter any issues or have questions, please:

1. Check the [Issues](https://github.com/OTurkson/Real-Time-Chat-Application/issues) section
2. Create a new issue if your problem isn't already reported
3. Provide detailed information about your environment and the issue

---

**Happy Chatting! 💬**
