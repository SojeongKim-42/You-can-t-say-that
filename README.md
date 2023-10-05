# on-game
![image](https://user-images.githubusercontent.com/78066907/210474057-26efcae3-bfd9-48d8-b41f-a1417e74c502.png)
https://youtu.be/oAY5j6EmNZk
> game rule
  1. Maximum player in this game is 3.
  2. After turning on your video, you can create a room or join a room by ID.
  3. Only user1 can start the game by play button, User2 and 3 must click the play button after User1.
  4. In the game, everyone is given a random forbidden word.
  5. Takes turns to talk about the selected topic (GIST), you have to click mic button in your turn.
  6. When you say your forbidden word, you fail, and your video & audio is turned off!
 

# Setting the Environment 
Firebase + WebRTC Codelab : See http://webrtc.org for details.

Before starting this codelab, make sure that you've installed:  
npm which typically comes with Node.js - Node LTS is recommended.  
see https://nodejs.org/ for details.

# command on cmd
Run the following Firebase CLI command:
```
  firebase serve --only hosting
```
Your command line should display the following response:
```
  hosting: Local server: http://localhost:5000
```
We're using the Firebase Hosting emulator to serve our app locally. The web app should now be available from http://localhost:5000.  

Open your app at http://localhost:5000.

# troubleshooting
js update : 
https://stackoverflow.com/questions/3951187/javascript-file-not-updating-no-matter-what-i-do



> Operation principle
  
  This project is based on P2P principle, and the firebase is used as signaling server. After asking STUN server of own public address, ICE brings all communicable addresses(local address, server reflexive address, TURN relay address …). SDP is Session Description Protocol which is used to set the initial information of media. It has offer/answer model, so if caller offers information of caller’s exchanging mediaStream callee can answer by callee’s mediaStream information. After the answer of callee, best ICE candidate that is the fastest and most reliable is selected. After all, peers can exchange the media directly. 
