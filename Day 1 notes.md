
### Data Structure and Algorithm Essentials | Jan 2021 Batch 1 | Day 1 Overview
### DAY 01 
#### Algorithm
Time complexity
Asymptotic notation
Various time complexity
And, to understand in detail please go through the below TIMESTAMPS

https://www.youtube.com/watch?v=DqTryDAeR_Q

Day 1 | Jan 2021 Batch 1 | LetsUpgrade - Data Structure and Algorithm Essentials
 ---------------------------------------------------------------------------------------- 

TIMESTAMP for EACH TOPIC:  

------------------------------------------------------------------------------------------ 

2:00 - Introduction 

3:40 - What is letsupgrade 

4:24 - Learning pedagogy 

5:15 - Expectation in the program 

6:03 - How to attend the class 

7:01 - About goodies 

8:50 - About exam 

9:20 - Certificates 

12:25 - Community details 

16:00 - General question 

18:35 - Algorithm 

22:29 - Quiz 1 

28:35 - Time complexity 

30:10 -Asymptotic notation 

32:45 - Worst case time complexity 

34:54 - Graph explanation 

38:12 - Quiz 2 

42:45 - Various time complexity 

43:20 - Linear time complexity and constant time complexity 

46:36 - Quadratic time complexity 

47:05 - Logarithmic time complexity 

49:30 - Quadratic example 

53:15 - Quiz 3 

57:45 - Logarithmic example 

1:12:35 - Quiz 4 

1:16:59 - Example 

1:22:25 - Time complexity example 

1:23:47 - Assignment question

----------------------------------------------------------------------------------------------------------------------- 

 ### Algorithm:  
 A procedure to solve a mathematical problem in a finite number of steps that frequently  involves repetition of the operation. To solve a problem, two things to be taken in account to  select best algorithm. 

                    1. Time complexity      

                    2. Space complexity        

### Time complexity: 
         The Time complexity is the computational complexity that describes the amount of  computer time it takes to run an algorithm. Time complexity is commonly estimated by   counting the number of elementary operations performed by the algorithm, supposing   that each  elementary operation takes a fixed amount of time to perform. 

Asymptotic notation: 
          Asymptotic notations are used to represent the complexities of algorithms for asymptotic   analysis. These notations are mathematical tools to represent the complexities. 

          Five notations:     

                    1. Big O 

                    2. Big Omega 

                    3. Big Theta 

                    4. Small O  

                    5. Small Omega 

       Mostly Big O, Big Omega, Big Theta are used . Other two are for research purpose. 

Linear time complexity: 
         If the time taken depends on input , then it is called linear time complexity. It is referred as   O(n) . 

 #### Example: 
~~~
for(i=1;i<=n;i++) 
   printf("Letsupgrade"); 
~~~
Constant time complexity: 
           If a time taken by the line of code is known then it is called constant time complexity. It is denoted by O(c). 

#### Example: 
~~~
for(i=1;i<=100;i++) 
    printf("Letsupgrade"); 
~~~
Quadratic Time complexity: 

          If the time taken depends on the square of the input  then it is said to be quadratic  time complexity. It is denoted by O(n^2). 

 #### Example: 
~~~
for(i=1;i<=n;i++) 
   for(j=1;j<=n;j++) 
       printf("hi"); 
~~~
Logarithmic Time Complexity: 

         An algorithm is said to have a logarithmic time complexity when it reduces the size of input   data in each step. This indicates that the number of operations is not the same as the input size. The number of operations gets reduced as the input size increases. It is denoted  by O(logn). 

         ####  Example: 
~~~
for(i=1;i<=n;i*=2) 
   printf("hi"); 
~~~
