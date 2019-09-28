Q: What code draws the blades of grass? 

A: If the grass naturally grow the code will be 
```bash
function draw() {
  stroke(random(60, 70), 100, 90);
  line(x, height-10, x+random(-10, 10), height-10-random(h));
  noStroke();

  x = x + 10;

  if (x > width) {
    x = random(10);
    h = h + 3;
  } 

```

Q: What code makes the "lawnmower" come by? How often does it come by? 

A: 0.01% chance of coming 

```bash
  if (random(100) > 99.9) {
    fill(255);
    rect(0, 0, width, height-15);
    h = 10;
  }
	
```

	
Q: What's the point of the h variable? 

A: Set the heighet of the grass.(Make it grow tall/cut short)



Q:What does the -10 do in the second and fourth arguments of the line function, height-10-random(h)? 

A: set the initail height to 0





