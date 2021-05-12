# Code 201 Reading Notes
## Table of Contents
- 2MAY2021 READ 01 Lines 5-34
- 3MAY2021 READ 02 Lines 36-161
- 4MAY2021 READ 03 Lines 162-203
- 5MAY2021 READ 04 Lines 206-254
- 8MAY2021 READ 05 Lines 249-277
- 7MAY2021 READ 06 Lines 281-297
- 10MAY2021 READ 07 Lines 309-327
- 11MAY2021 READ 08 Lines 330-337
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

# READ 06
## Jon Duckett JS Book
### Chapter 3: “Object Literals” (pp.100-105)
    - Object/Variables = properties
    - Object/Functions = Mehods


### Chapter 5: “Document Object Model” (pp.183-242)
#### SUMMARY: 
    - ""The browser represents the page using a DOM tree""
    - "DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes."
    - "You can select element nodes by their id or class attributes, by tag name, or by using CSS selector syntax"
    - "whenever a DOM query can return more than one node, it will always return a Nodelist"
    - "From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manitpulation techniques."
    -"An element node can contain multple text nodes and child elements that are siblines of each other"
    -"In older browsers, implementation of the DOM is inconsistent. (and is a popular reason for using JQUIERY)"
    -"Browsers offer tools for viewing the DOM tree"
# READ 06
## Domain Modeling
    -OBJECT ORIENTED MODEL
    - Property/Data/Type
    - "When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors."
    - "Model its attributes with a constructor function that defines and initializes properties."
    - "Model its behaviors with small methods that focus on doing one job well."
    - "Create instances using the new keyword followed by a call to a constructor function."
    -"Store the newly created object in a variable so you can access its properties and methods from outside."
    - "Use the this variable within methods so you can access the object's properties and methods from inside."

## Jon Duckett HTML book:
### Chapter 6: “Tables” (pp.126-145)
#### SUMMARY
    -"the <table> element is used to add tables to a web page"
    - "a table is drawn out row by row. each row is created with the <tr> element"
    - "inside each row there are a number of cells represented by the <td> element (or<th> if it is a header"
    -"you can make cells of a table span more than one row or a column using the rowspan and colspan attributes."
    -"for long tables you can split the table into a <thead> <tbody> and <tfoot>"

## Jon Duckett JS Book
### Chapter 3: “Functions, Methods, and Objects” (pp.106-144)
#### SUMMARY: 
    - "functions allow you to group a set of related statements together that represent a single task."
    -"functions can take parameters(information required to do their job) and may return a value"
    -"an object is a series of variables and functions that represent something from the world around you"
    -"in an object variables are known as properties of the object; functions are known as methods of the object."
    -"web browsers implement objects that represent both the browser window and the document loaded into the browser window"
    -"javascript also has several built in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts"
    -"arrays and objects can be used to create complex data sets (and both can contain the other)"

# READ 08
## Jon Duckett HTML book:
### HTML/CSS book, Ch. 15, “Layout” (again; repeat of Class 4 reading)
### SUMMARY
    - "the new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure"
    - "The new elements provice clearer code (compared with using multiple <div> elements)"
    - "older browsers that do not understand HTML5 elements need to be told which elements are block-level elements"
    - "to make html5 elements work in internet explorer 8 (an older version of IE) extra javascript is needed which is available free from google"