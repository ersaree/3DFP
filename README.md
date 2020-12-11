# 3DFP - A 3D Floorplan for Home Assistant

I am working on this project to implement a live interactive 3D Floorplan for Home Assistant. The 3D model is built with babylon.js and then I connect to Home Assistant through a websocket. 

Currently, I can show lights and use colors as indictors if windows are opened.There are also signs to display for instance the current temperature or other info for a room.
See a live beta demo here. https://tjntomas.github.io/3DFP/


![HADashboard-widgets](https://github.com/tjntomas/3DFP/blob/main/img/3dfp.jpg?raw=true)


Todo:
- Add more objects such as vacuum cleaners, outdoor street lights etc.
- Complete the popup control panels when you click an item in the model so you can control the colors of lights etc.
- Add functionality to display an actual open window or door.
- Light up the ceiling and walls of a room when a motion sensor is triggered, or add a stroboscobe-like effect.
- Move the yaml configuration from my previous 3DFP project so that the 3D model and the connections to Home Assistant entities can be defined in yaml

Feel free to leave a message if you are interested in helping out.


