<p align="center">
   <a href="https://github.com/nitzan-treg/community_projects/">
    <img alt="Website" src="https://img.shields.io/website?label=main%20project&up_message=Community%20Projects&url=https%3A%2F%2Fgithub.com%2Fnitzan-treg%2Fcommunity_projects">
  </a>
  <a href="https://github.com/nitzan-treg/community_projects/">
    <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/nitzan-treg/Polar_Trail">
  </a>
  <a href="https://www.nitzan-tregerman.com/">
    <img alt="Website" src="https://img.shields.io/website?up_message=nitzan-tregerman.com&url=https%3A%2F%2Fwww.nitzan-tregerman.com%2F">
  </a>
  <img alt="GitHub" src="https://img.shields.io/github/license/nitzan-treg/Polar_Trail">
</p>

#  Polar Trail

I made a tutorial that teaches how to create this system and how it works, you are welcome to check it on this [link](https://youtu.be/9MPGec7JNyA)

this project is a part of a series of free projects im releasing for free for everyone
This is an experiment with curves and polar coordinates, I tried to create an interesting animation by animating the U, V, or Radius components of the Polar Coordinates

<img alt = "gif" src="Images/2021_10_16_polar_trail_1.gif">
<img alt = "gif" src="Images/2021_10_16_polar_trail_2.gif">
<img src="Images/2021_10_16_polar_trail.png">

The curves were created in a for() loop inside Point VOP, in every loop, each point would sample a Curl noise, add it to its current position and add a new point in said position.

<img src="Images/Curl_Noise_Trail.png">

Afterward, I would normalize the Position attribute, convert it to polar coordinates, add the world and polar position together, while animating the world position. 

<img src="Images/Polar_Deform.png">

Full Node Tree:

<img src="Images/Node Tree.png">

<p align="center">
   I share my personal projects for free with everyone.
</p> 

<p align="center">
   You are welcome to explore all of them
   <a href="https://github.com/nitzan-treg/community_projects/">
      here
   </a>
</p> 
   

