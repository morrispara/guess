// Initialize Answer: generate random number btween 0 and 1, multiply by 1, convert to integer with round up
var Answer = Math.round(Math.random()*100);
// initialize Turns variable, set to 0
var Turns=0;
// initialize boolean variable Correct, set to value False).
var Correct=false;
// add one to value of variable turns
Turns++;
//keep looping until correct is set to true
while (Correct==false) {
    //initialize guess, set value to user input, telling user what to imput (give hint)
    var Guess = prompt("Guess my integer (between 0 and 100)!");
    // check if guess is equal to answer
    if (Guess == Answer) {
    //if equal, say "correct" and number of turns
        alert("CORRECT! You guessed it in "+Turns+" turns.");
        //set correct equal to true to get out of our "while loop"
        Correct = true;
    }
    //check if guess is equal to answer
    else if (Guess > Answer) {
    //give feedback, go lower
        alert("Hint: Try a lower number!");
    }
    //give feedback, go higher
    else if (Guess < Answer) {
        alert("Hint: Try a higher number!");
    }
    //add one to value of variable turns
    Turns++;
}
//end the game
alert("Thank you for playing.");
