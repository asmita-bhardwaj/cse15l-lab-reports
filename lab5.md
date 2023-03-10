# Lab Report 5: Doing Lab Report 3 For a Different Command (find)

For this lab report, I've chosen to do the same exploration as lab report 3 for find instead of grep. 

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

In the example above we can see how the command line argument, find directory -size (-size), can be used to search a directory for files that are less in size than specified in the command, in this case 10.

**EXAMPLE 2**

**Command Line Argument**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -size +200

**Output**

    travel_guides/berlitz1/WhereToIndia.txt
    travel_guides/berlitz1/WhereToItaly.txt
    travel_guides/berlitz1/WhereToMalaysia.txt
    travel_guides/berlitz1/WhereToJapan.txt
    travel_guides/berlitz1/WhereToFrance.txt
    travel_guides/berlitz2/Portugal-WhereToGo.txt
    travel_guides/berlitz2/Canada-WhereToGo.txt
    travel_guides/berlitz2/China-WhereToGo.txt
    
In the example above we can see how the command line argument, find directory -size (+size), can be used to search a directory for files that are more in size than specified in the command, in this case 200.


## `-name`

`find  directory -name "string"` displays all the files in said directory include the "string" specified in the command line argument. My source for this specific command line argument is: https://linuxhandbook.com/find-command-examples/

**EXAMPLE 1**

**Input**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -name  "*.txt" 
    
