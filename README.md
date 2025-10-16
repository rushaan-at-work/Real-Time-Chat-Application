# 🗨️ Real-Time Chat Application

A simple **real-time group chat** built using **Spring Boot**, **WebSocket**, **STOMP**, and **SockJS**.  
It allows multiple users to send and receive messages instantly through a web interface.

---

## 🚀 Features
- Real-time two-way messaging  
- Broadcasts messages to all connected users  
- Responsive and lightweight Bootstrap UI  
- Supports multiple concurrent users  

---

## 🛠️ Tech Stack
**Backend:**  
- Java 17+  
- Spring Boot  
- WebSocket + STOMP  
- SockJS  

**Frontend:**  
- HTML5, CSS3  
- Bootstrap 5  
- JavaScript (STOMP.js, SockJS Client)

---

## ⚙️ WebSocket Configuration
- **Endpoint:** `/chat`  
- **Message Broker:** `/topic`  
- **Application Prefix:** `/app`  

**Key Methods:**
- `sendMessage()`: Handles and broadcasts chat messages  
- `chat()`: Loads the chat page  

---

## ▶️ Run Locally

### Prerequisites
- Java 17 or higher  
- Maven installed  

### Steps
```bash
git clone https://github.com/your-username/realtime-chat-app.git
cd realtime-chat-app
mvn spring-boot:run
