java cSchool of Computer Science and Electronic Engineering
1
CE243 (NWU) Assignment 2 (2020-2021) 
1. Objectives 
The objective of this assignment is to demonstrate your understanding of the embedded 
system that can be effectively controlled using C language and ARM mbed you have learnt in 
this module. 
2. The task 
To design and write a C program to implement a guessing game on the ARM mbed 
development kit provided in the lab. Your design should include the following main features. 
- The main body of the guessing game logic should be implemented on the ARM mbed 
development kit. 
- Develop a PC host program in C that can communicate with the game on the ARM 
mbed via UART interface. The messages of the game should be displayed on the host 
program. 
- Use the peripherals on the mbed extension board to give better user experience, e.g. 
LCD, keypad, etc. 
- Your game should be error free and have error checking function to avoid any crash 
caused by invalid user input or similar bugs. 
Game: The finished game will provide a user experience that looks something like this: 
What is your guess? 5 
You are way off. 
What is your guess? 8 
You are way off. 
What is your guess? 3 
You are less than 3 away! 
What is your guess? 4 
You are less than 3 away! 
What is your guess? 2 
You guessed correctly! 
The guessing number should be set by the user when the mbed is initialised. Please consider 
suitable user experience here to make that happen smoothly. The number should be set 
between 0-30. 
User input 
The game will need to get guesses from the user on the PC host. Your programme 
always ask the user “What is your guess?”, and you should use an infinite loop to 
ask the user for a guess. After it is entered, print out each guess. A session might 
look like this: 
What is your guess? 2 
2 
Note: there is a fixed number of guesses, determined by the user. In the real game, 
the loop will finish once the number has been guessed correctly. 
Check proximity 
School of Computer Science and Electronic Engineering
The game will give the user a hint when a guess is close to the correct answer. In 
other words, with each guess the game has to determine the proximity of the guess to 
the randomly generated correct number. Write a function within(value, goal, n) that 
return 1 if value is within n distance of goal. For example, within(2, 5, 2) would 
return 0 but within(4, 5, 2) would return 0. 
Scoring 
One can think of a “score” in this game as the number of guesses made before 
getting the number right; a lower score is better. Once the user has guessed the 
number, print a line saying how many guesses were made (something like “Your 
score is 4”). 
LCD: The first row of the LCD should always show the secret number you set, and the 
second row of the LCD should show the current user guess. Once the user has the 
guessed number, the second row of LCD should show a message indicating the 
completion of the game and the final score of the user. 
Keypad: The keypad should be used to set the secret number. 
3. Deadline and submission requirements
The deadline for the electric submission of your Assignment 2 report and associated C 
programs is 11:59:59 on Friday 1 Nov. 2019. Please email your assignment as ONE 
attachment to ce243assignment@163.com prior to the above submission deadline. Please 
merge everything listed below into one .doc or .pdf file and submit. The filename shall take
the following format: Surname_Firstname_RegistrationNumber_A2, all in Eng代 写CE243、C/C++
代做程序编程语言lish. Your 
email subject shall use exactly the same format. No email content is necessary. In the 
meanwhile please ALSO upload the same file to FASER. 
 Your assignment shall be written in such a way that it is clear, concise and easy to read. 
 Write your name (both English and Chinese), registration number and module code 
(CE243-NWU) clearly on the cover page, including a ToC (Table of Contents) (1 page). 
 You shall use a flow chart to outline your software design and use text to explain how it 
works (2 or 3 pages). 
 You should run your code for testing different scenarios. The results of testing should be 
presented in the report and explain how you fix it if any bugs have been found. (2 or 3 
pages). 
 Your C program should be printed at the end of the report (3 or 4 pages). 
No extensions of the deadlines will be given. If, for any reason, you do not submit your code, 
there will be no record of the submission time and you will automatically get a zero mark. 
You shall submit your work through the proper channel (electronic submission) and on time, 
even if it is incomplete - something is better than nothing. 
This assignment is to be completed individually, i.e. whatever you hand in must be your own 
individual work. Any software or any other materials that you use in this assignment, whether 
previously published or not, must be referred and properly acknowledged. 
4. Assessment 
You will be assessed on the source code you submit and the performance of your code. 
(i) Marks will be awarded for programming style and the number of features implemented. 
2
School of Computer Science and Electronic Engineering
(ii) You are expected to show the performance of the programs during demonstration in the 
10th lab (Week 11). The demonstration session is mandatory to this assignment, and it is 
worth 50% of the overall mark of this assignment. 
(iii)You are expected to answer some questions about the main aspects of your work during 
your demonstration. 
(iv)More specifically, your Assignment 2 will be assessed as follows: 
Excellent (70 - 100%) 
All features have been implemented. The program is well-structured and commented. 
Your game is well functioned and playable during your demonstration. All questions 
are answered correctly. The report is well written and structured, and only contains 
minor mistakes and all requirements for the report are met. 
Good (55 - 69%) 
The program implements all of the required features, but has not well structured and 
commented. Your game is functional and reasonable playable your demonstration. 
Not all questions are answered correctly. The report is written reasonable well, but it 
contains some mistakes and/or few requirements are not met. The report was good 
structured, and it has many mistakes, but the overall requirement are mostly met. 
Poor (40 - 54%) 
The program implements less than 50% of the required features, but has poor 
structure and comments. Your game is not functioned well and barely playable during 
your demonstration. Most of the questions are not answered correctly. The report was 
poorly structured, and it has many mistakes, but the overall requirement are mostly 
met. 
Awful (0 – 39%) 
The program does not work. It has poor structure and comments. Your game is not 
functioning at all during your demonstration. No question is answered correctly. The 
report was poorly structured, and it contains many fundamental mistakes, the overall 
requirements are not met. 
3

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
