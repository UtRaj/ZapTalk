# 🌐 ZapTalk - Real-Time Chat App 🚀

A lightning-fast, real-time chat application built with the MERN stack, Socket.io, Redux Toolkit, and Tailwind CSS. Connect, chat, and share moments with friends and groups instantly!


## 🛠️ Tech Stack

1. **MongoDB** – Database for storing users & messages

2. **Express.js** – Backend framework for API handling

3. **React.js** – Frontend UI framework

4. **Node.js** – Server-side JavaScript runtime

5. **Socket.io** – Real-time communication

6. **Redux Toolkit** – State management

7. **Tailwind CSS** – Modern UI styling


## 🚀 Features

✅ Real-time Messaging – Instant text updates with Socket.io

✅ User Authentication – Secure sign-up/login with JWT & Google Auth

✅ Group Chat – Create rooms & invite others

✅ Message Notifications – Never miss a message!

✅ Emojis Support – Express yourself with emojis 🎉

✅ Profile Customization – Update your avatar & display name

✅ Responsive Design – Optimized for all devices 📱💻

✅ Search Functionality – Find chats & users instantly


## 📦 Installation & Setup

1️⃣ Clone the Repository

```
git clone https://github.com/UtRaj/ZapTalk.git
cd ZapTalk

```

2️⃣ Setup the Client (Frontend)


```

cd client
npm install

```


### Create a .env file in client/ and add:

```

REACT_APP_GOOGLE_CLIENT_ID=your-google-client-id
REACT_APP_SERVER_URL=http://localhost:8000

```


```
npm start

```


3️⃣ Setup the Server (Backend)

```

cd server
npm install

```


### Create a .env file in server/ and add:

```

PORT=8000
MONGO_URI=your-mongodb-uri
SECRET=your-jwt-secret
CLIENT_ID=your-google-client-id
BASE_URL=http://localhost:3000

```

```

npm start

```


🚀 Your chat app is now running on:

🔹 Frontend: http://localhost:3000

🔹 Backend: http://localhost:8000





To get your Google ClientID for authentication, go to the [credential Page ](https://console.cloud.google.com/apis/credentials) (if you are new, then [create a new project first](https://console.cloud.google.com/projectcreate) and follow the following steps;

- Click Create credentials > OAuth client ID.
- Select the Web application type.
- Name your OAuth client and click Create
- Remember to provide your domain and redirect URL so that Google identifies the origin domain to which it can display the consent screen. In development, that is going to be `http://localhost:3000` and `http://localhost:3000/login`
- Copy the Client ID and assign it to the variable `REACT_APP_GOOGLE_CLIENT_ID` in your .env file



# 🔑 Setting Up Google Authentication (Client ID)

To enable Google Sign-In for your real-time chat application, follow these steps:

## Create a Google OAuth Client ID

1. Go to Google Cloud Console

2. Click "Create Project" (if you don’t have one)

3. Navigate to APIs & Services → Credentials

4. Click "Create Credentials" → "OAuth Client ID"

5. Select "Web Application" as the application type

Set the Authorized Redirect URIs as:

```

http://localhost:3000
http://localhost:3000/login

```

6. Click Create, then copy your Client ID to Inside Client Directory at (client/.env) and Inside Server Directory at (server/.env) .


🚀 Now your Google Authentication is ready! 🎉