**Output**

    travel_guides/berlitz1/HandRLasVegas.txt
    travel_guides/berlitz1/HistoryJapan.txt
    travel_guides/berlitz1/IntroMalaysia.txt
    travel_guides/berlitz1/HandRIstanbul.txt
    travel_guides/berlitz1/HistoryJamaica.txt
    travel_guides/berlitz1/HandRJamaica.txt
    travel_guides/berlitz1/HandRHongKong.txt
    travel_guides/berlitz1/HistoryEgypt.txt
    travel_guides/berlitz1/IntroEdinburgh.txt
    travel_guides/berlitz1/HistoryIsrael.txt
    travel_guides/berlitz1/IntroDublin.txt
    travel_guides/berlitz1/HistoryIndia.txt
    travel_guides/berlitz1/IntroFrance.txt
    travel_guides/berlitz1/IntroMadeira.txt
    travel_guides/berlitz1/WhatToLakeDistrict.txt
    travel_guides/berlitz1/IntroIbiza.txt
    travel_guides/berlitz1/HistoryItaly.txt
    travel_guides/berlitz1/WhereToGreek.txt
    travel_guides/berlitz1/WhereToLakeDistrict.txt
    travel_guides/berlitz1/HistoryDublin.txt
    travel_guides/berlitz1/IntroIsrael.txt
    travel_guides/berlitz1/WhatToIbiza.txt
    travel_guides/berlitz1/HistoryFrance.txt
    travel_guides/berlitz1/WhatToHawaii.txt
    travel_guides/berlitz1/HistoryMallorca.txt
    travel_guides/berlitz1/HistoryJerusalem.txt
    travel_guides/berlitz1/HandRLisbon.txt
    travel_guides/berlitz1/WhereToIndia.txt
    travel_guides/berlitz1/HistoryMadrid.txt
    travel_guides/berlitz1/HistoryHongKong.txt
    travel_guides/berlitz1/IntroMadrid.txt
    travel_guides/berlitz1/IntroLosAngeles.txt
    travel_guides/berlitz1/HistoryIstanbul.txt
    travel_guides/berlitz1/WhereToItaly.txt
    travel_guides/berlitz1/HistoryLasVegas.txt
    travel_guides/berlitz1/HistoryGreek.txt
    travel_guides/berlitz1/HandRMallorca.txt
    travel_guides/berlitz1/JungleMalaysia.txt
    travel_guides/berlitz1/WhatToMadeira.txt
    travel_guides/berlitz1/WhatToFWI.txt
    travel_guides/berlitz1/WhereToMalaysia.txt
    travel_guides/berlitz1/WhatToMalaysia.txt
    travel_guides/berlitz1/WhatToDublin.txt
    travel_guides/berlitz1/WhereToJapan.txt
    travel_guides/berlitz1/HistoryHawaii.txt
    travel_guides/berlitz1/WhatToFrance.txt
    travel_guides/berlitz1/WhereToEgypt.txt
    travel_guides/berlitz1/WhereToEdinburgh.txt
    travel_guides/berlitz1/WhatToIsrael.txt
    travel_guides/berlitz1/HandRLosAngeles.txt
    travel_guides/berlitz1/HistoryMadeira.txt
    travel_guides/berlitz1/IntroJerusalem.txt
    travel_guides/berlitz1/HandRMadeira.txt
    travel_guides/berlitz1/WhereToIsrael.txt
    travel_guides/berlitz1/HandRIbiza.txt
    travel_guides/berlitz1/WhereToFrance.txt
    travel_guides/berlitz1/WhereToDublin.txt
    travel_guides/berlitz1/IntroLasVegas.txt
    travel_guides/berlitz1/IntroIstanbul.txt
    travel_guides/berlitz1/WhereToMallorca.txt
    travel_guides/berlitz1/WhatToMallorca.txt
    travel_guides/berlitz1/IntroHongKong.txt
    travel_guides/berlitz1/IntroFWI.txt
    travel_guides/berlitz1/IntroJamaica.txt
    travel_guides/berlitz1/IntroGreek.txt
    travel_guides/berlitz1/HandRIsrael.txt
    travel_guides/berlitz1/WhatToEdinburgh.txt
    travel_guides/berlitz1/WhereToMadeira.txt
    travel_guides/berlitz1/WhatToGreek.txt
    travel_guides/berlitz1/HandRLakeDistrict.txt
    travel_guides/berlitz1/WhereToIbiza.txt
    travel_guides/berlitz1/WhereToHawaii.txt
    travel_guides/berlitz1/HandRMadrid.txt
    travel_guides/berlitz1/HistoryMalaysia.txt
    travel_guides/berlitz1/IntroItaly.txt
    travel_guides/berlitz1/WhatToIndia.txt
    travel_guides/berlitz1/WhereToLosAngeles.txt
    travel_guides/berlitz1/HandRJerusalem.txt
    travel_guides/berlitz1/HistoryIbiza.txt
    travel_guides/berlitz1/HistoryEdinburgh.txt
    travel_guides/berlitz1/HistoryFWI.txt
    travel_guides/berlitz1/IntroIndia.txt
    travel_guides/berlitz1/WhatToItaly.txt
    travel_guides/berlitz1/HistoryLakeDistrict.txt
    travel_guides/berlitz1/WhereToMadrid.txt
    travel_guides/berlitz1/WhereToJerusalem.txt
    travel_guides/berlitz1/IntroEgypt.txt
    travel_guides/berlitz1/HandRHawaii.txt
    travel_guides/berlitz1/WhatToJapan.txt
    travel_guides/berlitz1/WhatToJamaica.txt
    travel_guides/berlitz1/IntroLakeDistrict.txt
    travel_guides/berlitz1/IntroMallorca.txt
    travel_guides/berlitz1/WhatToHongKong.txt
    travel_guides/berlitz1/WhatToEgypt.txt
    travel_guides/berlitz1/WhereToHongKong.txt
    travel_guides/berlitz1/WhereToFWI.txt
    travel_guides/berlitz1/WhatToIstanbul.txt
    travel_guides/berlitz1/WhereToIstanbul.txt
    travel_guides/berlitz1/IntroJapan.txt
    travel_guides/berlitz1/WhatToLasVegas.txt
    travel_guides/berlitz1/WhatToLosAngeles.txt
    travel_guides/berlitz2/Portugal-History.txt
    travel_guides/berlitz2/Berlin-WhereToGo.txt
    travel_guides/berlitz2/Costa-History.txt
    travel_guides/berlitz2/Amsterdam-WhereToGo.txt
    travel_guides/berlitz2/Costa-WhereToGo.txt
    travel_guides/berlitz2/Amsterdam-WhatToDo.txt
    travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
    travel_guides/berlitz2/Barcelona-History.txt
    travel_guides/berlitz2/Portugal-WhereToGo.txt
    travel_guides/berlitz2/Boston-WhereToGo.txt
    travel_guides/berlitz2/Poland-WhatToDo.txt
    travel_guides/berlitz2/California-WhereToGo.txt
    travel_guides/berlitz2/Cuba-WhatToDo.txt
    travel_guides/berlitz2/Berlin-History.txt
    travel_guides/berlitz2/Bahamas-WhereToGo.txt
    travel_guides/berlitz2/Cancun-WhatToDo.txt
    travel_guides/berlitz2/Bali-History.txt
    travel_guides/berlitz2/Crete-WhereToGo.txt
    travel_guides/berlitz2/Athens-History.txt
    travel_guides/berlitz2/Berlin-WhatToDo.txt
    travel_guides/berlitz2/Canada-WhereToGo.txt
    travel_guides/berlitz2/Bali-WhereToGo.txt
    travel_guides/berlitz2/Budapest-WhereoGo.txt
    travel_guides/berlitz2/Barcelona-WhereToGo.txt
    travel_guides/berlitz2/Athens-WhereToGo.txt
    travel_guides/berlitz2/Paris-WhereToGo.txt
    travel_guides/berlitz2/China-WhereToGo.txt
    travel_guides/berlitz2/Bermuda-WhatToDo.txt
    travel_guides/berlitz2/California-History.txt
    travel_guides/berlitz2/Vallarta-History.txt
    travel_guides/berlitz2/Budapest-WhatToDo.txt
    travel_guides/berlitz2/Cancun-History.txt
    travel_guides/berlitz2/PuertoRico-WhatToDo.txt
    travel_guides/berlitz2/Vallarta-WhatToDo.txt
    travel_guides/berlitz2/Bali-WhatToDo.txt
    travel_guides/berlitz2/CostaBlanca-History.txt
    travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
    travel_guides/berlitz2/NewOrleans-History.txt
    travel_guides/berlitz2/PuertoRico-History.txt
    travel_guides/berlitz2/Algarve-Intro.txt
    travel_guides/berlitz2/Nepal-History.txt
    travel_guides/berlitz2/China-History.txt
    travel_guides/berlitz2/Canada-History.txt
    travel_guides/berlitz2/Crete-History.txt
    travel_guides/berlitz2/Portugal-WhatToDo.txt
    travel_guides/berlitz2/Bahamas-Intro.txt
    travel_guides/berlitz2/Amsterdam-History.txt
    travel_guides/berlitz2/Bahamas-WhatToDo.txt
    travel_guides/berlitz2/Barcelona-WhatToDo.txt
    travel_guides/berlitz2/Algarve-WhatToDo.txt
    travel_guides/berlitz2/PuertoRico-WhereToGo.txt
    travel_guides/berlitz2/Cuba-WhereToGo.txt
    travel_guides/berlitz2/Costa-WhatToDo.txt
    travel_guides/berlitz2/Beijing-History.txt
    travel_guides/berlitz2/Nepal-WhereToGo.txt
    travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
    travel_guides/berlitz2/Bermuda-history.txt
    travel_guides/berlitz2/CanaryIslands-History.txt
    travel_guides/berlitz2/Amsterdam-Intro.txt
    travel_guides/berlitz2/Crete-WhatToDo.txt
    travel_guides/berlitz2/Algarve-WhereToGo.txt
    travel_guides/berlitz2/Athens-Intro.txt
    travel_guides/berlitz2/Algarve-History.txt
    travel_guides/berlitz2/Poland-History.txt
    travel_guides/berlitz2/Beijing-WhereToGo.txt
    travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
    travel_guides/berlitz2/California-WhatToDo.txt
    travel_guides/berlitz2/Budapest-History.txt
    travel_guides/berlitz2/China-WhatToDo.txt
    travel_guides/berlitz2/Athens-WhatToDo.txt
    travel_guides/berlitz2/Nepal-WhatToDo.txt
    travel_guides/berlitz2/Bermuda-WhereToGo.txt
    travel_guides/berlitz2/Paris-WhatToDo.txt
    travel_guides/berlitz2/Cuba-History.txt
    travel_guides/berlitz2/Vallarta-WhereToGo.txt
    travel_guides/berlitz2/Bahamas-History.txt
    travel_guides/berlitz2/Beijing-WhatToDo.txt
    travel_guides/berlitz2/Cancun-WhereToGo.txt
    
