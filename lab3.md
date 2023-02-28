# Lab Report 3

## `grep`

I chose to research on the command `grep`, where I will explore the following command-line arguments:
- `-c`
- `-n`
- `-r`
- `-i`

I researched on each command from the GNU manual page, https://www.gnu.org/software/grep/manual/grep.html#Command_002dline-Options. 

## `-c`

`grep -c string file/directory` displays the number of lines in the specific file in which `string` exists.

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

`grep -n string file` displays the line number in the specific file in which `string` exists along with the full line.   

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

`grep -r string directory` is a command line argument that uses recursion while searching through repositories. This command line is not required to be run on a specific file, but instead has the ability to search every file within a directory, as well as the directory itself.  

**EXAMPLE 1**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -r "persuasive"

**Output**

	./non-fiction/OUP/Kauffman/ch5.txt:The eorts following Hume to understand the meaning of ethical assertions have been long, twisted, arduous. 
	Following the dictates of the logical positivists of the Vienna Circle that only those statements capable of verification were meaningful, 
	philosophers as famous as G. E. Moore came to wonder if ethical assertions were merely emotive utterances. “It is wrong to kill.” Becomes, 
	“Agggah!” Does the positivist argument seem persuasive? It has always amused me that the core injunction of the logical positivists, “only 
	those statements that are empirically verifiable are meaningful,” is itself not empirically verifiable. One is reminded of something about
	hoisting and petards. 
	./non-fiction/OUP/Kauffman/ch6.txt:Wittgenstein wrote persuasively that the same systematic diYculty was lodged in attempts to reduce one 
	language game to another, for example, from a description of a legal event to a description in terms of mere human actions to a description
	in terms of physical events. As we noted earlier, legal descriptions involve a web of concepts concerning guilt, innocence, responsibility,
	evidence, admissible procedure that are absent from a description of human actions outside of the legal framework. And descriptions of human 
	actions = and, a fortiori, descriptions of the doings of autonomous agents, even bacteria acting on their own behalf to get dinner = seem 
	to involve a diVerent language game than mere descriptions in terms of physical events.
	./non-fiction/OUP/Fletcher/ch6.txt:This case would have been persuasive precedent for the butchers but for two hurdles that counsel had 
	to negotiate. The first was to brand the New Orleans slaughtering franchise a “monopoly.” That proved to be problematic. The dissenting 
	judges had no trouble concluding that requiring the butchers to use, for a fee, a single slaughterhouse was as “much a monopoly as 
	though the act had granted to the company the exclusive privilege of buying and selling the animals themselves.”13 But the majority, 
	led by Justice Miller, balked. The Court was willing to accept the label of “monopoly” but denied “the assertion that the butchers 
	are [thereby] deprived of the right to labor in their occupation.”14 
	./travel_guides/berlitz2/Cancun-WhereToGo.txt:There is only one settlement, the capital, on Cozumel, San Miguel de Cozumel; it’s a 
	bustling town chock-full of souvenir shops, duty-free emporiums, bars, and assorted cafés and restaurants. If you arrive on the island by 
	ferry from the mainland, you’ll be dropped off directly opposite the heart of the downtown area, Plaza del Sol, also called the zócalo. 
	This large, tree-lined square is where everyone meets for coffee, or lunch at one of the cafés nearby. Several streets surrounding the 
	square are traffic-free, and you can stroll at your leisure among the stores selling T-shirts, pottery, onyx, and silver. The storeowners 
	have a practiced line and can be pretty persuasive, so it pays to have a sense of humor — or a few words of Spanish so you can join 
	in the banter.


**EXAMPLE 2**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -r "conclusive"


