<h2>Destructuring Exercise<h2>

<p><i>Object Destructuring 1</i><br><b>What does the following code return/print?</b></p>
<p>
let facts = {numPlanets: 8, yearNeptuneDiscovered: 1846};<br>
let {numPlanets, yearNeptuneDiscovered} = facts;<br>
<p></p>
console.log(numPlanets); // ?<br>
console.log(yearNeptuneDiscovered); // ?<br>
 </p>
 
<p><i>Object Destructuring 2</i><br><b>What does the following code return/print?</b></p>
<p>
let planetFacts = {<br>
  numPlanets: 8,<br>
  yearNeptuneDiscovered: 1846,<br>
  yearMarsDiscovered: 1659<br>
};
</p>
<p>
let {numPlanets, ...discoveryYears} = planetFacts;<br>

console.log(discoveryYears); // ?
</p>

  <p><i>Object Destructuring 3</i><br><b>What does the following code return/print?</b></p>
<p>
function getUserData({firstName, favoriteColor="green"}){<br>
  return `Your name is ${firstName} and you like ${favoriteColor}`;<br>
}
</p>
<p>
getUserData({firstName: "Alejandro", favoriteColor: "purple"}) // ?<br>
getUserData({firstName: "Melissa"}) // ?<br>
getUserData({}) // ?
</p>
  
  <p><i>Array Destructuring 1</i><br><b>What does the following code return/print?</b></p>
  <p>
  let [first, second, third] = ["Maya", "Marisa", "Chi"];<br>
  </p>
  <p>
console.log(first); // ?<br>
console.log(second); // ?<br>
console.log(third); // ?  
  </p>
  
  <p><i>Array Destructuring 2</i><br><b>What does the following code return/print?</b></p>
  <p>
  let [raindrops, whiskers, ...aFewOfMyFavoriteThings] = [<br>
  "Raindrops on roses",<br>
  "whiskers on kittens",<br>
  "Bright copper kettles",<br>
  "warm woolen mittens",<br>
  "Brown paper packages tied up with strings"<br>
]
  </p>
  <p>

console.log(raindrops); // ?<br>
console.log(whiskers); // ?<br>
console.log(aFewOfMyFavoriteThings); // ?
  </p>
  
<p><i>Array Destructuring 3</i><br><b>What does the following code return/print?</b></p>
<p>
let numbers = [10, 20, 30];<br>
[numbers[1], numbers[2]] = [numbers[2], numbers[1]]
</p>
<p>
console.log(numbers) // ?
</p>
  
<h2>ES2015 Refactoring<h2>

<p><i>ES5 Assigning Variables to Object Properties</i><br><b>Write an ES2015 Version</b></p>
<p>
var obj = {<br>
  numbers: {<br>
    a: 1,<br>
    b: 2<br>
  }<br>
};
</p>
<p>
var a = obj.numbers.a;<br>
var b = obj.numbers.b;
</p>
  
<p><i>ES5 Array Swap</i><br><b>Write an ES2015 Version</b></p>
<p>
var arr = [1, 2];<br>
var temp = arr[0];<br>
arr[0] = arr[1];<br>
arr[1] = temp;
</p>

  <p><b>raceResults()</b></p>
<p>
first: the first element in the array<br>
second: the second element in the array<br>
third: the third element in the array<br>
rest: all other elements in the array<br>
</p>
<p><b>Write a one line function to make this work using</b><br></p>
<p>
An arrow function<br>
Destructuring<br>
‘Enhanced’ object assignment (same key/value shortcut)
</p>
<p><br>Write a function called <b>raceResults</b> which accepts a single array argument. It should return an object with the keys <b>first, second, third,</b> and <b>rest</b>.</p>
<p>
raceResults(['Tom', 'Margaret', 'Allison', 'David', 'Pierre'])<br>

/*
  {<br>
    first: "Tom",<br>
    second: "Margaret",<br>
    third: "Allison",<br>
    rest: ["David", "Pierre"]<br>
  }<br>
*/
</p>