In the example above we can see how the command line argument, find  directory -name "string", can be used to search a directory for files that contain "string" in their name, in this case ".txt". The * in the string allows to search for files that contain .txt in their name, not requiring the whole file to be just named .txt.

**EXAMPLE 2**

**Input**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -name  "*Malaysia*" 

**Output**

    travel_guides/berlitz1/IntroMalaysia.txt
    travel_guides/berlitz1/JungleMalaysia.txt
    travel_guides/berlitz1/WhereToMalaysia.txt
    travel_guides/berlitz1/WhatToMalaysia.txt
    travel_guides/berlitz1/HistoryMalaysia.txt
    
In the example above we can see how the command line argument, find  directory -name "string", can be used to search a directory for files that contain "string" in their name, in this case "Malaysia". The * in the string allows to search for files that contain Malaysia in their name, not requiring the whole file to be just named Malaysia.


## `-type`

`find  directory -type (f or d)` displays either only files (by using f) or directories (by using d) in the specific directory. It is useful to find subdirectories within a directory efficiently through this command line argument. My source for this specific command line argument is: https://linuxhandbook.com/find-command-examples/

**EXAMPLE 1**

**Input**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -type f
    
**Output**

    travel_guides/.DS_Store
    travel_guides/berlitz1/HandRLasVegas.txt
    travel_guides/berlitz1/HistoryJapan.txt
    travel_guides/berlitz1/IntroMalaysia.txt
    travel_guides/berlitz1/HandRIstanbul.txt
    travel_guides/berlitz1/HistoryJamaica.txt
    travel_guides/berlitz1/HandRJamaica.txt
    travel_guides/berlitz1/HandRHongKong.txt
    travel_guides/berlitz1/HistoryEgypt.txt
    travel_guides/berlitz1/IntroEdinburgh.txt
    travel_guides/berlitz1/HistoryIsrael.txt
    travel_guides/berlitz1/IntroDublin.txt
    travel_guides/berlitz1/HistoryIndia.txt
    travel_guides/berlitz1/IntroFrance.txt
    travel_guides/berlitz1/IntroMadeira.txt
    travel_guides/berlitz1/WhatToLakeDistrict.txt
    travel_guides/berlitz1/IntroIbiza.txt
    travel_guides/berlitz1/HistoryItaly.txt
    travel_guides/berlitz1/WhereToGreek.txt
    travel_guides/berlitz1/WhereToLakeDistrict.txt
    travel_guides/berlitz1/HistoryDublin.txt
    travel_guides/berlitz1/IntroIsrael.txt
    travel_guides/berlitz1/WhatToIbiza.txt
    travel_guides/berlitz1/HistoryFrance.txt
    travel_guides/berlitz1/WhatToHawaii.txt
    travel_guides/berlitz1/HistoryMallorca.txt
    travel_guides/berlitz1/HistoryJerusalem.txt
    travel_guides/berlitz1/HandRLisbon.txt
    travel_guides/berlitz1/WhereToIndia.txt
    travel_guides/berlitz1/HistoryMadrid.txt
    travel_guides/berlitz1/HistoryHongKong.txt
    travel_guides/berlitz1/IntroMadrid.txt
    travel_guides/berlitz1/IntroLosAngeles.txt
    travel_guides/berlitz1/HistoryIstanbul.txt
    travel_guides/berlitz1/WhereToItaly.txt
    travel_guides/berlitz1/HistoryLasVegas.txt
    travel_guides/berlitz1/HistoryGreek.txt
    travel_guides/berlitz1/HandRMallorca.txt
    travel_guides/berlitz1/JungleMalaysia.txt
    travel_guides/berlitz1/WhatToMadeira.txt
    travel_guides/berlitz1/WhatToFWI.txt
    travel_guides/berlitz1/WhereToMalaysia.txt
    travel_guides/berlitz1/WhatToMalaysia.txt
    travel_guides/berlitz1/WhatToDublin.txt
    travel_guides/berlitz1/WhereToJapan.txt
    travel_guides/berlitz1/HistoryHawaii.txt
    travel_guides/berlitz1/WhatToFrance.txt
    travel_guides/berlitz1/WhereToEgypt.txt
    travel_guides/berlitz1/WhereToEdinburgh.txt
    travel_guides/berlitz1/WhatToIsrael.txt
    travel_guides/berlitz1/HandRLosAngeles.txt
    travel_guides/berlitz1/HistoryMadeira.txt
    travel_guides/berlitz1/IntroJerusalem.txt
    travel_guides/berlitz1/HandRMadeira.txt
    travel_guides/berlitz1/WhereToIsrael.txt
    travel_guides/berlitz1/HandRIbiza.txt
    travel_guides/berlitz1/WhereToFrance.txt
    travel_guides/berlitz1/WhereToDublin.txt
    travel_guides/berlitz1/IntroLasVegas.txt
    travel_guides/berlitz1/IntroIstanbul.txt
    travel_guides/berlitz1/WhereToMallorca.txt
    travel_guides/berlitz1/WhatToMallorca.txt
    travel_guides/berlitz1/IntroHongKong.txt
    travel_guides/berlitz1/IntroFWI.txt
    travel_guides/berlitz1/IntroJamaica.txt
    travel_guides/berlitz1/IntroGreek.txt
    travel_guides/berlitz1/HandRIsrael.txt
    travel_guides/berlitz1/WhatToEdinburgh.txt
    travel_guides/berlitz1/WhereToMadeira.txt
    travel_guides/berlitz1/WhatToGreek.txt
    travel_guides/berlitz1/HandRLakeDistrict.txt
    travel_guides/berlitz1/WhereToIbiza.txt
    travel_guides/berlitz1/WhereToHawaii.txt
    travel_guides/berlitz1/HandRMadrid.txt
    travel_guides/berlitz1/HistoryMalaysia.txt
    travel_guides/berlitz1/IntroItaly.txt
    travel_guides/berlitz1/WhatToIndia.txt
    travel_guides/berlitz1/WhereToLosAngeles.txt
    travel_guides/berlitz1/HandRJerusalem.txt
    travel_guides/berlitz1/HistoryIbiza.txt
    travel_guides/berlitz1/HistoryEdinburgh.txt
    travel_guides/berlitz1/HistoryFWI.txt
    travel_guides/berlitz1/IntroIndia.txt
    travel_guides/berlitz1/WhatToItaly.txt
    travel_guides/berlitz1/HistoryLakeDistrict.txt
    travel_guides/berlitz1/WhereToMadrid.txt
    travel_guides/berlitz1/WhereToJerusalem.txt
    travel_guides/berlitz1/IntroEgypt.txt
    travel_guides/berlitz1/HandRHawaii.txt
    travel_guides/berlitz1/WhatToJapan.txt
    travel_guides/berlitz1/WhatToJamaica.txt
    travel_guides/berlitz1/IntroLakeDistrict.txt
    travel_guides/berlitz1/IntroMallorca.txt
    travel_guides/berlitz1/WhatToHongKong.txt
    travel_guides/berlitz1/WhatToEgypt.txt
    travel_guides/berlitz1/WhereToHongKong.txt
    travel_guides/berlitz1/WhereToFWI.txt
    travel_guides/berlitz1/WhatToIstanbul.txt
    travel_guides/berlitz1/WhereToIstanbul.txt
    travel_guides/berlitz1/IntroJapan.txt
    travel_guides/berlitz1/WhatToLasVegas.txt
    travel_guides/berlitz1/WhatToLosAngeles.txt
    travel_guides/berlitz2/Portugal-History.txt
    travel_guides/berlitz2/Berlin-WhereToGo.txt
    travel_guides/berlitz2/Costa-History.txt
    travel_guides/berlitz2/Amsterdam-WhereToGo.txt
    travel_guides/berlitz2/Costa-WhereToGo.txt
    travel_guides/berlitz2/Amsterdam-WhatToDo.txt
    travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
    travel_guides/berlitz2/Barcelona-History.txt
    travel_guides/berlitz2/Portugal-WhereToGo.txt
    travel_guides/berlitz2/Boston-WhereToGo.txt
    travel_guides/berlitz2/Poland-WhatToDo.txt
    travel_guides/berlitz2/California-WhereToGo.txt
    travel_guides/berlitz2/Cuba-WhatToDo.txt
    travel_guides/berlitz2/Berlin-History.txt
    travel_guides/berlitz2/Bahamas-WhereToGo.txt
    travel_guides/berlitz2/Cancun-WhatToDo.txt
    travel_guides/berlitz2/Bali-History.txt
    travel_guides/berlitz2/Crete-WhereToGo.txt
    travel_guides/berlitz2/Athens-History.txt
    travel_guides/berlitz2/Berlin-WhatToDo.txt
    travel_guides/berlitz2/Canada-WhereToGo.txt
    travel_guides/berlitz2/Bali-WhereToGo.txt
    travel_guides/berlitz2/Budapest-WhereoGo.txt
    travel_guides/berlitz2/Barcelona-WhereToGo.txt
    travel_guides/berlitz2/Athens-WhereToGo.txt
    travel_guides/berlitz2/Paris-WhereToGo.txt
    travel_guides/berlitz2/China-WhereToGo.txt
    travel_guides/berlitz2/Bermuda-WhatToDo.txt
    travel_guides/berlitz2/California-History.txt
    travel_guides/berlitz2/Vallarta-History.txt
    travel_guides/berlitz2/Budapest-WhatToDo.txt
    travel_guides/berlitz2/Cancun-History.txt
    travel_guides/berlitz2/PuertoRico-WhatToDo.txt
    travel_guides/berlitz2/Vallarta-WhatToDo.txt
    travel_guides/berlitz2/Bali-WhatToDo.txt
    travel_guides/berlitz2/CostaBlanca-History.txt
    travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
    travel_guides/berlitz2/NewOrleans-History.txt
    travel_guides/berlitz2/PuertoRico-History.txt
    travel_guides/berlitz2/Algarve-Intro.txt
    travel_guides/berlitz2/Nepal-History.txt
    travel_guides/berlitz2/China-History.txt
    travel_guides/berlitz2/Canada-History.txt
    travel_guides/berlitz2/Crete-History.txt
    travel_guides/berlitz2/Portugal-WhatToDo.txt
    travel_guides/berlitz2/Bahamas-Intro.txt
    travel_guides/berlitz2/Amsterdam-History.txt
    travel_guides/berlitz2/Bahamas-WhatToDo.txt
    travel_guides/berlitz2/Barcelona-WhatToDo.txt
    travel_guides/berlitz2/Algarve-WhatToDo.txt
    travel_guides/berlitz2/PuertoRico-WhereToGo.txt
    travel_guides/berlitz2/Cuba-WhereToGo.txt
    travel_guides/berlitz2/Costa-WhatToDo.txt
    travel_guides/berlitz2/Beijing-History.txt
    travel_guides/berlitz2/Nepal-WhereToGo.txt
    travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
    travel_guides/berlitz2/Bermuda-history.txt
    travel_guides/berlitz2/CanaryIslands-History.txt
    travel_guides/berlitz2/Amsterdam-Intro.txt
    travel_guides/berlitz2/Crete-WhatToDo.txt
    travel_guides/berlitz2/Algarve-WhereToGo.txt
    travel_guides/berlitz2/Athens-Intro.txt
    travel_guides/berlitz2/Algarve-History.txt
    travel_guides/berlitz2/Poland-History.txt
    travel_guides/berlitz2/Beijing-WhereToGo.txt
    travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
    travel_guides/berlitz2/California-WhatToDo.txt
    travel_guides/berlitz2/Budapest-History.txt
    travel_guides/berlitz2/China-WhatToDo.txt
    travel_guides/berlitz2/Athens-WhatToDo.txt
    travel_guides/berlitz2/Nepal-WhatToDo.txt
    travel_guides/berlitz2/Bermuda-WhereToGo.txt
    travel_guides/berlitz2/Paris-WhatToDo.txt
    travel_guides/berlitz2/Cuba-History.txt
    travel_guides/berlitz2/Vallarta-WhereToGo.txt
    travel_guides/berlitz2/Bahamas-History.txt
    travel_guides/berlitz2/Beijing-WhatToDo.txt
    travel_guides/berlitz2/Cancun-WhereToGo.txt
    
