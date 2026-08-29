# LANShare

LANShare is a simple, serverless web application that allows you to send files directly between two browsers on the same network (Wi-Fi / LAN). It uses WebRTC data channels to establish a peer-to-peer connection, meaning your files are sent directly and are never uploaded to any server.

## Features

- **Peer-to-Peer:** Files are transferred directly between devices using WebRTC.
- **Serverless:** No backend server is required for file storage or transfer.
- **Privacy Focused:** Files are never stored anywhere else.
- **No Internet Required:** Once the initial WebRTC signaling (copy-pasting room codes) is done, the transfer happens locally over your LAN.
- **Browser Based:** Runs entirely in your web browser without the need to install any additional software.

## How to Use

1. **Open LANShare:** Open the `index.html` file in your browser.
2. **Choose a Role:**
   - **Person A (Sender):** Clicks "Create room". A room code will be generated. Send this code to Person B via any chat app or email.
   - **Person B (Receiver):** Clicks "Join a room", pastes the room code received from Person A, and clicks "Generate reply code". Person B then sends this reply code back to Person A.
   - **Person A:** Pastes the reply code from Person B and clicks "Connect".
3. **Connect & Transfer:** Once the status shows "connected — ready to send files", Person A can select a file and click "Send". The file will begin downloading on Person B's browser.

## Technologies Used

- HTML5
- Vanilla JavaScript
- WebRTC (RTCPeerConnection, RTCDataChannel)

## Setup

Simply clone the repository and open `index.html` in any modern web browser. No build steps or local servers are required!
