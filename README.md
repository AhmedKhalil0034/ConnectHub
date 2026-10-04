# 🌐 ConnectHub

ConnectHub is a comprehensive social networking platform that empowers users to build relationships, share content, and engage interactively with ease and scalability.

---

## 📌 Table of Contents

- [Key Features](#-key-features)
- [Core Entities and Relationships](#-core-entities-and-relationships)
- [Security Features](#-security-features)
- [Privacy & Scalability](#-privacy--scalability)
- [Project Structure](#-project-structure)

---

## ✨ Key Features

- **User Profiles**: Personalize with bios, profile pictures, and cover photos.
- **Posts**: Share text, images, and videos with privacy controls.
- **Interaction**: Likes, comments, and reactions.
- **Messaging**: Private and group chats.
- **Groups**: Join communities with customizable privacy settings.
- **Friendships**: Send and manage friend requests.
- **Notifications**: Stay updated on platform activities.
- **Verification**: Secure identity verification process.

---

## 🧩 Core Entities and Relationships

### 1. User

- Name, email, date of birth.
- Passwords are securely stored using hashing.
- Creation and update timestamps.
- Activity status.

### 2. Profile

- Bio, profile picture, cover photo.
- Profile and cover images are validated to prevent malicious uploads.
- Linked to one user.

### 3. Post

- Text content, attached media.
- Privacy settings.
- Linked to a user or group.

### 4. Comment

- Text content.
- Belongs to a post and authored by a user.

### 5. Like

- Reaction type (like, love, etc.).
- Linked to a post or comment.

### 6. Friend

- Relationship status (pending, accepted, etc.).
- Connects two users.

### 7. Message & Chat

- Message text and timestamps.
- Chats involve two or more users.

### 8. Group

- Name and description.
- Privacy settings.
- Linked to posts and users.

### 9. Notification

- Content and read status.
- Sent to one user.

### 10. Friend Request

- Status (pending, accepted, rejected).

### 11. Verification

- Request status and date.

---

## 🔒 Security Features

- **Password Hashing**: All user passwords are hashed for secure storage.
- **Image Validation**: Profile and cover images are validated to ensure safe uploads and prevent malicious content.

---

## 📈 Privacy & Scalability

- Efficient identifiers ensure seamless scaling.
- Robust privacy controls for posts, groups, and accounts.

---

## 📂 Project Structure

```text
├── src/main/            # Application source code
├── javafx-sdk-23.0.1/   # JavaFX SDK
├── .mvn/wrapper/        # Maven wrapper configuration
├── mvnw, mvnw.cmd       # Maven wrapper scripts
├── pom.xml              # Maven project configuration
├── users.txt            # Stored users
├── posts.txt            # Stored posts
├── comments.txt         # Stored comments
├── chats.txt            # Stored chats
├── notifications.txt    # Stored notifications
├── friends_graph.txt    # Stored friendships
└── README.md
```
