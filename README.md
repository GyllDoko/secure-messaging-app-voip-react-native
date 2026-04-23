# Realtime Messaging & VoIP App (React Native)

A fullstack mobile messaging platform with real-time chat, voice/video calling, and push notifications, built with React Native and a scalable backend architecture.

---

## 🧩 Problem

Modern communication apps require real-time messaging, reliable call handling, and seamless user experience across devices, while managing complex systems like push notifications and WebRTC.

---

## 💡 Solution

Built a mobile communication platform combining real-time messaging and VoIP capabilities, with backend-driven authentication, event handling, and scalable infrastructure.

---

## ⚙️ Tech Stack

- React Native (Expo + native modules)
- Supabase (auth, database, storage)
- Stream Chat (real-time messaging)
- Stream Video (VoIP / calls)
- Firebase Cloud Messaging (push notifications)
- WebRTC (call handling)

---

## 🚀 Key Features

- Real-time chat with channel-based messaging
- 1:1 conversations and user directory
- Voice/video calling (VoIP integration)
- Push notifications for messages and calls
- Profile management with avatar upload
- Authentication (email/password)

---

## 🧠 Architecture

- Supabase handles authentication, profiles, and storage
- Stream Chat manages messaging infrastructure
- Stream Video handles call sessions and signaling
- Firebase Cloud Messaging delivers push notifications
- Edge functions generate secure tokens for Stream services

---

## ⚠️ Challenges & Solutions

**Real-time communication**

- Integrated Stream Chat with token-based authentication via backend

**VoIP call handling**

- Implemented call lifecycle management with Stream Video + WebRTC

**Push notifications**

- Connected Firebase Cloud Messaging with Stream services for message and call alerts

**Native module integration**

- Used custom dev client due to dependencies like CallKeep and Notifee

---

## 🔄 Communication Flow

User → Auth (Supabase) → Request Token → Connect to Stream → Send Message / Start Call → Push Notification → Other User Receives Event

---

## 📸 Screenshots

(Add screenshots here if you want — optional)

---

## ▶️ Running Locally

```bash
npm install
npm start
npm run android
npm run ios
```

### Environment variables

```bash
EXPO_PUBLIC_SUPABASE_URL=
EXPO_PUBLIC_SUPABASE_ANON_KEY=
EXPO_PUBLIC_STREAM_API_KEY=
```

## Notes

> - Requires native build (not Expo Go)
> - Push notifications and VoIP require proper credentials and configuration
> - Designed to simulate production-level messaging and communication systems
