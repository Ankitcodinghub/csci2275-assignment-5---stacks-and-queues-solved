# csci2275-assignment-5---stacks-and-queues-solved
**TO GET THIS SOLUTION VISIT:** [CSCI2275 Assignment 5 – Stacks and Queues Solved](https://www.ankitcodinghub.com/product/csci2275-csci-2270-ae-data-structures-assignment-5-stacks-and-queues-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119708&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI2275  Assignment 5 - Stacks and Queues Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Objectives

1. Create, add to, delete from, and work with a stack implemented as a linked list

2. Create, add to, delete from, and work with a queue implemented as an array

Instructions

Write code to complete Parts 1 and 2. Implement the solution for each part as a separate program. To receive credit for your code, you will need to pass the necessary test cases. Use the following steps to test your code as you work on the assignment:

1. Open up your Linux terminal, navigate to the build directory of this assignment (e.g. cd build).

2. Run the cmake .. command.

3. Run the make command.

4. If there are no compilation errors, three executables will be generated within the build directory: run_app_1, run_app_2, and run_tests.

5. If you would like to run your program including your app implementation in the main function, execute run_app_1 from the terminal by typing ./run_app_1. Similarly, you can execute run_app_2.

6. While executing the run_app_2 you need to pass the initial queue size using command line, so the command to execute is ./run_app_2 &lt;queue_size&gt;.

7. To run the grading tests, execute run_tests from the terminal by typing ./run_tests.

Overview

Stacks and Queues are both data structures that can be implemented using either an array or a linked list. You will gain practice with each of these in the following two programs. The first is to build a word decoder using a linked list stack and the second is to simulate a course registration waitlist system using a circular array based queue.

Word decoder – Part-1

Sherlock and Watson are working on a new case. Suddenly, Sherlock gets an encoded text from Moriarity. He figures out that he needs to reverse all the strings enclosed by parenthesis to get a meaningful word. He needs help from you to do this. We know that stacks are great for reversing strings and parsing nested structures.

Your task will be to implement the stack using a linked list and an accompanying driver file to test your implementation.

How to Evaluate

The input will be nested sentences which are separated by closing and opening square brackets. We will evaluate sentences by pushing each word onto a stack until we encounter a â€œ)â€ bracket. After we get a â€œ)â€ bracket we subsequently pop from the stack until we get the first â€œ(â€œ. After this we again, push the letters the were popped in reverse order.

Class Specifications

The node structure for the linked list is defined in WordDecoder.hpp. We have a struct Letter as they represent letters in a word.

“` struct Letter { string Letter; // the string to store Letter* next; // the pointer to the next node };

“`

The WordDecoder class definition is provided in the file WordDecoder.hpp in Canvas. Do not modify this file or your code wonâ€™t work! Fill in the file WordDecoder.cpp according to the following specifications.

Letter* stackHead; + Points to the top of the stack

WordDecoder(); + Class constructor; set the stackHead pointer to NULL

~WordDecoder(); + Destroy the stack. Take special care not to leave any memory leaks

bool isEmpty(); + Returns true if the stack is empty void push(string letter); + Push a letter to the stack

void pop(); + Pop the element out of the stack. Do not leave any memory leak. Print Stack empty, cannot pop a letter. if the stack is empty.

Letter* peek(); + Returns the top of the stack. Print Stack empty, cannot peek. if the stack is empty.

Letter* getStackHead() { return stackHead; } + Returns the stackHead. This is already implemented.

void evaluate(std::string* s, int size); + This function will accept an array of strings and the length of the array. This function will evaluate the encoded word and print the final decoded word after performing the stack operations described above. E.g. The decoded word: zyx Instructions for the main_1.cpp file

The driver code should start with printing Enter the encoded word separated by ‘(‘ and ‘)’. Print #&gt;. Then accept the encoded string from user.

If the string array is empty print Nothing to evaluate Otherwise call the evaluate function with the string array. Free any unused memory

Order of function implementation

1. Constructor

2. isEmpty

3. push

4. pop

5. peek

6. evaluate

7. Destructor

8. main

Example Runs:

1.

“` Enter the encoded word separated by ‘(‘ and ‘)’.

&gt; (xyz)

The decoded word: zyx “`

2.

“` Enter the encoded word separated by ‘(‘ and ‘)’.

&gt; ((od)og)

The decoded word: good “`

3.

“` Enter the encoded word separated by ‘(‘ and ‘)’.

&gt; (ni(su(ats)))

The decoded word: sustain “`

WaitlistQueue Class

NOTE: Beware of edge cases that arise from the array being circular

In this class, you will build a queue using the circular array implementation to emulate a simple course registration waitlist. Implement the methods of WaitlistQueue according to the following specifications. string queue + A dynamically allocated array of strings to act as a container for the circular queue.

int qCapacity + The total capacity of the dynamically allocated array, queue. This value will be passed in a parameterized constructor as an argument.

int qFront + Index in the array that keeps track of the index at which dequeue will happen next, i.e., it refers to the front (or first) element in the queue. int qEnd + Index in the array that keeps track of the tail element in the queue.

WaitlistQueue(int qSize=5) + Constructor. Initialized qFront, qEnd to -1 and qCapacity to qSize. It’s already implemented for you, don’t change.

~WaitlistQueue() + Destructor. Deallocate the memory for the queue container.

void enqueue(string value) + If the queue is not full, then add the value to the end of the queue and modify qFront and/or qEnd appropriately, else print Waitlist is full. Cannot enqueue.

void dequeue() + Remove the first element from the queue if the queue is not empty and modify qFront and/or qEnd appropriately. Otherwise, print Waitlist is empty. Cannot dequeue. + Take care of the edge case where there is only 1 element in the queue to be dequeued. In such a case, you should appropriately reset qFront and qEnd.

string peek() + If the queue is empty then return &lt;EMPTY QUEUE&gt;. Otherwise, return the first element in the queue.

void resize(int newSize) + Resize the queue container to this newSize (&gt;= 1). You must start at the front of the original queue and copy elements till the end of the original queue, or until the new queue is full. + You must update queue, qFront, qEnd and qCapacity appropriately. Take care of any possible memory leaks.

int size() + Return the number of active elements in the queue. Not to be confused with qCapacity. int capacity() + Return the capacity of the queue container, i.e., qCapacity.

bool isEmpty() + Return true if the queue is empty, false otherwise bool isFull() + Return true if the queue is full, false otherwise

Instructions for the main_2.cpp file

Your program will start by creating a queue, pass the size of the queue as the first argument from command line and then display a menu by calling the menu() function which is included in the provided skeleton code. The user will select an option from the menu to decide upon what the program will do, after which the menu will be displayed again. Below are the specifics of the menu (Tips: We recommend using the stream extraction operator(&gt;&gt;) rather than the getline() method to get input.)

Option 1: Enqueue

Request the user for the value to be enqueued using the below print statement

cout &lt;&lt; “Enter the value to add into queue:” &lt;&lt; endl;

Call the enqueue() method on the value given by user.

Option 2: Dequeue

Simply call the dequeue() method.

Option 3: Peek

Simply print the output of the peek() method.

Option 4: Resize + Request the user for the new size of the queue using the below print statement cout &lt;&lt; “Enter the new capacity:”

&lt;&lt; endl; + Call the resize() function after printing the following message “Resizing from &lt;old_capacity&gt; to &lt;new_capacity&gt;”

Option 5: Quit + Print the following message cout &lt;&lt; “Quitting…” &lt;&lt; endl; + Prior to exiting the program, print the queue from front to back. Example: Contents of the queue: buff01 buff02 buff03 + Print “Goodbye!” and exit the program.

If user selects options other than 1 to 5, print the following statement cout &lt;&lt; “Invalid choice. Please enter a number between 1 and 5.” &lt;&lt; endl;

Below is a sample output

*—————————————-* Choose an option: 1. Enqueue 2. Dequeue 3. Peek 4. Resize 5. Quit

*—————————————-* 1 Enter the value to add into queue:course1 *———————-

——————* Choose an option: 1. Enqueue 2. Dequeue 3. Peek 4. Resize 5. Quit *———————–

—————–* 1 Enter the value to add into queue:course2 *—————————————-*

Choose an option: 1. Enqueue 2. Dequeue 3. Peek 4. Resize 5. Quit *—————————————-* 1

Enter the value to add into queue:course3 *—————————————-* Choose an option: 1.

Enqueue 2. Dequeue 3. Peek 4. Resize 5. Quit *—————————————-* 2 *——————-

———————* Choose an option: 1. Enqueue 2. Dequeue 3. Peek 4. Resize 5. Quit *——————–

——————–* 3 course3 *—————————————-* Choose an option: 1. Enqueue 2. Dequeue 3. Peek 4. Resize 5. Quit *—————————————-* 5 Quitting… Contents of the queue: course2 course3 Goodbye!

Order of function implementation

1. Constructor

2. size

3. capacity

4. isEmpty

5. isFull

6. enqueue

7. dequeue

8. peek

9. resize

10. main
