> [!imp]
> **Js is the synchronous and singel threaded language **

Two components 
- Meomory (variable enviroment)
- Code (Therad of Execution)
![](at/Pasted%20image%2020241224152815.png)
1st phase is the memory creation phase  
-  all the varables and functions are stored in the MemoryPart (variable enviroment)
![](Pasted%20image%2020241224152854.png)
![](at/Pasted%20image%2020241224152747.png)
This code' Memory context will look like below 

In this you can see that 
	n = 2 
	square all the fn's got alloted to them also complete conde is wrtten in the square 
	square2 and square4 is not defined cause their value is not there 
when invoking the fuction `square` then a whole new execution context is created for that function 
	Here is the picture of that. 
![](at/Pasted%20image%2020241224152831.png)
The final execution will look like this 
	both the fn's were solved in the code execution part an then return the value 
	1st two context are deleted when they return their values 

and in the final complete global context is deleted 

## CallStack 
All these things(like heriechal storage of execution context ) handled by the call stack which is a stack
![](at/Pasted%20image%2020241224153055.png)

First the e1 is solved and then after that e1 is popped out and then the gec is used come in control 

> [!Imp]
> 
>** Callstack maintain the order of execution of executions context's **
