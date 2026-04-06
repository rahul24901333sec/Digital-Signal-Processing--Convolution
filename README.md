# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM:
```
clc;% clear screen
clear all;%clear screen
close all;%close all figure windows

%input sequence
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;

figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;

figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution
z=conv2(x,y);
nl=a+b:1:length(z)+a+b-1;

figure(3);
stem(nl,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
<img width="674" height="618" alt="image" src="https://github.com/user-attachments/assets/22d6c95f-ce68-4ee7-802d-0bc7d9c95774" />
<img width="627" height="593" alt="image" src="https://github.com/user-attachments/assets/0d789ac7-1433-4f2f-b097-01c8c7ef6605" />
<img width="649" height="604" alt="image" src="https://github.com/user-attachments/assets/c753c61a-c966-4492-8715-0c000262ed48" />

## RESULT:
<img width="720" height="1280" alt="image" src="https://github.com/user-attachments/assets/99db2aed-f86a-4ded-b809-b44576bc6b26" />


