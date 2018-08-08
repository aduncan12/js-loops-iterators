# Robot Booking
We're going to build a basic bot that will allow a user to book a table and order food. The focus is NOT on the UI; the focus is on the underlying logic, using loops, conditionals and variables.

0. Start by discussing in groups what this system could do, and share with the class.
0. Then define the inputs for your program as a series of variables.
    ```javascript

    var name = "Jeremiah";
    var lastUserName = "Jeremiah";
    var tableFor = 5;
    ```
0. Next, work out what the outputs should be; for example, what should happen if the user asks for a table for five people. You should do this in the form of psuedocode, using comments.

    ```javascript
    //if the user's name is same as last time welcome them back
    //else welcome them for the first time
    
    //ask them how many they want a table for
    //if the number if greater than 0 but less than the restaurant capacity then continue to ask them what they want to eat
    //else apologise and offer them a discount next time
    ```
    
0. Finally, you should write the conditional logic and use console.logs to output it.

    ```
    javascript
    //if the user's name is same as last time welcome them back
    if ( name === lastUserName ) {
        console.log("welcome back " + name);
    }
    ``` 
    
Get a basic system working first, then add further complexity to make your system more comprehensive and human-like. 


    var name = "Alan";
    var lastUserName = "Alan";
    var time = 1930;
    var tableFor = 6;
    var availableSeats = 5;

    //if the user's name is same as last time welcome them back
    if(name === lastUserName) {
        console.log("Welcome back, " + lastUserName +"!");
    //else welcome them for the first time
    } else {
        console.log("Welcome to restaurant, " + name +"!");
    }

        //ask user when they would like a table
    if(time > 2100) {
        console.log("Sorry, we're closed. Please choose an earlier time or come back tomorrow");
    //ask them how many they want a table for
    } else {
        console.log("Great! How many seats do you need?");
    }

    //check available seats for that time
    //if requested # of seats available, confirm booking
    if(tableFor < availableSeats) {
        console.log("Your table is reserved! See you then!")
    //else apologise and suggest a different time
    } else {
        console.log("We're sorry, there are no seats available. Please select another time");
    }