# Processing_drawings-3

/*

Your name: Elias Han

Date: 9/28/18

Project/assignment name: Java Drawings

Description: This is Pac Man

Credits for code referenced:
https://processing.org/reference/arc_.html
https://processing.org/tutorials/transform2d/
https://processing.org/tutorials/color/
https://processing.org/tutorials/drawing/

Notes: Used:
Color
Arc
Ellipse
2D transformation

*/

void setup()
{
  size(200, 200);
  background(0);
  smooth();
  fill(color(255,255,0));
  noStroke();                //this block sets up properties (not size or coordinates) of Pac-man
  
  translate(50,100);                       //translates graph so that Pac is still fully on screen
  rotate(QUARTER_PI);                      //rotates Pac-Man 45 degrees to the right
  arc(0, 0, 90, 90, 0, PI+HALF_PI, PIE);   //<--original non-rotated Pac Man 
}

void draw(){                    //draws the pellets
ellipse(70, 100, 10, 10);
ellipse(90, 100, 10, 10);
ellipse(110, 100, 10, 10);
fill(255);
}      
