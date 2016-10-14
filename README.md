# Hello-World

Im just a highschool student in a big world 

// Example 2-2 work

void setup() {
 size(480, 120);
 smooth();
}
void draw() {
 if (mousePressed) {
 fill(0);
 } else {
 fill(255);
 }
 ellipse(mouseX, mouseY, 80, 80);
}

//example 3-7 work 

void setup() 
{
 size(120, 120);
 arc(60,60,80,80,radians(45),radians(310));
 ellipse(65,40,10,10);
}

// example 3-13 work 

void setup() 
{
size(600, 120);
smooth();
strokeWeight(12);
strokeJoin(ROUND); // Round the stroke corners
rect(40, 25, 70, 70);
strokeJoin(BEVEL); // Bevel the stroke corners
rect(140, 25, 70, 70);
strokeCap(SQUARE); // Square the line endings
line(270, 25, 340, 95);
strokeCap(ROUND); // Round the line endings
line(350, 25, 420, 95);
ellipse(510,60,70,70);
strokeCap(ROUND);
}

//Class Logo

void setup() 
{
size(600,600);
fill(52,226,255);
triangle(300,250,300,175,250,230);
fill(201,245,252);
triangle(300,250,300,175,350,230);
fill(51,84,139);
quad(300,290,300,500,100,450,225,255);
fill(0,45,121);
quad(300,290,300,500,500,450,375,255);
}

// Monster 

strokeWeight(14);
  background(196, 255,248); 
    
    fill(255, 0, 0);
    beginShape();
    vertex(300,250);
    vertex(250,300);
    vertex(350,300);
    vertex(150,400);
    vertex(450,400);
    vertex(250,500);
    endShape();

    fill(0, 255, 0); 
    beginShape();
    vertex(250,300);
    vertex(300,250);
    vertex(300,350);
    vertex(400,150);
    vertex(400,450);
    vertex(500,250);
    endShape();
    
    strokeWeight(2);
    line(300,300,100,300);
    line(300,300,300,100);

}





