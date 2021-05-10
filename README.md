# Code 201 Reading Notes
## Table of Contents
- 2MAY2021 READ 01 Lines 5-34
- 3MAY2021 READ 02 Lines 36-161
- 4MAY2021 READ 03 Lines 162-203
- 5MAY2021 READ 04 Lines 206-254
- 6MAY2021 READ 05 Lines 249-277
- 6MAY2021 READ 06 Lines 
# READ 01
## HTML Jon Duckett
### Chapter 1: “Structure” (pp.12-39) 
- Element = closing/opening tag
- "HTML pages are text documents"
- "tags are often reffered to as elements"
- "opening tags can carry attributes, which tell us more about the content of that element
- "attributes require a name and value"
### Chapter 8: “Extra Markup” (p.176-199) 
- block elements =  h1> <li> <ul> <p> 
- Inline elements = <a> <b> <em> <img>
- "DOCTYPES tell browsers which version of HTML you are using"
- "The ID and class attributes allow you to group block level and inline elements together"
- "the <div> and <span> elements allow you to group block level and inline lements together"
- "the <meta> tag allows you to supply all kinds of information about your web page"
### Chapter 17: “HTML5 Layout” (pp.428-451) 
- "<nav> element is used to contain the major navigational blocks on the site such as the primary site navigation"
- "<article> element acts as a container for any section of a page that could stand alone and potentially be syndicated"
- "<aside> element has two purposes, depending on whether it is inside an <article> element or not"
### Chapter 18: “Process & Design” (pp.452-475)
- "A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require"
- target audience is important


## JS Jon Duckett
### Chapter 1: “The ABC of Programming” (pp.11-52)
- "A script is a series of instructions"
- Objects have properties 
- event = change 
- Method = how things interact with object in real world

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

# READ 03
## HTML Jon Duckett
### Chapter 3: “Lists” (pp.62-73)
- ol/ul = ordered list/unordered list li = list item 
- nested lists
- ordered lists used numbers while unordered lists use bullets 

### Chapter 13: “Boxes” (pp.300-329)
#### SUMMARY: 
- CSS treats each HTML element as its own box  
- border margin padding
- top right bottom left
- border radius em
- "Different types of selectors allow you to target your rules at different elements"
- "Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. for example, the font-family property sets the choice of font and the value arial specifies Arial as the preffered typeface."
- "CSS rules usually appear in a seperate document, although they may appear within an HTML page."

## JS Jon Duckett
### Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)
- "An array is a special type of variable. It doesn't jsut store one value; it stores a list of values."

let colors;
colors = ['white', 'black', 'custom'];
0 white
1 black
2 custom

colors [2] = 'biege';
let el = document.getElementById('colors');

el.textContent = colors [2];

### Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)
I covered this chapter in class -02 reading notes.

# READ 04
## HTML Jon Duckett
### Chapter 4: Ch.4 “Links” (pp.74-93)
    -"Links are the defining feature of the web because they allow you to move from one web page to another -- enabling the very idea of browsing or surfing."
    -<a hreg =""> IMDB </a>
    - DIRECTORY STRUCTURE root folder 
    - grandparent/parent/sibling/child grandchild
    - Root Folder = index.html and directories
    - RELATIVE URLS = 
    - SAME FOLDER <a href ="reviews.html">Reviews</a>
    - CHILD FOLDER <a href ="music/listings.html">Listings</a>
    - GRANDCHILD FOLDER <a href ="movies/dvd/reviews.html'>Reviews</a>
    - PARENT FOLDER <a href ="../index.html">Home</a>
    - GRANDPARENT FOLDER <a href ="../../index.html">Home</a>
    - opening links in NEW WINDOW <a href ="http://www.imdb.com" target="_blank">
    - Linking to a specific part of the same page <h2 id = "arc_shot">Arc Shot</h2> <a href="#arc_shot">Arc Shot</a><br />


### Chapter 15: “Layout” (pp.358-404)
#### SUMMARY: 
    - "css treats HTML element as if it is in itts own box. This will either be a block level box or an inline box"
    - Normal Flow = every block element new line
    - relative positioning = moves position relative to normal flow
    - absolute = taken out of normal flow and absolute to block element
    - Fixed = in relation to browser window
    - float = take element in normal flow and place as far to left or right of containing element as possible
    - FIXED WIDTH LAYOUTS = greater control of liquid elements + size of image will always stay the same DISADVANTAGES = large gaps look smaller with higher resolution screen and more verticle space.
    - LIQUID LAYOURS = pages expand to fit entire page of layout + if user has small window can contract to fit it ithout user having to scroll - resolution problems too wide


## JS Jon Duckett
### Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)
    - functions & methods + objects + built in objects 
    - function has parameters 
    - DECLARE  function sayHello(){ document.write('Hello');}
    - CALLING a function sayHello();
    - PARAMETERS = function getArea(width, height)
    - ARGUMENTS =  getArea(3, 5);
    - MULTIPLE VALUES FUNCTION = multiple parameters and values with comparison operators and array of let values and call new arguments for whatever numbers
    - LOCAL VARIABLES/GLOBAL VARIABLES



### Article: “6 Reasons for Pair Programming”
    - DRIVER/NAVIGATOR
    - DRIVER GETS TO DRIVE USING THE EXPERIENCE OF THE NAVIGATOR AND VICE VERSA
    - ALLOWS TWO MINDS TO WORK ONE PROJECT
    - HELPS WITH EFFICIENCY AND CREATIVITY AND SOLIDIFIES LEARNING
    - WORKS WELL WITH PEOPLE WHO HAVE CHEMISTRY THAT IS BUILT OVER TIME

 # READ 05
## HTML Jon Duckett
### Chapter 5: “Images” (pp.94-125)
    - mkdir images/assets for images
    - download adobe photoshop
    - img format = JPEG, GIF, 
    - "The <img> element is used to add images to a web page"
    - add source and alt attributes


### Chapter 11: “Color” (pp.246-263)
#### SUMMARY: 
    - color values = RGB, HEX CODES, COLOR NAMES
    - background-color
    - opacity 
    - contrast 

### Chapter 12: “Text” (pp.264-299)
    - typeface terminology = SERIF, SANS SERIF, MONOSPACE, CURSIVE, FANTASY
    - unites of type size = pixels, percentages, EMS
    - styling links = :link, :visited
    - ATTRIBUTE SELECTORS 


## Blog Post
### JPEG vs PNG vs GIF NOTE: The post has a TL;DR you might find hand
    - COMPRESSION TYPES = lossless, lossy
    - JPEGS are bigger in size and better in quality than PNG
    - JPEG = lossy && PNG || = LOSSLESS
