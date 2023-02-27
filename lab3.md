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

	Asmitas-MacBook-Air:written_2 asmita$ grep -c "History" travel_guides/berlitz2/Bali-History.txt

**Output**

	1
    


## `-n`
`grep -n "query" filename` displays the line and line number in which "query" exists. 

**EXAMPLE #1** 
  


## `-r`

`grep -r` is a command line argument that uses recursion while searching through repositories. This command line is not required to be run on a specific file, but instead has the ability to search every file within a directory, as well as the directory itself.  

## `-i`

