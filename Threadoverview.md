Name:Manjusri Daita
Course:5143 Operating Systems
Date :08  April 2016
Mustang ID:M20227907

## Question 1

Difference between Threads1.py and Threads2.py
Threads1.py are the threads which run independently without any need to access the same memory space during their execution, here Threads2.py uses global variables where both threads try to access at the same time at some point during execution which results in race condition.

##Question 2

After running Thread3.py does it fix the problems that occured in Threads2.py? What's the down-side?
Yes, the code Threads3.py will fix the race condition in Threads2.py by using the lock method, here the threads are ready to access the global variable, the thread locks this access so that no other thread has access to the variable till the process ends and  aqfter that it unlocks the variable.

##Question 3

Describe what happens after commenting out Join.
Here in this program if we add join then the threads execute first and then the main program is executed next.So when we remove join there is no particular order for the program to execute .

##Question 4

What happens if you try to Ctrl-C out of the program before it terminates?
Here program doesn't stop running but the threads keep on executing.

##Question 5

This generates a different and more ridiculous race condition. Write concise explanation of what's happening to cause this bizarre behavior using lines from the code and precise explanation.?
Threads try to assign a value to the global variable, based on this value if loop will be executed or not is decided.When threads tries to access global variables they make change to the content and when another thread comes to access these varibles since content is changed confusion is occured or abnormality is observed this is called as bizarre

##Question 6

Does uncommenting the lock operations clear up the problem in question 5
Yes if we add lock operation other threads cannot access the variables otherwise at any point of time these variables can be accessed by other threads
