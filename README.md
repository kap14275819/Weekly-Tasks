# Weekly-Tasks-Maths

## Greatest Common Divisor and Least Common Multiple:
#### In maths the Greatest Common Divisor (GCD) is the largest positive integer that divides into two or more intergers which are not all 0.
#### In maths the Least Common Multiple (LCM) is The least common multiple to appear in a list of multiplications of two or more intergers which are not all 0.

### Examples

#### What is the GCD of 22 and 32 ?
#### The divisors of 22 are 1, 2, 11, 12.
#### The divisors of 32 are 1, 2, 4, 8, 16, 32.
#### Both have 1 and 2 in their lists. This means that 2 is the GCD.
#### What is the LCM of 6 and 10 ?
#### The Multiplications of 6 are 6, 12, 18, 24, 30, 36, 42, ... And so on.
#### The Mulitplications of 10 are 10, 20, 30, 40, 50, 60, ... And so on.
#### The LCM in these lists is 30, therefore the LCM of 6 and 10 is 30.

## Conditional Probability:

#### Conditional probability is when the probability of an event (A), given that another event (B) has already occured.

### Examples

#### What is the probability of having a 8 when rolling two die?
#### Chances / Total = 6/36 = 1/6
#### What is the probability of having a 8 after rolling a 2?
#### Chances / Total = 1/6
#### What is the probability of having at least one 2 when rolling two die?
#### Chances / Total = 11/36

## Expectations of an event:

#### Infinite Probability means that any section of time and space can be divided into an infinite number of smaller and smaller pieces. For example, 10 feet can be subdivided into 1 foot sections, 0.1 foot sections, 0.00001 foot sections…and so on. However, infinite divisibility in probability theory has a more defined meaning.
#### A probability distribution is infinitely divisible if it can be written as the sum of n independent and identically distributed random variables for any positive integer n.

### Formula
### ![formula](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/formula%20event.jpg)

### Examples

#### What is the probability of a random interger being divisible by 5?
#### Range 1-100 / Total = 20/100 = 1/5

#### What is the probability of a random interger being divisible by 10?
#### Range 1-100 / Total = 10/100 = 1/10

## Vectors
#### A vector is a quantity or phenomenon that has two independent properties: magnitudeand direction. The term also denotes the mathematical or geometrical representation of such a quantity.

### ![Vector](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/vector.png)

#### Vectors play an important role in physics: the velocity and acceleration of a moving object and the forces acting on it can all be described with vectors. Many other physical quantities can be usefully thought of as vectors. Although most of them do not represent distances (except, for example, position or displacement), their magnitude and direction can still be represented by the length and direction of an arrow. The mathematical representation of a physical vector depends on the coordinate system used to describe it. Other vector-like objects that describe physical quantities and transform in a similar way under changes of the coordinate system include pseudovectors and tensors.

### Script to determine shapes using vectors
```html 
<html>
<body>

<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;"></canvas>

<br>
<button onclick="move(1)">LEFT</button>
<button onclick="move(2)">UP</button>
<button onclick="move(3)">DOWN</button>
<button onclick="move(4)">RIGHT</button>
<br>
<button onclick="move(5)">DIAGONAL RIGHT DOWN</button>
<button onclick="move(6)">DIAGONAL RIGHT UP</button>
<br>
<button onclick="move(7)">DIAGONAL LEFT DOWN</button>
<button onclick="move(8)">DIAGONAL LEFT UP</button>
<br>
<button onclick="shape()">SHAPE?</button>


<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();

var curX=parseInt(prompt("Please enter the initial X"));;
var curY=parseInt(prompt("Please enter the initial Y"));;

function move(dir){
var mag = parseInt(prompt("Please enter the magnitude"));

if(dir==1){
  //left
  ctx.moveTo(curX, curY);
  curX = curX-mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Left / Vector Magnitude: "+mag);
}else if(dir==2){
  //up
  ctx.moveTo(curX, curY);
  curY = curY-mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Up / Vector Magnitude: "+mag);
}else if(dir==3){
  //down
  ctx.moveTo(curX, curY);
  curY = curY+mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Down / Vector Magnitude: "+mag);
}else if(dir==4){
  //right
  ctx.moveTo(curX, curY);
  curX = curX+mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Right / Vector Magnitude: "+mag);
}else if(dir==5){
  //diagonal right down
  ctx.moveTo(curX, curY);
  curX = curX+mag/2;
  curY = curY+mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Right Down / Vector Magnitude: "+mag);
}else if(dir==6){
  //diagonal right up
  ctx.moveTo(curX, curY);
  curX = curX+mag/2;
  curY = curY-mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Right Up / Vector Magnitude: "+mag);
}else if(dir==7){
  //diagonal left down
  ctx.moveTo(curX, curY);
  curX = curX-mag/2;
  curY = curY+mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Left Down / Vector Magnitude: "+mag);
}else if(dir==8){
  //diagonal left up
  ctx.moveTo(curX, curY);
  curX = curX-mag/2;
  curY = curY-mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Left Up / Vector Magnitude: "+mag);
}

ctx.stroke();

}

function shape(){
  var shape = prompt("Is this a shape Y/N?");

  if(shape=='Y'){
      prompt("What shape?");
  }else {
      alert("Keep drawing!");
  }
}

</script>

</body>
</html>
```

## Integral Calculus
#### Integration can be used to find areas, volumes, central points and many useful things. When there is a curve that is needed to be calculated, it can be done through using Integral Calculus, when looking at complex shapes that are curved, normal methods of working out the area inside the shape cannot be used, instead we use this method.

#### In order to complete this calculation, there cannot be one area to look at but several, so what we do is create multiple rectangles within the area in order to figure out each one, by doing so we will be able to figure out the area.

### Area
#### ![area](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/integ.png)
#### ![arearec](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/area%20rectangle.JPG)

### Formulas
#### Here are some forumlas used for figuring out Integral Calculus
#### ![formula](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/main%20formulas.JPG)
#### ![formula](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/formula.png)

#### The symbol ∫ represents intergration within the formula, this is where the intergral is found. The opposite of this is derivation.

#### The two letters a and b are both placed on either side of the ∫ symbol as the calculations are going from a to b. The two letters that are both together is dx, this shows the differential of the variable which is x, this shows the variable of integration is also x. The area is found from the x axis from the curve, this means the integral of the function must be x.

#### We can now calculate the area of the curve and infinite rectangles to find the area. We do this by multiplying the function by the derivative of the function. The formula of the area of one of the rectangles is already known, this means that we can calculate this much easier.

## Rate of Change

#### The rate of change means the average rate at which one quantity is changing with respect to something else changing.
#### There are already some familiar average rate of change calculations such as:
#### 1. Miles per gallon-calculated by dividing the number of miles by the number of gallons used.
#### 2. Cost per kilowatt-calculated by dividing the cost of the electricity by the number of kilowatts used.
#### 3. Miles per hour-calculated by dividing the number of miles travelled by the number of hours it takes to travel them.

### Average Rate of Change function

#### In general, an average rate a change function is a process that calculates the the amount of change in one item divided by the corresponding amount of change in another. Using function notation, we can define the Average rate of Change of a function from a to x:

#### ![formula](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/rate%20of%20change.png)

### Average Rate of Change function

#### F(x) = x2
#### Rate of change from 1 to 3
#### (32  -12) / (3 -1) = (9 –1) / (3 –1) = 8/2 = 4
#### F(x) = 2x+3
#### Rate of change from 10 to 100
#### (2*100 + 3) –(2*10 + 3) / (100 –10) = 180 / 90 = 2
