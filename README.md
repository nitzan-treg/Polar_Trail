#  Davidoe II
This project is very much inspired by davidope's art

Its an attempt to create a satisfying looping animation in the black & white style of davidope
I used a falloff and a rotation matrix to control the animation

---

//get data
int prims[] = pointprims(0,i@ptnum);
float falloff = f@falloff;
matrix xform = ident();

//rotate matix
vector rnd_axis = normalize(rand(prims[0]+111));
v@rnd_axis = rnd_axis;
float rotate_amp = radians(chf('rotate_amount')*falloff);
rotate(xform,rotate_amp,rnd_axis);

v@P*=xform;

---

<img src="Images/Node Tree.png">
<p><img alt = "gif" src="2021_10_09_dvdp_II.gif"></code>