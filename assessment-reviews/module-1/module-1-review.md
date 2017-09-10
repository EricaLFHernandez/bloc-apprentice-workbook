# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for?  
  Hyper Text Markup Language. It's used to create the structural elements of a webpage.
2. What is the difference between an ID and a class?  
  IDs are used to set the style of one specific element. Classes are used to set the style of many elements.
3. What does it mean to write "semantic" HTML?  
  Semantic HTML uses elements that describe the content of the elements as often as possible.

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".  
  `<p class="highlight">Watch out!</p>`
2. Write an HTML image tag to show an image called `profile-picture.jpg`.  
  `<img src="/profile-picture.jpg">`
3. Write a link tag that links to http://google.com.  
  `<a href="http://google.com>Google</a>`
5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
  ```html
  <!DOCTYPE html>
  <html>
  <head>
    <meta charset="utf-8">
    <script src="/main.js"></script>
    <link rel="stylesheet" src="main.css">
  </head>
  <body>
  </body>
  </html>
  ```
6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.
7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
8. Write a numbered list in HTML and list three of your favorite books.
  ```html
  <ol>
    <li>Meditations</li>
    <li>Y: The Last Man</li>
    <li>Masters of Doom</li>
  </ol>
  ```
9. Fix the indentation of the following HTML sample:

  ```html
  <div>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?  
  Cascading Style Sheets. CSS is used to style HTML.
2. What is the CSS box model?  
  The CSS box model is used to set the margins, border, and padding surrounding HTML content.
3. What's the difference between margin and padding?  
  A margin adds space outside of the border. Padding adds space between the content and the border.

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.
  ```css
  h1 {
    color: red;
  }
  ```
2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```
  
  ```css
    .btn {
      background-color: blue;
    }
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.

  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```
  ```css
  header p {
    font-size: 20 px;
  }
  ```

## JavaScript

### Questions

1. What is a function? What are they used for?
  
2. What is the difference between `==` and `===`?
3. What is the difference between global and local scope variables?
4. What is a boolean value?
5. What is an array?

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.   
`var myName = "Erica Hernandez";`
2. Write a loop that logs the numbers 1 through 10 to the console.  
```js
for (var i = 1; i <= 10; i++) {
  console.log(i);
}
```
3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".
```js
if (score > 5 && lives > 0) {
  alert("You win!");
}
```
4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
```js
function sayHello(name) {
console.log("Hello, " + name + "!");
}

sayHello("Erica");
```
5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```
  
`"Friday, Friday"`

6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```
  `10`

7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```
  `"Hello Sarah ! Goodbye Sarah !"`

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.
  http://jsbin.com/momahaqubu/edit?js,console
9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.
  http://jsbin.com/joyivin/edit?js,console
10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
  http://jsbin.com/kuhenir/edit?js,console
11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```
  `pet.speak();`

12. Using the same script as above, write the correct line to log the dog's name to the console.  
`console.log(pet.name);`

## Command Line

### Questions

1. What is the command line and what is it used for?
2. What does the command `ls` do?
3. What does the command `pwd` do?
4. What does the following command do: `cd my-cool-project`

### Exercises

1. Write the command to make a new directory called "my-cool-project".
2. Write the command to create a file called "index.html".
3. Write the command to delete a file called "main.css".

## Git

### Questions

1. What is Git and what is it used for?
2. What's the difference between a local repository and a remote repository?

### Exercises

1. Write the command that you would use to create a new local Git repository.
2. Write the command to stage a file called `index.html` to be committed.
3. Write the command to view the current status of the git repository.
