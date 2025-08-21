<img width="692" height="471" alt="image" src="https://github.com/user-attachments/assets/60c9a368-c984-4942-bdf1-f909a4630d98" /># EXPERIMENT--01-ALP-FOR-8086
### Name : GANESH D

### Roll no: 212223240035

### Date of experiment : 18/07/2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
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

## Addition of 16 bit ALP (Immediate mode)
```
org 100

mov ax, 3521h     ; AX ? 3521h  (immediate)
add ax, 4612h     ; AX ? AX + 4612h (immediate)

ret
    
```



## Output  
<img width="950" height="950" alt="image" src="https://github.com/user-attachments/assets/5654c0a1-06ff-4e82-b043-e3db07df5229" />


 
## Subtraction of 16 bit numbers  ALP (Register mode)
```
org 100h

mov ax, 2561h   ; AX = 2561h
mov bx, 00F0h   ; BX = 00F0h
sub ax, bx      ; AX = AX - BX

hlt             ; stop execution

```

## Output  
<img width="950" height="950" alt="image" src="https://github.com/user-attachments/assets/21f90aea-e48c-4286-9f1a-a10d8f965fed" />


## Multiplication 16 bit alp (Direct memory mode)
```
org 100

NUM DW 3421h

MOV AX, 5D89h

MUL NUM       
ret  

```

## Output  
<img width="950" height="950" alt="image" src="https://github.com/user-attachments/assets/68dffd80-8e29-49c8-81df-c64843355716" />



## Division 16 bit alp (Register indirect mode)
```
NUM DW 6D87h    

MOV BX, OFFSET NUM
MOV AX, 3521h

DIV WORD PTR [BX]
ret  
```
## Output  
<img width="950" height="950" alt="image" src="https://github.com/user-attachments/assets/02084a17-bbe3-4f50-84ae-8be8e75f3165" />

## Programs for Logical  operations

## AND 16 bit opeartion(Register mode)

```
org 100h

mov ax, 2345h   ; AX = 2345h
mov bx, 1111h   ; BX = 1111h
and ax, bx      ; AX = AX AND BX

ret
```

## Output
<img width="950" height="950" alt="image" src="https://github.com/user-attachments/assets/043047b0-49f7-4a4f-812e-cbada6b09440" />

## OR 16 bit operation(Register mode)
```
org 100

mov ax,4d69h
mov bx,3521h

OR ax,bx
ret
```
## Output
<img width="950" height="950" alt="image" src="https://github.com/user-attachments/assets/a611590d-80bc-4405-a57d-979bcf4f03fe" />

## NOT 16 bit Operation(Register mode)

```
org 100
mov ax,6d79h

NOT ax
ret                 

```

## Output
<img width="691" height="472" alt="image" src="https://github.com/user-attachments/assets/c1efe02e-2410-4561-b3b8-b2095d151cdc" />

## XOR 16 bit Operation(Register mode)
## Result :

The execution of ALP on fundamental arithmetic operations is successfully completed.








