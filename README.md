# EXPERIMENT--01-ALP-FOR-8086
### Name : SREE HARI K
### Roll no : 212223230212
### Date of experiment : 19.08.24





## Aim:
To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 
8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

### Addition  of 16 bit ALP 
~~~
org 100h
MOV AX,4554H;
MOV BX,3322H;
ADD AX,BX;
MOV [3000H],AX;
ret
~~~
### Output  
 ![Screenshot 2024-08-19 133725](https://github.com/user-attachments/assets/3fe55c10-4809-4216-a8c5-94f2010d9ce0)

### Subtraction of 16 bit numbers  ALP 
~~~
org 100h 
MOV AX,768BH;
MOV BX,38FFH;
SUB AX,BX;
MOV [2000H],AX;
ret
~~~
### Output  
![Screenshot 2024-08-19 134308](https://github.com/user-attachments/assets/54c0a349-971a-4910-b33d-29d8ee6c2216)

### Multiplication alp 
~~~
org 100h
MOV AX,[2000H];
MOV BX,[3000H];
MUL BX; 
MOV [4000H],AX;
ret
~~~
 ###  Output  
![Screenshot 2024-08-19 135014](https://github.com/user-attachments/assets/f90b3027-7c2c-4054-85ad-c15fff02a366)


### Division alp 
~~~
org 100h
MOV AL,44H;
MOV BL,02H
DIV BL;
MOV [5000H],AL;
ret
~~~

### Output  
![Screenshot 2024-08-19 135830](https://github.com/user-attachments/assets/3f787889-13d4-4c3a-a2af-431c4cbf12d7)

## Programs for logical  operations
### OR operation alp
~~~
org 100h
MOV SI,0532H;
MOV AX,0A32H;
MOV BX,0B13H;
OR AX,BX;
ret
~~~
### Output
![Screenshot 2024-08-20 052903](https://github.com/user-attachments/assets/33c2c619-0fb7-47dd-a63e-cb1a95abca86)

### AND operation alp
~~~
org 100h
MOV AX,2255H;
MOV BX,1133h;
AND AX,BX;
MOV [SI],AX;
ret
~~~
### Output
![Screenshot 2024-08-19 142608](https://github.com/user-attachments/assets/46739ffd-d150-4049-84cb-9d064296e8ae)

### XOR operation alp
~~~
org 100h
MOV AX,3223H;
MOV BX,3322H;
XOR AX,BX;
MOV [SI+2],AX;
ret
~~~
### Output
![Screenshot 2024-08-19 142832](https://github.com/user-attachments/assets/aadedde0-ec30-4546-a2fb-8dc2e043facc)

### NOT operation alp
~~~
org 100h
MOV [SI+2],AX;
MOV AX,4554H;
NOT AX;
MOV [SI+8],AX;
ret
~~~
### Output
![Screenshot 2024-08-19 142720](https://github.com/user-attachments/assets/d2572530-0b6b-49f3-bd12-99947cd772f2)

## Result :
Thus the ALP on the fundamental Arithmetic and Logical operations has been written and executed successfully.
