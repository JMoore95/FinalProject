Final Project (CAP 4720) by Jacob Williams-Moore

Description:

This Final Project demonstrates the use of Three.js and the WebGL Renderer to imitate weather
effects in different environments. As of right now the only effects that can be shown are
rain and rain clouds. The different environments are being implemented using skyboxes.
A simple cube is made and images are mapped to each side of the cube. The user will be inside
of the cube and able to select three different skyboxes which represent different environments.

Prerequisites:

Computer and browser capable of loading WebGL renderer and Three.js.

How to run:

Open the index.html file in a browser or go to https://jmoore95.github.io/FinalProject/

Contact:

jacobmoore@knights.ucf.edu
https://github.com/JMoore95/FinalProject (follow for future updates)

Javascript Code:

init() function:

Description - This function is used to create the scene, call other init functions, and handleResize function.
Parameters - None
Returns - None


initRenderer function:

Description - Creates WebGL Renderer
Parameters - None
Returns - None


handleResize function:

Description - Adjusts the renderer and camera size to match the window size if adjusted
Parameters - None
Returns - None


initCamera function:

Description - Creates a perspective camera and pointer lock controls and adds to the scene
Parameters - None
Returns - None


onKeyDown function:

Description - Listens for and switch on keypresses from user. Calls functions for moving camera and locking the mouse pointer
Parameters - None
Returns - None


initLight function:

Description - Creates an ambient and directional light for the scene.
Parameters - None
Returns - None


initCube function:

Description - Creates skyboxes for user environments using THREE.Texture loader.
Parameters - None
Returns - None


initClouds function:

Description - Creates clouds by mapping "smoke-1.png" to plane geometry and creates 100 clouds using random coordinates
Parameters - None
Returns - None


addClouds function:

Description - Adds clouds that were created in initClouds function to the scene
Parameters - None
Returns - None


removeClouds function:

Description - Removes clouds that were created in initClouds function to the scene
Parameters - None
Returns - None


initRain function:

Description - Creates rain drops using Vector3 vertices and treats it as one object with many points
Parameters - None
Returns - None


guiControls function:

Description - Controls for dat.gui, everything is initialized to false
Parameters - None
Returns - None

render function:

Description - Animates the scene and adds velocity to rain and rotates clouds
Parameters - None
Returns - None