**Output**

	./non-fiction/OUP/Berk/ch1.txt:Furthermore, no conclusive evidence exists for the assertion that the most consequential 
	environment for children’s development is the peer group rather than the family. It is based on an array of selective and equivocal 
	ﬁndings, mustered to convince readers that parenting eects are conﬁned to how children behave in parents’ presence and do not 
	extend beyond the home. I will show repeatedly in this book that just the opposite is so—that parenting practices have much to do with 
	children’s competence at language and communication; sensitivity to others’ feelings and needs; capacity to get along with others within 
	and beyond the family; achievement in school; and guiding values, beliefs, and attitudes.
	./non-fiction/OUP/Kauffman/ch8.txt:But what of real cells? We have no conclusive evidence, yet an abundance of telling hints. 
	If I am not yet entirely convinced and if I am  as I am  biased, I nevertheless become increasingly confident that cells, and probably 
	communities of cells, do live in the ordered regime near the edge of chaos. Not only does the evidence point this way, but cells should 
	live near the edge of chaos. Why? As remarked already, the intuition is simple. Being autonomous agents, cells must, as individuals 
	living in communities, make the maximum number of reliable discriminations possible and act on them reliably, without “trembling hands.” 
	Just inside the edge of chaos seems the ideal place.
	./non-fiction/OUP/Kauffman/ch8.txt:Darwin is correct about contemporary life, and presumably about ancient life, based on the record. 
	In fact, for current life forms, seven decades of hard work by geneticists, working with organisms as disparate as mouse, fruit fly, 
	maize, yeast, and many other eukaryotes, demonstrates conclusively that most mutations are of minor eect. For example, the fruit fly, 
	Drosophila melanogaster, upon which I worked for twelve years, has the abdominal bristles alluded to above. A modest number of mutants 
	exist that slightly increase or slightly decrease the number of abdominal bristles. The flies don’t seem to mind, at least in the 
	odd security of my and other biologists’ laboratories.
	./travel_guides/berlitz1/HistoryMadrid.txt:        inconclusively for six years. Finally, with the help of the British
	./travel_guides/berlitz2/PuertoRico-History.txt:Politically, recent history is less conclusive. In 1951 the island’s 
	voters approved a new constitution (still in effect) forming a commonwealth between the United States and the “free associated 
	state” of Puerto Rico (though even the commencement ceremony was marred by violent demonstrations by radicals). As a result 
	Puerto Ricans now elect their own governor, legislature, and local officials, and send a non-voting representative to the US Congress. 
	In turn, Washington runs the postal, customs, and immigration services, handles defense and foreign relations, and sends dollars 
	— particularly useful in times of crisis, such as after hurricanes.
	./travel_guides/berlitz2/Bermuda-history.txt:On a dark night in mid-August 1775, several boats sailed into the dark harbor 
	of Tobacco Bay near Fort St. Catherine and, in a daring and dangerous raid, stole 100 kegs of gunpowder from the main ordnance store. 
	Once safely on the boats, the ammunition made its way to the rebel forces. To this day nobody knows if this was part of an orchestrated 
	campaign or simply a spur-of-the-moment action by local sympathizers. But Bermuda got its grain. The British authorities were 
	horrified but could find no conclusive proof of guilt. The Tuckers, a prominent family with many connections to the American 
	revolutionaries, were the prime suspects. Not all Bermudians, however, were sympathetic to the rebel cause, as privateers continued to 
	capture and ransack American ships.


## `-i`

`grep -i string file` is a command line argument that displays sentences that include the `string`. The search is case insensitive, meaning that "historical" is the percieved as the same as "Historical".

**EXAMPLE 1**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -i "historical" travel_guides/berlitz2/Budapest-WhereoGo.txt
	
**Output**

	Historically, Obuda is the oldest quarter of Buda, centred on the site of Aquincum, the capital of the Roman province of 
	Lower Pannonia. Nowadays it’s a nightmare of Soviet town-planning, with heavy trafﬁc constantly rumbling past on the main 
	northern highway out of Budapest. Amid this unlikely setting, however, there are some major Roman remains to be discovered.
	Andrássy út ends in an outburst of pomp at Heroes’ Square (Hosök tere), a huge open space housing the Millenary Monument, built 
	on the thousandth anniversary of the Magyar conquest. Surmounting all is a 36-metre (118-foot) column supporting the ﬁgure of the 
	Archangel Gabriel, who, according to legend, appeared in a dream of St. Stephen’s and offered him Hungary’s first crown. Around 
	the pedestal, on horseback, sit Prince Arpád and the Magyar tribal chiefs, while ﬂanking the column is a semi-circular 
	colonnade with statues of historical ﬁgures, starting with King Stephen. In front of the statuary is the Tomb of the Unknown Soldier.
	Next door to the Abbey Church, housed in the old priory, is the Tihany Historical Museum (closed November to February). This 
	museum features regional folk items and art, three small rooms where Hungary’s last king, Károly IV, lived for ﬁve days in 1921, 
	and, in the basement, an atmospheric lapidarium containing Roman remains. In front of the church, King András is commemorated in 
	a typically offbeat Imre Varga statue, wrapped in an aluminium cloak.
	Continuing out of Keszthely to the southwest on Highway 71, you reach another good historical collection. The Balaton Museum 
	portrays the story of the settlement of the lake and the development of its people, including their agriculture and ﬁshing and its 
	fauna and flora, in a lively exhibition.
	
**EXAMPLE 2**

**Input**

	Asmitas-MacBook-Air:written_2 asmita$ grep -i "flora" travel_guides/berlitz2/Paris-WhereToGo.txt

**Output**

	Claude Monet’s glorious floral and water gardens are much more attractive than the rather artificially restored house. 
	The painter lived at Giverny from 1883 to 1926 and painted the gardens many times, especially the water lilies.
