#  Strange Attractor
This project is based on Entagma's tutorial: https://entagma.com/vex-in-houdini-strange-attractors/
the tutorial teachs how to create an attractor by following a differtial equation from the site http://3d-meier.de/

I found a way to optemize the setup by running the whole simulation inside a single attribute wrangler where each step is run over in a for() loop, this optimization is about 500 times faster and can be developed further to be multithreaded:

vector pos = chv('start_pos');
float dt = chf('accurcy');
int steps = chi('steps');

float x,y,z,a,b,c,d,e,k,f;

a = 40;
c = 1.833;
d = 0.16;
e = 0.65;
k = 55;
f = 20;

x = pos.x;
y = pos.y;
z = pos.z;

for(int step=0;step<steps;step++){
    x += (a * (y-x) + d*x*z) * dt;
    y += (k*x + f*y - x*z) * dt;
    z += (c*z + x*y - e*x*x) * dt;
    
    pos = set(x,y,z);
    
    int new_pt = addpoint(0,pos);
}