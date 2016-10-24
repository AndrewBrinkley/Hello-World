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

void setup() 
{
  size(600,600);
  smooth();
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

// Robot 2 

void setup() 
{
int x = 60; // x-coordinate
int y = 420; // y-coordinate
int bodyHeight = 210; // Body Height
int neckHeight = 40; // Neck Height
int radius = 45; // Head Radius
int ny = y - bodyHeight - neckHeight - radius; // Neck Y
size(170, 480);
smooth();
strokeWeight(2);
background(204);
ellipseMode(RADIUS);
// Neck
stroke(102);
line(x+2, y-bodyHeight, x+2, ny);
line(x+12, y-bodyHeight, x+12, ny);
line(x+22, y-bodyHeight, x+22, ny);
// Antennae
line(x+12, ny, x-18, ny-43);
line(x+12, ny, x+42, ny-99);
line(x+12, ny, x+78, ny+15);
// Body
noStroke();
fill(102);
ellipse(x, y-33, 33, 33);
fill(0);
rect(x-45, y-bodyHeight, 90, bodyHeight-33);
fill(102);
rect(x-45, y-bodyHeight+17, 90, 6);
// Head
fill(0);
ellipse(x+12, ny, radius, radius);
fill(255);
ellipse(x+24, ny-6, 14, 14);
fill(0);
ellipse(x+24, ny-6, 3, 3);
fill(153);
ellipse(x, ny-8, 5, 5);
ellipse(x+30, ny-26, 4, 4);
ellipse(x+41, ny+6, 3, 3);
}



//part 3

int x = 300;
int y = 300;
int a = 200;
int b = 350;
int c = 250;
int radius = 40;


   void setup()
    {  
    background(63,111,240);
    size(600,600);
    }
  
  void draw()
  {
    
    strokeWeight(14);
       
    
      if (keyPressed && (key == CODED)) 
       { 
         if (keyCode == UP) 
         { 
           y--;
         } 
         else if (keyCode == DOWN) 
         {
           y++;
         }
       }    
       
       if (keyPressed && (key == CODED)) 
       { 
         if (keyCode == LEFT) 
         { 
           x--;
         } 
         else if (keyCode == RIGHT) 
         {
           x++;
         }
       }    

    fill(255,243,103);
    ellipse(x,y,400,400);
    
     if (keyPressed) {
 if ((key == 'q') || (key == 'Q')) {
 fill(239,26,255);
 ellipse(x,y,400,400);
 }
 else if ((key == 'w') || (key == 'W')) {
 fill(8,252,5);
 ellipse(x,y,400,400);
 }
 }
    fill(255,243,103);
   
   strokeWeight(7);
    fill(255,255,255);
    ellipse(a,c,100,100);
    ellipse(b,c,100,100);
    
    float d = dist(mouseX, mouseY, a, c);
    if (d < radius) 
    {
      fill(0);
      ellipse(mouseX,mouseY,radius,radius);
    }
     float f = dist(mouseX, mouseY, b, c);
    if (f < radius) 
    {
      fill(0);
      ellipse(mouseX,mouseY,radius,radius);
    }
   

    line(200,400,400,400);
  }

//example 6-7

PFont font;
void setup() {
 size(480, 120);
 font = loadFont("DialogInput-30.vlw");
 textFont(font);
}
void draw() {
 background(102);
 text("andrew brinkley ", 26, 30, 240, 400);
}

PFont font;
void setup() {
 size(480, 120);
 font = loadFont("DialogInput-30.vlw");
 textFont(font);
}
void draw() {
 background(102);
 text("andrew brinkley ", 26, 30, 240, 400);
}

// 7 -4 

int radius = 40;
float x = -radius;
float speed = 0.5;
void setup() {
 size(240, 120);
 smooth();
 ellipseMode(RADIUS);
}
void draw() {
 background(0);
 x += speed; // Increase the value of x
 if (x > width+radius) { // If the shape is off screen,
 x = -radius; // move to the left edge
 }
 arc(x, 60, radius, radius, 0.52, 5.76);
}


// Pong ?

int radius = 25;
float direction = 1;
float direction2 =.75;
float x = 600;
float y = 300;
float time;
int x2 = 100;
int y2= 250;
int z = 1050;
int score ;
float speed = 10;


void setup() {
  size(1200,600);
  smooth();
 // background(0);
  ellipseMode(RADIUS);
}

void draw() 
{
  background(0);
   
   fill(225);
   text("score:" + score , width/2, 50 );
   
   time= millis();
   fill(255);
   text("Time:" + time/1000, width/2, height-50);
   
   if (keyPressed && (key == CODED)) 
   { 
     if (keyCode == UP) 
     { 
     y2 = y2 - 10;
     } 
     else if (keyCode == DOWN) 
     {
     y2 = y2 + 10;
     }
   }    

   if (keyPressed && (key == CODED)) 
   { 
      if (keyCode == LEFT) 
      { 
      x2 = x2 - 10;
      } 
      else if (keyCode == RIGHT) 
      {
      x2 = x2 + 10 ;
      }
   }    
      rect(x2,y2,25,100);
  
   if (keyPressed && (key == CODED)) 
   { 
      if (keyCode == UP) 
      { 
      y2 -- ;
      } 
      else if (keyCode == DOWN) 
      {
      y2 ++ ;
      }
   }    

   if (keyPressed && (key == CODED)) 
   { 
      if (keyCode == LEFT) 
      { 
      x2 -- ;
      } 
      else if (keyCode == RIGHT) 
      {
      x2 ++ ;
      }
   }    
   
      
     //  rect(z,y2,25,100);
  
  
      x += speed * direction ;
      if ((x > width-radius) || (x < radius) || (x < x2 + radius ))
      {
       direction = -direction ;
       score += 1;
      }
      y += speed * direction2;
      if ((y > height-radius) || (y < radius))
      {
       direction2 = -direction2;
       score += 1;
      }
      ellipse(x,y,radius,radius);
}


// 8-7

void setup() {
 size(480, 120);
 smooth();
}
void draw() {
 background(204);
 randomSeed(0);
 for (int i = 35; i < width + 40; i += 40) {
 int gray = int(random(64,225));
 float scalar = random(0.25, 1.0);
 owl(i, 110, gray, scalar);
 }
}
  
void owl(int x, int y, int g, float s) {
 pushMatrix();
 translate(x, y);
 scale(s); // Set the size
 stroke(g); // Set the gray value
 strokeWeight(70);
 line(0, -35, 0, -65); // Body
 noStroke();
 fill(255-g);
 ellipse(-17.5, -65, 35, 35); // Left eye dome
 ellipse(17.5, -65, 35, 35); // Right eye dome
 arc(0, -65, 70, 70, 0, PI); // Chin
 fill(g);
 ellipse(-14, -65, 8, 8); // Left eye
 ellipse(14, -65, 8, 8); // Right eye
 quad(0, -58, 4, -51, 0, -44, -4, -51); // Beak
 popMatrix();
} 


//spinsagram

PImage img;
int x ;
int y ;
int r ; 


void setup() {
  background(0);
  size(600,600);
  imageMode(CENTER);
 img = loadImage("yak.png");
}
void draw() {
   
  if (key== CODED && keyCode == LEFT )
  {
    r-- ;
  } else if ( key== CODED && keyCode == RIGHT )
  {
    r++ ;
  }
  
  if (key== CODED && keyCode == UP)
  {
    x++ ;
  } else if ( key== CODED && keyCode == DOWN)
  {
    x-- ;
  }
  if (keyPressed && key == 'r')
  {
    tint(255,0,0,255);
  }
   if (keyPressed && key == 'g')
  {
    tint(0,255,0,255);
  }
   if (keyPressed && key == 'b')
  {
    tint(0,0,255,255);
  }
  if (keyPressed && key == 'z')
  {
    tint(144,144,144,255);
  }
  
  
  translate(width/2,height/2);
  rotate(radians(r));
  image(img,0,0,200+x,200+x);
}
