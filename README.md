# Dhanno: Ride-Booking App (Customer + Rider End-to-End)

Dhanno is a fully functional ride-booking app, designed as a clone of the popular Ola app. Built using the latest technologies such as Expo New Arch, Zustand Toolkit, Node.js, MongoDB, and WebSocket, Dhanno provides a seamless experience for both customers and riders. The app allows users to book rides, track their drivers in real-time, and ensures smooth, real-time communication for efficient ride-booking management.

## Features

- **End-to-End Ride-Booking**: A complete ride-booking experience for both customers and riders, from booking a ride to tracking the location of the driver.
- **Real-Time Location Tracking**: Real-time location updates for both customers and riders using WebSocket and Socket.IO integration.
- **Smooth Cross-Platform Support**: Built with Expo New Arch for consistent performance across both Android and iOS platforms.
- **Efficient State Management**: Zustand Toolkit for managing app state effectively and efficiently.
- **Real-Time Communication**: WebSocket integration ensures fast and seamless communication between riders and customers.
- **Backend Integration**: The app is powered by Node.js and MongoDB, providing robust and dynamic features for both the frontend and backend.
- **Real-Time Location Tracking**: Track the location of both the rider and the customer in real-time.
- **WebSocket & Socket.IO**: Utilizes WebSocket and Socket.IO for efficient and low-latency communication.
- **Google Maps Integration**: Displays real-time location on Google Maps.
- **Single Server**: Both customer and rider are managed on the same server.

## Tech Stack

### Frontend (React Native)

- **Expo New Arch**: Utilized for seamless cross-platform development and smooth user experience.
- **Zustand Toolkit**: For efficient state management and app flow control.
- **React Navigation**: Used for navigation and routing within the app.
- **Nativewind**: Utility-first CSS framework for styling the app with ease.
- **Socket.IO**: Real-time communication between customer and rider through WebSocket.
- **TypeScript**: Type-safety for maintaining code quality and reducing bugs.

### Backend

- **Node.js**: Backend server built with Node.js to handle requests and manage real-time connections.
- **MongoDB**: Database to store user profiles, ride data, and more.
- **Socket.IO**: WebSocket-based library to enable real-time communication between customers and riders.
- **Google Maps API**: For location tracking and map display features.

---

## Backend Setup

### Requirements

- **Node.js**: Ensure you have Node.js installed on your machine.
- **Google Maps API Key**: You’ll need a Google Maps API key for location tracking.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/AbhijeetParashar/dhanno-ride.git

   ```

2. Navigate to the project directory::

   ```bash
   cd server

   ```

3. Install the dependencies:

   ```bash
   npm install

   ```

4. Rename env.template to .env and update MONGO_URI

5. Start the Server

   ```bash
   npm start
   ```

## Frontend Setup

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/AbhijeetParashar/ride-app.git

   ```

2. Navigate to the project directory::

   ```bash
   cd ride-app

   ```

3. Install the dependencies:

   ```bash
   npm install

   ```

4. Open the Universal Search in VS Code and replace all instances of `YOUR_GOOGLE_MAP_API_KEY` with your actual API key.

5. Next, go to the `app.json` file and change the `bundleIdentifier` from `com.abhijeet.rideapp` to your preferred identifier.

6. Install Expo EAS CLI and log in to your Expo account:

```bash
  npm install -g eas-cli

```

7. Login to your EAS accound

```bash
eas login

```

8. Run the following command to prebuild the project:

```bash
npx expo prebuild --clean

```

8. If using a real device, update the API URLs in the client configuration:

- Open `src/service/config.js` and modify the `BASE_URL` and `SOCKET_URL` to use your local network IP or hosted URL.

9. Start the Server

```bash
npm start
```
