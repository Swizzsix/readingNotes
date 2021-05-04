# READ 02
## HTML Jon Duckett
### Chapter 2: “Text” (pp.40-61) 
- Headings = <h1>-<h6> paragraphs = <p> bold = <b> italic = <i> line break = <br> emphasis = em
- "HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs)."
- "They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation)."
### Chapter 10: Ch.10 “Introducing CSS” (pp.226-245) 
#### SUMMARY: 
- "CSS trats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look"  
- "Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like)"
- "Different types of selectors allow you to target your rules at different elements"
- "Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. for example, the font-family property sets the choice of font and the value arial specifies Arial as the preffered typeface."
- "CSS rules usually appear in a seperate document, although they may appear within an HTML page."
## JS Jon Duckett
### Chapter 2: “Basic JavaScript Instructions” (pp.53-84)
- STATEMENTS:
let today = new Date();
let hourNow = today.getHours();
let greeting;
  if (hourNow > 18){
  greeting = 'Good evening';
} else if (hourNow > 12){
  greeting = 'good afternoon';
} else if (hourNow > 0){
  greeting = 'Good Morning';
} else {
  greeting = 'welcome';
}
  document.write(greeting);
- COMMENTS = //
- USING A VARIABLE TO STORE A NUMBER:
let price;
let quantity; 
let total;

price = 5;
quantity = 14;
total = price * quantity;

let el = document.getElementById('cost');
el.textContent = '$' + total;

- message = '<a href=\"sale.html\">25% off!</a>';
- ARRAY = 
let colors;
colors = ['white', 'black', 'custom']; 
let el = document.getElementById('colors');
el.textContent = colors[0];

- ASSIGNMENT OPERATORS: color = 'biege';
- ARITHMETIC OPERATORS: area = 3 * 2;
- STRING OPERATORS: greeting = 'hi ' + 'Molly';
- ARITHMETIC OPERATORS: (addition +) (subtraction -) (divison /) (multiplcation *) (increment ++) (decrement --)
(modulus = %) 10 % 3 = 1 divides two values and returns remainder

- STRING OPERATORS
let greeting = 'Howdy ';
let name = 'molly';

let welcomeMessage = greeting + name + 'i';
el.textContent = welcomeMessage;

#### SUMMARY: 
- "A script is made up of a series of statemenets. Each statement is like a step in a recipe."
- "Scripts contain very precise instructions. For example. you might specify that a value must be remembered before creating a calculation using that value"
- "variables are used to temporarily store pieces of information used in the script"
- "arrays are a special types of variables that store more than one piece of related information."
- "Javascript distinguishes betwenn numbers (0-9), strings (text) and BOOLEAN values (true or false)"
- "expressions evaluate into a single value"
- "expressions rely on operators to calucalte a value"

### Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)
- DECISION MAKING = Question: YES/NO if/else
if (score > 50){
  document.write('You Passed!');
} else {
  docuument.write('Try again...');
}

- COMPARISON OPERATORS:
(== is equal to) (!= is not equal to) (=== strictly equal to) (!== strict not equal to) (> greater than)
(< less than) (>= greater than of equal to) (<= less than or equal to)

- USING COMPARISON OPERATORS:
let pass = 50; //pass mark
let score = 90; //score

//check if the user has passed
let hasPassed = score >= pass;

//write the message into the page
let el = document.getElementById('answer');
el.textcontent = 'level passed: ' + hasPassed;

- USING EXPRESSIONS WITH COMPARISON OPERATORS
((score1 + score2) > (highScore1 + highScore2))

- LOGICAL OPERATORS
- (&& = this operator tests more than one condition)
  ((5 < 2) && (2 >= 3))
   false       false
- (|| = this operator tests at least one condition)
  ((2 < 5) && (2 < 1))
          true
"if either expression evaluates to true, then the expression returns true. if both return false, then the expresssion will return false."
- (! = this operator takes a single boolean value and inverts it)
  !(2 < 1) = true
  !true returns false
  !false returns true

  -TRUTHY/FALSEY values

#### LOOPS
- FOR = "if you need to run a code a specific number of times, use a for loop"
- WHILE = "if you do not know how mnay times the code should run, you can use a while loop" 
- DO WHILE = "similar to while loop but will run entire statement in curly braces even if false"

for (let i = 0; i < 10; i++) {
    document.write (i);
}

- LOOP THROUGH ARRAY LENGTH

for (i = 0; i < arrayLength; i++){

}








