# 📌 Display Memory (Video Card Memory), Strings, Software Interrupts, Hardware Interrupts - 8086 Assembly


[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](#)
[![GitHub Forks](https://img.shields.io/github/forks/harismuneer/Graphical-Display-Memory-and-Software_Hardware-Interrupts-x86_Assembly.svg?style=social&label=Fork&maxAge=2592000)](https://www.github.com/harismuneer/Graphical-Display-Memory-and-Software_Hardware-Interrupts-x86_Assembly/fork)
[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Graphical-Display-Memory-and-Software_Hardware-Interrupts-x86_Assembly.svg?style=flat&label=Issues&maxAge=2592000)](https://www.github.com/harismuneer/Graphical-Display-Memory-and-Software_Hardware-Interrupts-x86_Assembly/issues)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat&label=Contributions&colorA=red&colorB=black	)](#)



I solved all these questions and shared the solutions here so that you can have a strong grip on these concepts with ready to run interesting solved problems.

## Book to Understand Concepts

[Assembly Language Programming by Belal Hashmi and Junaid Haroon](https://onlinebookpoint.blogspot.com/2016/10/assembly-language-programming-delivered.html)

Its an excellent book for understanding the language and concepts of 8086 Assembly. It starts from the very basics and then takes you to advanced concepts in an efficient manner. Highly Recommended!

## How to Run
1- Download this code and move the 'assembly_code' folder to C: directory.

2- Install DOSBOX from this link: [Download DOSBOX Emulator](https://www.dosbox.com/download.php?main=1)

3- After complete installation, go to DOSBOX installation directory and run "DOSBox 0.74 Options.bat". This will save you from the pain       of searching the configuration file yourself and will open that file for you.
Copy these lines at the end of that file:
```
mount c: c:\assembly_code 
```  
```
c:
```
4- Now to run any question (say named 'q1.asm'), run DOSBOX 0.74 and type
```
nasm q1.asm -o q1.com  
```
To run the code, type

```
q1.com
```

To examine step by step working of the code, type

```
afd q1.com
```


## Problems Solved

### Display Memory

* Q1. Write a program to make an asterisk travel the border of the screen, from upper left to upper right to lower right to lower left and back to upper left indefinitely.
* Q2. Write a subroutine “splitScreen” to reverse the screen i.e. left becomes right and right becomes left. Similarly top becomes bottom and bottom becomes top. You cannot use any temporary array. Only a word variable can be declared if needed.


### Strings + Display Memory

* Q3. Write a subroutine to copy a given area on the screen at the center of the screen without using a temporary array. The routine will be passed top, left, bottom, and right in that order through the stack. The parameters passed will always be within range the height will be odd and the width will be even so that it can be exactly centered. 

* Q4. Write a subroutine findSubstr that takes a null terminated string and a null terminated substring as its parameters and prints “Substring Found.” on video screen if that substring is found in that string and prints “Substring Not Found.” otherwise.

Sample : 
str: db ‘Marry has a little lamb.’,0
substr1: db ‘lamb’,0             ; findSubstr  prints “Substring Found.” for this substring.
Substr2: db ‘lame’,0            ; findSubstr  prints “Substring Not Found.” for this substring.

* Q5.  Write a subroutine “strcpy” that takes the address of two parameters via stack, the one pushed first is source and the second is the destination. The function should copy the source on the destination including the null character assuming that sufficient space is reserved starting at destination.

### Software Interrupts

* Q6. Write an assembly program that takes a 16 bit number as input from user and calculates whether the number is a happy number or unhappy. If the number is a happy number, display ‘Happy’ on the screen else display ‘UnHappy’. A happy number is defined by the following process: 

Starting with the given number, replace that number by the sum of the squares of its digits. Repeat the process on the replaced number until the number either equals 1 within 256 iterations of the process. The number for which this process ends in 1 within 256 iterations is called a happy number; otherwise it is called an unhappy number. Use ah =01 service of int 21h to take input from user and ah=09 service of int 21h to print string on the screen.

### Hardware Interrupts
* Q7. Write a TSR to calculate the current typing speed of the user. Current typing speed is the number of characters typed by the user in the last five seconds. The speed should be represented by printing asterisks at the right border (80th column) of the screen starting from the upper right to the lower right corner (growing downwards). Draw n asterisks if the user typed n characters in the last five seconds. The count should be updated every second.


-----------------------

## Author
You can get in touch with me on my LinkedIn Profile: [![LinkedIn Link](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=linkedin&longCache=true&style=social&label=Follow)](https://www.linkedin.com/in/harismuneer)

You can also follow my GitHub Profile to stay updated about my latest projects: [![GitHub Follow](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=Github&longCache=true&style=social&label=Follow)](https://github.com/harismuneer)

If you liked the repo then kindly support it by giving it a star ⭐ and share in your circles so more people can benefit from the effort.

## Sponsor
If you or your company use any of my projects or like what I’m doing then consider backing me.

- 🌟  **$9.99/month (recommended)** ❯ [Two cups of Caffè latte (coffee) every month](https://tinyurl.com/Haris-OSS-Coffee)
- 🚀  **$99.99 (one-time sponsor)** ❯ [Support an hour of open-source work](https://tinyurl.com/Haris-OSS-Platinum)
- 🔰  **$49.99 (one-time sponsor)** ❯ [Support an hour of maintenance](https://tinyurl.com/Haris-OSS-Gold)
- ☕️  **$9.99 (one-time sponsor)** ❯ [Lunch/coffee](https://tinyurl.com/Haris-OSS-Silver)

## Contributions Welcome
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](#)

If you find any bug in the code or have any improvements in mind then feel free to generate a pull request.

## Issues
[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Graphical-Display-Memory-and-Software_Hardware-Interrupts-x86_Assembly.svg?style=flat&label=Issues&maxAge=2592000)](https://www.github.com/harismuneer/Graphical-Display-Memory-and-Software_Hardware-Interrupts-x86_Assembly/issues)

If you face any issue, you can create a new issue in the Issues Tab and I will be glad to help you out.

## License
[![MIT](https://img.shields.io/cocoapods/l/AFNetworking.svg?style=style&label=License&maxAge=2592000)](../master/LICENSE)

Copyright (c) 2018-present, harismuneer                                                        
