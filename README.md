# Advanced-JavaScript-Constructor-Word-Guess
Instructions

The completed game should meet the following criteria:


The completed game should be able to receive user input using the inquirer or prompt npm packages.
Your solution should have, at minimum, three files:
 Index
 Letters.js
 Words.js

function Letter(letter) = {
var prompt = function (
    prompt();
)
var this.characterArray = [];
var this.guessed = false;
var this.process = function (letter){
    push letter to an array
    if (this.letter = resul ......)
    }
 }

function prompt() {
    prompt.get(['guess'], function (err, result) {
        // Log the results. 
        console.log('Command-line input received:');
        console.log('  guess   : ' + result.guess);
    
        //this var is reassigned to make it more workable
        var guess = result.guess;

    var
    return
}
 



Letter.js: Contains a constructor, Letter. This constructor should be able to either display an underlying character or a blank placeholder (such as an underscore), depending on whether or not the user has guessed the letter. That means the constructor should define:


A string value to store the underlying character for the letter
A boolean value that stores whether that letter has been guessed yet
A function that returns the underlying character if the letter has been guessed, or a placeholder (like an underscore) if the letter has not been guessed
A function that takes a character as an argument and checks it against the underlying character, updating the stored boolean value to true if it was guessed correctly

each letter is an object with the 4 values above.


Word.js: Contains a constructor, Word that depends on the Letter constructor. This is used to create an object representing the current word the user is attempting to guess. That means the constructor should define:


An array of new Letter objects representing the letters of the underlying word
A function that returns a string representing the word. This should call the function on each letter object (the first function defined in Letter.js) that displays the character or an underscore and concatenate those together.
A function that takes a character as an argument and calls the guess function on each letter object (the second function defined in Letter.js)



index.js: The file containing the logic for the course of the game, which depends on Word.js and:


Randomly selects a word and uses the Word constructor to store it
Prompts the user for each guess and keeps track of the user's remaining guesses





Letter.js should not require any other files.
Word.js should only require Letter.js
HINT: Write Letter.js first and test it on its own before moving on, then do the same thing with Word.js
HINT: If you name your letter's display function toString, JavaScript will call that function automatically whenever casting that object to a string (check out this example: https://jsbin.com/facawetume/edit?js,console)





Notes


Since this assignment is a command-line application, you don't need to deploy it anywhere. You will, however, be required to upload it to Github.
Remember to include a package.json file containing your project dependencies in your Github repo!



Minimum Requirements

Attempt to complete homework assignment as described in instructions. If unable to complete certain portions, please pseudocode these portions to describe what remains to be completed. Adding a README.md as well as adding this homework to your portfolio are required as well and more information can be found below.

