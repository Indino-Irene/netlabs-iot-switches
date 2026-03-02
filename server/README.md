This folder contains the work covering the development and deployement of the server
We are going to use socket programing to come up with a server and a client. Socket programming is essentally the "digital plumbing" that allows your software to send commands across a network.For the case of the building of an ac dimmer, It talks to the hardware that that physically dims the light.
So, we are going to have two parts, the client(controller) and a server(the light fixer). 
Socket programming is going to enable, in real-time communication, command transmission and remote access

How we are going to use socket programming.
So we are going to follow a Client-Server model using Python's built-in socket library
1.The server(The Light controller) The light buld needs a "listener". This script runs on the device connected to the light
What it does: It waits for a connection, receives a number(0-100),and translates that number into hardware signal like PWM(Pulse width Modulation) to change the voltage going to the light

2. The Client.(The Remote Control)- This script runs on the user's computer or a mobile app.
3. The purpose. Is to connect to the server's IP address and sends the desired brightness value based on user input
