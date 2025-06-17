
# 💬 Flutter Chat App (GetX + WebSocket)

A simple real-time chat app built with Flutter using **GetX** for state management and **WebSocket** for live messaging.

---

## 🚀 Features

- Chat user list display
- Real-time messaging via WebSocket
- Clean navigation with `Get.to()`
- Reactive UI with GetX

---

## 🧠 Key Components

- `UsersChatList`: Shows available users
- `ChatScreen`: One-to-one chat UI
- `ChatController`: Handles chat logic & socket connection

---

## 🔗 WebSocket

```dart
static const String websocketUrl = "";
````

---

## ⚙️ Initialization

```dart
final ChatController chatController = Get.put(ChatController());
chatController.fetchUserList();
```

To open chat:

```dart
Get.to(() => ChatScreen(
  name: receverFullName,
  receiverId: receverId,
  imageUrl: profileImage,
));
```

---

## 📦 Dependencies

```yaml
get: ^4.6.5
web_socket_channel: ^2.3.0
```



## 📄 License

MIT License


