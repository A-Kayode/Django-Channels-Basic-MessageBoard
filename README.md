## **DJANGOO-CHANNELS BASIC MESSAGE BOARD**

A simple and basic non-persistent message board platform designed to demonstrate real-time communications using websocket technology. Built using Django Framework and the Django-Channels library. Also makes use of Redis to facilitate asynchronous websocket connections via Channels.

## **INSTALLATION**
This project can only be found at this repository at the moment. It was created with Python 3.9 recommended for up to Python 3.12.
  1. Clone this repository into your directory of choice.
  2. Ensure your python version is withing the recommended python version range.
  3. At the chosen directory, install the project requirements via the command: =pip install -r requirements.txt=
  4. In the 'settings.py' module, nagivate to the 'CHANNEL_LAYERS' configuration setting and replace the string 'redis_connection_string_here' with a connection string to any redis cache service of your choice.

## **USAGE**
### Local Usage
1. At the directory with the 'manage.py' file, start the server using the =python manage.py runserver= command.
2. Once started, navigate to =127.0.0.1:8000/chat/= where you will be prompted to input a room name. Do that and you will be redirected to the 'chat-room' page with two seperate areas. The first section displays in real time, messages posted in that room, while the other is an input field where you can send messages to the chatroom. 
3. Repeat step two on a seperate or anonymous browser to simulate the connection of another client to the chatroom.
4. Messages sent to the chatroom from any browser/client will now be displayed in real time for everyone in the room.
