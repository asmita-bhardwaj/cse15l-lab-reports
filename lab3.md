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

	Asmitas-MacBook-Air:written_2 asmita$ grep -c "To" */*/*/**

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


**EXAMPLE 2**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -c "Athens" travel_guides/berlitz2/Athens-WhatToDo.txt

**Output**

	16


## `-n`

`grep -n "word" file` displays the line number in the specific file in which "word" exists along with the full line.   

**EXAMPLE 1**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -n "traditional" travel_guides/berlitz2/Budapest-WhereoGo.txt

**Output**

	123:Just behind the baths are the zoo and two amusement parks. The zoo welcomes visitors with an Art Nouveau entrance 
	decorated with polar bears and elephants. It keeps a wide range of animals, including most children’s and adults’ favourite species. 
	The animals are mostly held in traditional cages, though renovations on several pavilions are in progress. Grown-ups may like to note 
	that next to the zoo is Gundel’s restaurant, a legend in Hungarian culinary circles.
	131:Teréz körút and Erzsébet körút have traditionally been centres of Budapest’s cultural, as well as its commercial, life. At the 
	Great Boulevard’s intersection with Dohány utca is the New York Café (formerly known as the Hungaria). The café’s Neo-Baroque Art 
	Nouveau interior, shining with polished wood, brass, and cut glass, has been restored to its original gaudy glory — it looks the same 
	as it did at the beginning of the 20th century. It is once again a meeting point for actors, writers, and journalists. 
	169:Tihany is built high on a hill above the main lake, and its principal street, Pisky sétány (a promenade), has a few charming 
	traditional thatched houses. Start your tour of the village below this point at the Abbey Church (Apátság), which stands just off the 
	main road. The present 18th-century Baroque church stands over an atmospheric crypt almost a thousand years old. A rare survivor in 
	a land constantly ravaged by so many invasions, it is claimed to be the oldest in Hungary. Here you will ﬁnd the tomb of King András 
	(Andrew) I who, in 1055, founded the Benedictine Abbey that once stood on this site. The church itself is being renovated at present, 
	but even through the tarpaulins you can glimpse its rich Baroque carvings and decorative ornamentation.
	

**EXAMPLE 2**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -n "tourist" */*/*/**

**Output**

	non-fiction/OUP/Rybczynski/ch2.txt:25:The Kennedy Center was criticized from the start, but the dazzling décor 
	of Radio City Music Hall, which opened in 1932—in the midst of the Depression—guaranteed its immediate success. 
	Radio City became the most famous theater in the country, the Rockettes the most famous chorus line, “live from Radio City” 
	the most famous dateline. In the late 1950s, when I visited New York City as a boy with my parents, Radio City was still 
	one of the obligatory tourist sites. What I don’t remember is ever learning about Radio City as an architecture student. 
	According to the reductive standards of my International Style teachers, its opulent materials, its glowing colors, and 
	its very theatricality disqualified Radio City as architecture (never mind that it was a technologically sophisticated “machine 
	for entertainment”). It was dismissed as kitsch. By 1978, Radio City had lost its glamour, and the owners of Rockefeller 
	Center decided to demolish the aging hall. Thanks to preservationists’ efforts, the hall was saved from demolition and granted 
	landmark status. Now, 20 years later, freshened by a masterful restoration, it is once again acclaimed as a masterpiece.
	non-fiction/OUP/Rybczynski/ch2.txt:32:Walpole, the Fourth Earl of Orford, spent his entire life enlarging his house. He 
	eventually added a cloister, a gallery, and a tower. As he was an author and a public figure who corresponded with a wide 
	circle of literary and artistic friends throughout Europe, the Gothic design of Strawberry Hill became famous among connoisseurs. 
	(It also became a tourist attraction, much to Walpole’s chagrin.) Architects and their clients now saw medieval buildings as 
	sources of inspiration, just as they had once looked to ancient Greece and Rome. The Gothic style became an established alternative 
	for building country houses, and pointed arches appeared in décor and furniture. Gothic was “in” again.

## `-r`

`grep -r` is a command line argument that uses recursion while searching through repositories. This command line is not required to be run on a specific file, but instead has the ability to search every file within a directory, as well as the directory itself.  

## `-i`

