![](../images/banner.jpg)

# Ponder 11 : Disk Scheduling Lab

##### Due Monday night at Midnight MST

Write a program to implement the disk scheduling algorithms discussed in the chapter. The first step in the coding projects is to write the code.

### A. Start with the provided code

Most of the code for this program is provided. You are only to implement the disk scheduling algorithms, not the user interface. The code is provided in the following location:

<pre>/home/cs345/week11/</pre>

Here you will find several files:

*   `makefile` : compile the files and create a TAR for submission and should not need to be changed.
*   `lab11.cpp` : defines `main()` and a few user interface functions and will not need to be changed.
*   `lab11.out` : an executable so you can see how it should work. This is mostly provided for testing purposes.
*   `ds.h` : defines the `DiskSchedulilngAlgorithm` base-class from which you will author the various derived classes. There is also the `ScheduleProblem` structure which contains all the information about the problem which was read from the file. This will not need to be changed.
*   `ds.cpp` : implements the interfaces for `DiskSchedulingtAlgorithm` and will not need to be changed.
*   `dsFCFS.h` : contains an implementation for the simplest disk scheduling algorithm. This code is provided. You might want to use it as a reference when implementing the rest of the other algorithms.
*   `dsSSTF.h` : a stub for the SSTF algorithm you will have to write.
*   `dsSCAN.h` : a stub for the SCAN algorithm you will have to write.
*   `dsC_SCAN.h` : a stub for the Circular-SCAN algorithm you will have to write.
*   `dsLOOK.h` : a stub for the LOOK algorithm you will have to write.
*   `dsC_LOOK.h` : a stub for the Circular-LOOK algorithm you will have to write.
*   `test1.txt` : one data-set used in textbook for Figure 9.4, 9.7, and 9.8.
*   `test2.txt` : another data-set used in textbook for Figure 9.5 and 9.5.
*   `test3.txt` : another data-set.
*   `test4.txt` : a complex data-set similar to what a real algorithm would be faced with.

Make sure you update the header in the makefile so it gets submitted to the correct location. The assignment this week will be called `Lab 11, Disk Scheduling Lab`

### B. Write the code

Implement five of the six scheduling algorithms as mentioned in the textbook (the first has been implemented as an example). These algorithms are:

*   **SSTF**: Shortest-Seek-Time-First found in section 9.4.2 SSTF Scheduling on page 448-449
*   **SCAN**: The elevator algorithm found in section 9.4.3 SCAN Scheduling on page 449-450
*   **C-SCAN**: Circular SCAN found in section 9.4.4 C_SCAN Scheduling on page 450
*   **LOOK**: The look-ahead variant of SCAN found in 9.4.5 LOOK Scheduling on page 451
*   **C-LOOK**: The circular variant of LOOK also found in 9.4.5 LOOK Scheduling on page 451

Note that all algorithms will have to implement the constructor, the `run()` method, and add at least one local variable. A few algorithms will need to also implement `computeDistance()`.

### C. Verify

The testBed for this assignment is:

<pre>testBed cs345/lab11 lab11.tar</pre>

Please make sure your program runs without error.

### D. Style

Your program should be well-commented and free of any style-checker errors.

## Submit

Please submit your TAR file using your Linux account.


### Assessment

Your grade for this activity will be according to the following rubric:

<table class="rubric">

<tbody>

<tr>

<th> </th>

<th>Exceptional  
100%</th>

<th>Good  
90%</th>

<th>Acceptable  
70%</th>

<th>Developing  
50%</th>

<th>Missing  
0%</th>

</tr>

<tr>

<th>Correct  
30%</th>

<td>No defects could be found</td>

<td>The code works as designed, including passing testBed</td>

<td>One test failed to pass on testBed or one glaring bug exists in the code</td>

<td>Elements of the solution exist</td>

<td>No attempt was made to solve the problem</td>

</tr>

<tr>

<th>Efficient  
20%</th>

<td>It is difficult to imagine how the code could be made more efficient</td>

<td>No obvious efficiency problems exist</td>

<td>One minor thing could be done to improve the efficiency of the code</td>

<td>Many obvious opportunities exist to increase performance</td>

<td>The code has horrible performance issues</td>

</tr>

<tr>

<th>Elegant  
10%</th>

<td>The most elegant solution imaginable was found</td>

<td>The code looks "professional"</td>

<td>One minor inelegancy was found</td>

<td>One obvious inelegancy remains in the code</td>

<td>The code was thrown together</td>

</tr>

<tr>

<th>Maintainable  
30%</th>

<td>The code lends itself to reuse and extension</td>

<td>The solution is well designed and thought out</td>

<td>One aspect of the solution design could be improved</td>

<td>Obvious maintainability problems exist</td>

<td>Support costs on this code would be much greater than necessary</td>

</tr>

<tr>

<th>Readable  
10%</th>

<td>"Anyone" could read and understand this code</td>

<td>The code honors all the style guidelines</td>

<td>One minor style error was found</td>

<td>One obvious style error was found</td>

<td>No obvious attention was spent on readability</td>

</tr>

</tbody>

</table>