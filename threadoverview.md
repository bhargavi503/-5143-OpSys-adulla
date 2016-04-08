Name:Adulla Bhargavi
Course: 5143 Operating Sysytems
Date: 07 April 2016
MustangID: M20227903

##Question 1

Explain the differences between Threads1 and Threads2 using lines from the code and a precise explanation?

Threads1.py
During the execution of thread1.py,the threads run independently without the need for accessing the same memory space at any point and it has the copy of the local variables. 
Threads2.py
During the execution of thread2.py it uses a global variable shared counter,which is accesed together at same point by both threads which results a complex situation.



##Question 2

After running Thread3.py does it fix the problems that occured in Threads2.py? What's the down-side?

Yes, when we run Threads3.py it fix the problems that occur in Threads2.py with the help of lock method.By using this lock method,one thread access 
the global variable and locks it accessing and another thread cannot acccess that variable until its work is done.Once the work is done it unlocks that variable.



##Question 3

Comment out the join statements at the bottom of the program and describe what happens?

If we have join in the program,first all the threads in that program are executed and then the main method is executed.
If we dont have the join method,it executes in any order.


##Question 4

What happens if you try to Ctrl-C out of the program before it terminates?

The threads keep executing, they donot stop running.

##Question 5

Read and run Threads4.py. This generates a different and more ridiculous race condition.
Write concise explanation of what's happening to cause this bizarre behavior using lines from the code and precise explanation?

In this scenerio, each thread tries to assign a value to the global variable. 
If any two threads try to access the same global variable at the same time, then that would result in the change of the contents accordingly.


##Question 6

Does uncommenting the lock operations clear up the problem in question 5?

If we have the lock operation in the program, any other thread cannot access the resources of the variable.
If we dont have that lock operation,the threads can access the resources of the particular variable independantly.

