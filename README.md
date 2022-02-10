#  Polar Trail
This is an experiment with curves and polar coordinates, I tried to create an interesting animation by animating the U, V or Radius compounents of the Polar Coordinates

<img alt = "gif" src="Images/2021_10_16_polar_trail_1.gif">
<img alt = "gif" src="Images/2021_10_16_polar_trail_2.gif">
<img src="Images/2021_10_16_polar_trail.png">

The curves were created in a for() loop inside Point VOP, in every loop each point would sample a Curl noise, add it to its current position and add a new point in said position.

<img src="Images/Curl_Noise_Trail.png">

Afterward I would normalize the Position attribute, convert it to polar cordiantes, add the world and polar position togerher, while animating the world position. 

<img src="Images/Polar_Deform.png">

Full Node Tree:

<img src="Images/Node Tree.png">

