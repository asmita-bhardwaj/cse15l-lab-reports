# Lab Report 3

## `grep`

I chose to research on the command `grep`, where I will explore the following command-line arguments:
- `-c`
- `-n`
- `-r`
- `-i`

I researched on each command from the GNU manual page, https://www.gnu.org/software/grep/manual/grep.html#Command_002dline-Options. 

## `-c`

`grep -c "word" file` displays the number of lines in the specific file in which "word" exists.

**EXAMPLE 1**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -c "Athens" travel_guides/berlitz2/Athens-WhatToDo.txt

**Output**

	16
	

**EXAMPLE 2**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -c "To" */*/*/*

**Output**

	non-fiction/OUP/Abernathy/ch1.txt:4
	non-fiction/OUP/Abernathy/ch14.txt:3
	non-fiction/OUP/Abernathy/ch15.txt:1
	non-fiction/OUP/Abernathy/ch2.txt:3
	non-fiction/OUP/Abernathy/ch3.txt:2
	non-fiction/OUP/Abernathy/ch6.txt:5
	non-fiction/OUP/Abernathy/ch7.txt:4
	non-fiction/OUP/Abernathy/ch8.txt:5
	non-fiction/OUP/Abernathy/ch9.txt:3
	non-fiction/OUP/Berk/CH4.txt:14
	non-fiction/OUP/Berk/ch1.txt:16
	non-fiction/OUP/Berk/ch2.txt:12
	non-fiction/OUP/Berk/ch7.txt:5
	non-fiction/OUP/Castro/chA.txt:3
	non-fiction/OUP/Castro/chB.txt:2
	non-fiction/OUP/Castro/chC.txt:2
	non-fiction/OUP/Castro/chL.txt:5
	non-fiction/OUP/Castro/chM.txt:6
	non-fiction/OUP/Castro/chN.txt:1
	non-fiction/OUP/Castro/chO.txt:1
	non-fiction/OUP/Castro/chP.txt:2
	non-fiction/OUP/Castro/chQ.txt:2
	non-fiction/OUP/Castro/chR.txt:5
	non-fiction/OUP/Castro/chV.txt:2
	non-fiction/OUP/Castro/chW.txt:2
	non-fiction/OUP/Castro/chY.txt:0
	non-fiction/OUP/Castro/chZ.txt:0
	non-fiction/OUP/Fletcher/ch1.txt:11
	non-fiction/OUP/Fletcher/ch10.txt:2
	non-fiction/OUP/Fletcher/ch2.txt:2
	non-fiction/OUP/Fletcher/ch5.txt:2
	non-fiction/OUP/Fletcher/ch6.txt:9
	non-fiction/OUP/Fletcher/ch9.txt:12
	non-fiction/OUP/Kauffman/ch1.txt:6
	non-fiction/OUP/Kauffman/ch10.txt:4
	non-fiction/OUP/Kauffman/ch3.txt:3
	non-fiction/OUP/Kauffman/ch4.txt:3
	non-fiction/OUP/Kauffman/ch5.txt:2
	non-fiction/OUP/Kauffman/ch6.txt:6
	non-fiction/OUP/Kauffman/ch7.txt:0
	non-fiction/OUP/Kauffman/ch8.txt:9
	non-fiction/OUP/Kauffman/ch9.txt:2
	non-fiction/OUP/Rybczynski/ch1.txt:5
	non-fiction/OUP/Rybczynski/ch2.txt:4
	non-fiction/OUP/Rybczynski/ch3.txt:5
    


## `-n`
`grep -n "query" filename` displays the line and line number in which "query" exists. 

**EXAMPLE #1** 
  


## `-r`

`grep -r` is a command line argument that uses recursion while searching through repositories. This command line is not required to be run on a specific file, but instead has the ability to search every file within a directory, as well as the directory itself.  

## `-i`

