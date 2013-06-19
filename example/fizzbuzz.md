Fizz Buzz
=========

A simple game for children to learn about division. Players take turns
counting outloud. If their number is divisible by 3, say "fizz". If the
number is divisible by 5, say "buzz". For numbers divisble by 3 *and* 
5 shout "fizz buzz!".

The problem also makes for a simple coding challenge. 

Let's define  a simple function called `fb` that handles an integer
`n`. We will simply count from `0 to n`. 

Note that any markdown embedded codeblocks are just blocks of text 
preceded by **4 spaces**. Running `lpjs` against this document 
will strip the markdown and leave the codeblocks intact.

-------

Define function fb

    var fb = function(n) {

Iterate from 0 to n

        for(var i=0; i < n; i++) {

Check divisibility and print

            if( i%3 == 0 && i%5 == 0) {
              console.log('fizz buzz!');
            } else if ( i%3 == 0) {
              console.log('fizz');
            } else if ( i%5 == 0) {
              console.log('buzz');
            } else {
              console.log(i);
            }
        }
    }        

Run a case for n = 100

    fb(100);
