###SWBATs

####Loops
+ iterate over arrays using for loops and do while loops
+ iterate over arrays using loops

###Lesson Plan

####Loops
+ Let’s make a new array but use numbers now. Get an example set from a student and make an integer based array. <b>Ask a few review questions (add a number? index? etc…)</b>
+ Ok, what if we want to do something to each number. Like add one to each number. We could do it manually: numbers[0] = numbers[0] +1, etc. but that would take forever
+ A better way to do this is to set up a little machine with instructions on how to iterate (go through) every number in the array and do something specific to each one.
+ We do this in javascript with something called a for loop. Here is the syntax of what a for loop looks like:
for (starting condition; ending condition; step for moving our machine forward) {
  thing that we want to do each time we cycle through this loop
+ }
+ This might make a little more sense when you see this in action - with our number array. We want to add 1 to each number in our array and alert it to our screen. Here is how we would set that up:
+ numbers = [1,2,3,4,5]
+ for (var i=0; i<numbers.length; i++) {
    + alert(numbers[i]+1)
+ }
+ Let’s walk through each part of this.
  + for is the keyword that we use to set up a loop
  + inside of the parentheses is where we set up the conditions of our loop
  + we start off by declaring the starting conditions in the for loop should start with - a counter variable i set to 0. <b>Why do we set it at 0?</b> Because the first index in our array is 0 - so we want to set up our little machine to pull out each item in the array starting with the item at index 0.
  + <b>Why do we use the variable i?</b> It’s convention to use the variable i because i is short for index - we are counting through the indices of the of the array
  + we close this condition with a ; to indicate that we are done with these starting instructions for our machine and we’re ready to move on to 
  + in the next part of our for loop we set up the ending instructions for our machine - it’s like saying this machine should keep going until this condition is true
  + The condition here is that our var i must be less than numbers.length. <b>Why is this the ending condition for our machine? What is numbers.length equal to? Does numbers[5] exist?</b> No it doesn’t. We want to make sure we stop our machine before it starts requesting indices that don’t exist. Or in other words - keep going ONLY while i is less than the length of the array (5 in this case). 
  + The last condition of the for loop are instructions for how to keep our machine moving. Here we are saying - at the end of each iteration in the loop add one to var i. <b>What would happen if we didn’t have this condition set?</b> We wouldn’t get anywhere! We wouldn’t be iterating at all, because we would just keep trying to change numbers[0] over and over again in an infinite loop.
  + <b>Everyone create a iteration.js doc and try setting up a for loop with a numbers array and alert each number doubled.</b>
+ <b>Do you guys remember what we said yesterday about ALWAYS HAVING YOUR CODE WRAPPED UP IN FUNCTIONS? Everyone go into you iteration.js doc and wrap up your for loop in a function called doubleNumbers. Did you put your numbers array in your function? Is there a better way to do this?
+ What if we set up the function to accept a numbers array instead of hardcoding one specific array into the function? Why would that be better? Set up a new numbers array and call your doubleNumbers array with your new array.</b>
+ Let’s do one more practice lab with iteration and strings instead of numbers. 
  + Everyone create an array of your top 5 favorites movies.
  + Now create a function called myFavorites();
  + This function should take in an array of favorites and for each favorite it should alert to the screen something like “The Shawshank Redemption? That is my favorite too!”
+ Now create a new array of your favorite songs. Try calling the myFavorites() function with your favorite songs array.

