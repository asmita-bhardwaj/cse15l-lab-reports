# Lab Report 5: Researching Commands 

## `find`

I chose to research on the command `find`, where I will explore the following command-line arguments:

- `-size`
- `-name`
- `-type`
- `-delete`

I research on each command from the GNU manual page https://www.gnu.org/software/findutils/manual/html_node/find_html/Invoking-find.html#Invoking-find.

## `-size`

`find  directory -size (+size/-size)` displays all the files in said directory that satisfies the size requirement mentioned by either (+size) or (-size). `+size` returns all the files that are greater than the size in the command line argument, while `-size` returns all the  files that are less  than the size in the command line argument. My command line argument is: https://linuxhandbook.com/find-command-examples/

**EXAMPLE 1**

**Command Line Argument**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -size -10
    
**Output**

    travel_guides
    travel_guides/berlitz1
    travel_guides/berlitz1/HandRLasVegas.txt
    travel_guides/berlitz1/HandRIstanbul.txt
    travel_guides/berlitz1/HandRHongKong.txt
    travel_guides/berlitz1/WhatToHawaii.txt
    travel_guides/berlitz1/HandRLisbon.txt
    travel_guides/berlitz1/HandRMallorca.txt
    travel_guides/berlitz1/WhatToFrance.txt
    travel_guides/berlitz1/HandRLosAngeles.txt
    travel_guides/berlitz1/HandRMadeira.txt
    travel_guides/berlitz1/HandRIbiza.txt
    travel_guides/berlitz1/HandRLakeDistrict.txt
    travel_guides/berlitz1/WhereToHawaii.txt
    travel_guides/berlitz1/HandRJerusalem.txt
    travel_guides/berlitz2