In the example above we can see how the command line argument,find  directory -type f, can be used to search a directory for files using f. 

**EXAMPLE 2**

**Input**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -type d
    
**Output**

    travel_guides
    travel_guides/berlitz1
    travel_guides/berlitz2
    
In the example above we can see how the command line argument,find  directory -type d, can be used to search a directory for more directories using d.


## `-delete`

`find directory -name "filename" -delete` deletes the file found first through the -name command line. It deletes the file specified by "filename" in the specific directory. My source for this specific command line argument is: https://linuxhandbook.com/find-command-examples/

**EXAMPLE 1**

**Input**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -name "Beijing-WhatToDo.txt" -delete
    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -name "Beijing-WhatToDo.txt"

**Output**

    <empty>
    

In the example above we can see how the command line argument,find  directory -name "filename" -delete, can be used to delete a certain file from a directory, in this case "Beijing-WhatToDo.txt". This is proved by using the find -name command line to find the same file after the -delete command line and having it return nothing, as the file no longeer exists. 

**EXAMPLE 2**

**Inputs**

    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -name "Beijing-WheretToGo.txt" -delete
    Asmitas-MacBook-Air:written_2 asmita$ find travel_guides -name "Beijing-WheretToGo.txt" 
    
**Output**

    <empty>
    
In the example above we can see how the command line argument,find  directory -name "filename" -delete, can be used to delete a certain file from a directory, in this case "Beijing-WhereToGo.txt". This is proved by using the find -name command line to find the same file after the -delete command line and having it return nothing, as the file no longeer exists. 
