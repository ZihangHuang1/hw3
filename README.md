# hw3
1. What code draws the blades of grass?
stroke(random(60, 70), 100, 90);
  line(x, height-10, x+random(-10, 10), height-10-random(h));

2. What code makes the "lawnmower" come by? How often does it come by?
   if (random() > 0.999) {
    fill(255);
    rect(0, 0, width, height-15);
    h = 10;
Whatever when the function returns the number between 0.999 and 1, because random does not include the number 1

3. What's the point of the h variable?
To keep track of the grass' height. The variable is incremented by 3 every time the function is looped. It also sets the y coordinates for the lines of each grass blade

4. What does the -10 do in the second and fourth arguments of the line function, height-10-random(h)? Why is it there?
Height-10 is to set the root of the blades at the rectangle and the height-10-random(h) is to set the top of one blade height as 5 which makes it look like its growing.

