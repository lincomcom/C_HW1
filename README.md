C_HW1
=====

This is a 3-part assignment.  Preparation: •	create a directory named hw1 •	
for each part, create a subdirectory such as part1, part2, part3 etc. •	
put your .c files into the directory (named part1.c, part2.c, part3.c etc) Checklist for source files •	
include /* */-style comments in your .c files. You need to say o	the file name, assignment number (#1), 
due date, your name, your student ID o	describe what the program does (in English), o	
state the status of the program. does it work? what works and what doesn't work? what do you think may be the problem? •	
include a typescript to show how you compile and test each program. % script Script started, 
output file is typescript % cc myfile.c % ./a.out ... % exit Script done, output file is typescript % _ •	
Turn in ONE single .tgz (tar-gzipped) file including all parts of your hw1 directory. o	
Go to the directory that contains the hw1 directory (so that when you ls, it shows hw1)  % tar czf hw1.tgz hw1 o	
If you want to make sure your .tgz file is created properly, you can do  % tar tzf hw1.tgz to list the content of the tgz file. o	
Optionally, you can extract the content of your .tgz file by putting it in a temporary directory, and then try  % tar xzf hw1.tgz . 
It should create a hw1 directory with the same content as the original. o	
your .tgz file should contain your .c source file and the typescript for each part. •	To copy the file from the instructional server back to your own computer, log out first, and then type % scp username@cs25.cs.nthu.edu.tw:hw1.tgz . •	You need to type the command exactly.  There is a space and a dot (.) after the hw1.tgz file above! 
________________________________________ 
Part 1: 
Write a C program to print out the ASCII table use a single printf statement for the printable set of characters (32 to 126). 
The output can print all entries on the same line.  % cc part1.c % ./a.out 
32 ' ' 33 '!' 34 '"' 35 '#' 36 '$' 37 '%' 38 '&amp;' 39 ''' 40 '(' 41 ')' 42 '*' 43 '+' 44 ',' 45 '-' 46 '.' 47 '/' 48 '0' 49 '1' 50 '2' 51 '3' 52 '4' 53 '5' 54 '6' 55 '7' 56 '8' 57 '9' 58 ':' 59 ';' 60 '&lt;' 61 '=' 62 '>' 63 '?' 64 '@' 65 'A' 66 'B' 67 'C' 68 'D' 69 'E' 70 'F' 71 'G' 72 'H' 73 'I' 74 'J' 75 'K' 76 'L' 77 'M' 78 'N' 79 'O' 80 'P' 81 'Q' 82 'R' 83 'S' 84 'T' 85 'U' 86 'V' 87 'W' 88 'X' 89 'Y' 90 'Z' 91 '[' 92 '\' 93 ']' 94 '^' 95 '_' 96 '`' 97 'a' 98 'b' 99 'c' 100 'd' 101 'e' 102 'f' 103 'g' 104 'h' 105 'i' 106 'j' 107 'k' 108 'l' 109 'm' 110 'n' 111 'o' 112 'p' 113 'q' 114 'r' 115 's' 116 't' 117 'u' 118 'v' 119 'w' 120 'x' 121 'y' 122 'z' 123 '{' 124 '|' 125 '}' 126 '~'   
________________________________________ 
Part 2:  
Write a C program that asks the user to type in the starting and ending values and then prints the ASCII table entries using a for-loop. Assume the user types two valid integers within range separated by space.  % cc part2.c % ./a.out please input the starting and finishing ASCII codes: 65 90 
65 'A' 66 'B' 67 'C' 68 'D' 69 'E' 70 'F' 71 'G' 72 'H' 73 'I' 74 'J' 75 'K' 76 'L' 77 'M' 78 'N' 79 'O' 80 'P' 81 'Q' 82 'R' 83 'S' 84 'T' 85 'U' 86 'V' 87 'W' 88 'X' 89 'Y' 90 'Z' % _   
________________________________________ 
Part 3:  Write a C program that uses a printf statement to print the source code to your program in Part 2.  % cc part3.c % ./a.out > part3.out % diff ../part2/part2.c part3.out % _   If the two files are different, then diff will display their differences. If their contents are identical, then diff will show no difference.
