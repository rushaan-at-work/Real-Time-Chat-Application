project:
  name: Real-Time Chat Application
  description: >
    A real-time group chat application built using Spring Boot, WebSocket, STOMP, and SockJS.
    It allows multiple users to communicate instantly through a responsive web interface.

technologies:
  backend:
    - Java 17+
    - Spring Boot
    - WebSocket
    - STOMP
    - SockJS
  frontend:
    - HTML5
    - Bootstrap 5
    - JavaScript (STOMP.js, SockJS Client)

features:
  - Real-time two-way messaging
  - Message broadcasting to all users
  - Lightweight and responsive UI
  - Works with multiple concurrent clients

backend:
  websocket_config:
    - Endpoint: "/chat"
    - Broker: "/topic"
    - Prefix: "/app"
  controller:
    - sendMessage(): Handles and broadcasts messages
    - chat(): Returns chat interface page

frontend:
  - connect(): Establishes WebSocket connection
  - sendMessage(): Sends messages to backend
  - showMessage(): Displays messages in chat window

run_instructions:
  prerequisites:
    - Java 17 or higher
    - Maven installed
  steps:
    - Clone repo:
      ```bash
      git clone https://github.com/your-username/realtime-chat-app.git
      ```
    - Run:
      ```bash
      mvn spring-boot:run
      ```
    - Access:
      ```bash
      http://localhost:8080
      ```

author:
  name: Mohd Rushaan Siddiqui
  github: https://github.com/rushaan-siddiqui
  linkedin: https://linkedin.com/in/mohd-rushaan-siddiqui

license:
  type: MIT
