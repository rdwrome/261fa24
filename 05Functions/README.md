## Functions
- takes input value, does a process to it, returns an output value
- we've been using many that are already built-in, now we'll write our own!
- Useful for repetitive code
```python FIX RACHEL
# a = x * x * 3.14 is repeatedly used.

a = 3.0 * 3.0 * 3.14
print("The are of circle with radius 3 is: ", a)

a = 5.0 * 5.0 * 3.14
print("The are of circle with radius 5 is: ", a)

a = 7.0 * 7.0 * 3.14
print("The are of circle with radius 7 is: ", a)

a = 11.0 * 11.0 * 3.14
print("The are of circle with radius 11 is: ", a)
```
becomes
```python
# Simplify to three lines of code
# Now we just need to change the number for x
# to get different answers with the same equation.

function circleArea(x) {
  return x * x * 3.14;
}

console.log(circleArea(3.0));
)
```


- Function with no input
```
function hello() {
  console.log("Hello, World!");
}

hello();

```

- Function with one argument/parameter
```
function cube(n) {
  return n * n * n;
}

console.log(cube(2));

```

- Function with default argument
```
function displayInstrument(name, instrument = "Guitar") {
  console.log(name + " likes " + instrument);
}

displayInstrument("Jennifer");
displayInstrument("Elizabeth", "Drum");
displayInstrument("Susan", "Bass");


```

- Function with Multiple Inputs
```
function sqr(x, n) {
  return Math.pow(x, n);
}

console.log(sqr(2, 3));

```
- Function with Multiple Outputs
```
function getInstruments() {
  return ["Drum", "Guitar", "Bass"];
}

let instruments = getInstruments();
let primary = instruments[0];
let secondary = instruments[1];
let tertiary = instruments[2];

console.log("My Instruments are: " + primary + ", " + secondary + ", " + tertiary);

```


- Nesting Function Calls
```
function printLyrics() {
  console.log("I'm gonna take my horse to the old town road.");
  console.log("I'm gonna ride 'til I can't no more.");
}

function repeatLyrics() {
  printLyrics();
  printLyrics();
}

repeatLyrics();

```

- Function with 'if'
```
function minimum(x, y) {
  if (x < y) {
    return x;
  }
  return y;
}

console.log(minimum(3, 4));
```
- Function with 'if/else'
```
function factorial(n) {
  if (n === 0) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

console.log(factorial(3));
```

- Functions with 'for'
```function sumup(n) {
  let sum = 0;
  for (let i = 0; i <= n; i++) {
    sum += i;
  }
  return sum;
}

console.log(sumup(5));
```
- Function with local variable
```
function printFavoriteInstrument() {
  let instrument = prompt("What is your favorite instrument?");
  console.log("Your favorite instrument is: " + instrument);
}

function printLeastFavoriteInstrument() {
  let instrument = prompt("What is your least favorite instrument?");
  console.log("Your least favorite instrument is: " + instrument);
}

printFavoriteInstrument();
printLeastFavoriteInstrument();
```
- Function with global variable
```name = input("What is your name? ")

def display_name():
  global name
  print("Your name is: ", name)
  name = input(f"Are you sure your name is {name}? ")
  print(name)

display_name()
```
// two eyes
function setup() {
  createCanvas(100, 100);
  noStroke();
}

function draw() {
  background(204);

  // Right Eye
  fill(255);
  ellipse(65, 44, 60, 60);
  fill(0);
  ellipse(75, 44, 30, 30);
  fill(255);
  ellipse(81, 39, 6, 6);

  // Left Eye
  fill(255);
  ellipse(20, 50, 60, 60);
  fill(0);
  ellipse(30, 50, 30, 30);
  fill(255);
  ellipse(36, 45, 6, 6);
}

- GROUP EXERCISE:
- Write a program that prints out a graph of `y = x^2` (^2 means power of 2) horizontally. The print out of the graph should look like the following:

```
****************************************************************
*************************************************
************************************
*************************
****************
*********
****
*

*
****
*********
****************
*************************
************************************
*************************************************
****************************************************************

- LAST WEEK AND MOVE ON
// draw eye
function setup() {
  createCanvas(100, 100);
  noStroke();
}

function draw() {
  background(204);
  fill(255);
  ellipse(50, 50, 60, 60);
  fill(0);
  ellipse(60, 50, 30, 30);
  fill(255);
  ellipse(66, 45, 6, 6);
}

//eyes
function setup() {
  createCanvas(100, 100);
  noStroke();
}

function eye(x, y) {
  fill(255);
  ellipse(x, y, 60, 60);
  fill(0);
  ellipse(x + 10, y, 30, 30);
  fill(255);
  ellipse(x + 16, y - 5, 6, 6);
}

function draw() {
  background(204);
  eye(65, 44);
  eye(20, 50);
  eye(65, 74);
  eye(20, 80);
  eye(65, 104);
  eye(20, 110);
}

// draw eyes
function setup() {
  createCanvas(400, 400);
  noStroke();
}

function draw() {
  background(204);
  eye(mouseX, mouseY);
}

function eye(x, y) {
  fill(255);
  ellipse(x, y, 60, 60);
  fill(0);
  ellipse(x + 10, y, 30, 30);
  fill(255);
  ellipse(x + 16, y - 5, 6, 6);
}

```

