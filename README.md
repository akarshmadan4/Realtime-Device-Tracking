# Realtime-Device-Tracking

## Overview
This project is a real-time device tracking system that leverages WebSockets to monitor and display the location of devices on a map. It is designed to provide an efficient and responsive way to track multiple devices simultaneously, with updates appearing on the map in real-time.

## Features
- Real-Time Tracking: Uses WebSockets to provide real-time updates of device locations.
- Map Integration: Displays device locations on a map interface.
- Automatic marker updates as device locations change

## Technologies Used
- Node.js
- Express.js
- Socket.io
- Leaflet.js

## Backend

**Server Initialization**: The server is initialized using Express.js and sets up an HTTP server.


**Socket.io Integration**: Socket.io is integrated to handle real-time communication. When a client connects, a unique socket ID is generated.


**Geolocation Data Handling**: The server listens for geolocation data sent from clients. When data is received, it broadcasts the location update to all connected clients.


## Frontend

**Geolocation Retrieval**: The browser's Geolocation API is used to continuously monitor the device's position.


**Map Rendering**: Leaflet.js is used to create an interactive map. Markers are added to the map to represent the location of each connected device.


**Real-time Updates**: As location updates are received from the server, the positions of the markers on the map are updated in real-time.


**Marker Management**: The client-side code handles the creation, updating, and removal of markers based on the data received from the server.
