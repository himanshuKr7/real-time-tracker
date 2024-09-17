
# Real-Time Tracker Backend

This is a real-time geolocation tracking application built using **Node.js**, **Express.js**, **Socket.IO**, and **Leaflet** (open-source geolocation map). The application allows users to track multiple clients' locations on a map in real-time.

## Features

- **Real-time Geolocation Tracking**: Tracks the location of multiple users and displays their positions on a map.
- **Socket.IO Integration**: Enables real-time communication between the server and connected clients.
- **Leaflet Map**: Renders the user’s locations on an interactive map.
- **Dynamic Markers**: Each connected user is represented by a dynamic marker on the map.
- **User Disconnect**: When a user disconnects, their marker is automatically removed from the map.

## Technologies Used

- **Node.js**: Backend server runtime environment.
- **Express.js**: Server-side framework for handling routes and serving static files.
- **Socket.IO**: For real-time, bidirectional communication between the server and clients.
- **Leaflet**: An open-source JavaScript library for mobile-friendly interactive maps.

##Images
![location1](https://github.com/user-attachments/assets/b26bbb73-0fdd-410a-9afa-4960835d81d1)

![location2](https://github.com/user-attachments/assets/e46b6d06-5586-40f0-b6b3-a5af39838059)

## Project Structure
/public
    /css
        - style.css      # Styling for the frontend
    /js
        - script.js      # Client-side JavaScript for handling geolocation and map interactions
/views
    - index.ejs          # The main HTML template rendered by Express
app.js                   # The main server file
package.json             # Project metadata and dependencies
```

## Installation

### Prerequisites
- **Node.js** and **npm** should be installed on your machine.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/himanshuKr7/realtime-tracker.git
   cd realtime-tracker
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   node app.js
   ```
   Or use **nodemon** for automatic server restarts during development:
   ```bash
   npx nodemon app.js
   ```

4. Open the app in your browser:
   ```
   http://localhost:3000
   ```

## Geolocation Error Handling

- **Permission Denied (Error Code 1)**: User has denied access to geolocation services.
- **Position Unavailable (Error Code 2)**: The device or network couldn't determine the user’s location.
- **Timeout (Error Code 3)**: The request to retrieve the geolocation data took too long.

Made with &#10084; By Himanshu :)
