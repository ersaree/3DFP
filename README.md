# 3DFP - A 3D Floorplan for Home Assistant

I am working on a project to implement an interactive 3D Floorplan for Home Assistant. The 3D model is built with babylon js, http://babylonjs.com and then I connect to Home Assistant through a websocket to receive events and send service calls to monitor and control entities. 

Currently, I can show lights and use colors as indictors if for instance a window is open. There are also signs to display the current temperature or other info for a room.
See a live beta demo here. https://tjntomas.github.io/3DFP/

Feel free to leave a message in issues if you are interested in helping out.


![HADashboard-widgets](https://github.com/tjntomas/3DFP/blob/main/img/3dfp.jpg?raw=true)


Todo
- Add more objects such as a television, vacuum cleaner, outdoor street light etc.
- Complete the popup control panels when you click an item in the model so you can control the colors of lights etc.
- Add functionality to display an actual open window or door.
- Light up the ceiling and walls of a room when a motion sensor is triggered, or add a stroboscobe-like effect.
- Move the yaml configuration from my previous 3DFP project so that the 3D model and the connections to Home Assistant entities can be defined in yaml



Log
- It appears that the 3D engine babylon.js, http://babylonjs.com has some limitations when it comes to rendering a large number of lights and shadows. To overcome this, the 3D model  need to be separated into elements such as walls, ceilings and floors for each room and making sure that any light only reflects on objects in one room.

- The 3D engine is using up a lot of GPU (when available) in Chrome and Edge browsers, so I have implemented rendering on-demand to limit the GPU load. This is a not a problem in Safari, Firefox or the android Chrome browser.
