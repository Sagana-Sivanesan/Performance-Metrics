# Performance-Calculator
A user-interactive project to gain knowledge in computer architecture in response to measuring performance metrics. The performance calculator takes in user inputs and calculates the appropriate Clock Rate or CPU Execution Time. The focus of this performance calculator is to understand the functionality of a program with optimum performance and to study Clock Rate and CPU Executions Time. C programming language and Sublime Text text editor was used for the completion of this project.
## Background Information
The study of computer organization and design enhances the quality of a programmers' code writing skills that results in a program with the best performance. What defines the best performance? As programmers or a regular computer user, we value the importance of reducing response time. Response Time is defined as the time between the start and completion of a task. The components of performance: Number of Instructions, CPU Execution Time, Clock Cycles per Instruction (CPI), and Clock Cycle Time. A Clock Cycle determines the CPU (The speed of a processor). CPI is the average amount of clock cycles per instruction for a program. The Execution Time is the actual time the CPU spends computing for a specific task. Therefore, by increasing the performance the execution time is decreasing. In this assignment, we use our understanding of hardware terminology to calculate the Clock Rate and CPU Execution Time user inputs.

Clock Rate Formula:
Clock Rate (Hertz) = 1/Duration of 1 Clock Cycle (Seconds)

CPU Execution Time Formula:
CPU Execution Time (Seconds) = Instructions/Program * Clock Cycles/Instruction * Seconds/Clock Cycle
## Getting Started
The following variables were declared and initialized:
    
    #include <stdio.h>

     int main( int argc, char** argv ) {
       int num;
       float time;
       int instruction, clockCycles;
       float clockRate;
       float cpu;
The user is prompted to select 1 (Clock Rate) or 2 (CPU Time):

      printf("Please select the computation you want to make: (1 = clock rate, 2 = CPU time): ");
      scanf("%i", &num);
      
The Clock Rate or CPU Time is calculated and the output is printed:

      if (num == 1) {
        printf("You selected clock rate, please enter the duration of one clock cycle in seconds: ");
        scanf("%f", &t);
        clockRate = 1/t;
        printf("The clock rate corresponding to this duration is: %.1f Hertz.", clockRate);
      } else {
        if (num == 2) {
          printf("You selected CPU time, please enter the duration of one clock cycle in seconds: ");
          scanf("%f", &t);
          printf("You selected CPU time, please enter the number of instructions in the program: ");
          scanf("%i", &i);
          printf("You selected CPU time, please enter the number of clock cycles per instruction: ");
          scanf("%i", &c);
          cpu = t*i*c;

	printf("The CPU execution time corresponding to these parameters is: %.1f seconds.", cpu);
     }
     }
     }
## Skills
* Presented my knowledge in computer archtecture
* Fluency in C, Submlime Text
* Proper code writing style and syntax
* Expressed the importance of studying computer organization and design to write efficient programs
