# Researching the Grep Command 

## grep -w 

grep -w returns matches to word boundaries

    grep -w "fun" Costa-WhatToDo.txt
    
    Alternative diversions for children include the aquariums in Benalmádena and Puerto Banús, the Eagle Park in Benalmádena, the Cueva (cave) De Nerja, and Mini- Hollywood near Almería. In the evenings, Tívoli World near Benalmádena provides all the fun of the fair, with carnival rides and a roller coaster, and there’s also a bar and flamenco show for the grown-ups. The Crocodile Park just north of Málaga will intrigue most children, as will the horse shows of El Ranchito in Benalmádena and Aires del Sur in Estepona.
    
The command above is searching through the Costa-WhatToDo.txt file for text that appears near the word "fun". This can be useful if you are strictly looking for what the author describes as fun things to do in Costa del Sol. 

    grep -w habitually chM.txt
    
    Death, personified as a woman and dressed in white clothing, is a well-known character in Chicano and Mexicano folklore. Commonly accepted as just La Muerte, she is a frequent personality in legends, urban belief tales, and is integrated into many family folk belief systems. Death is sometimes feared, but it is also accepted as the transition to another stage of the life cycle. A common saying is “De la muerte y la suerte nadie se escapa” (No one escapes from death or luck) (Espinosa, A. M., 1910, 404). She habitually appears late at night, to men who are out alone, some intentionally, others innocently on their way home from work. In tales collected in the Southwest, La Muerte is seen standing at streetlights, or waiting by a bridge or the side of the road.
    
The command above is searching through chM.txt for text that appears near the word "habitually". This could be useful if you remember that word "habitually" being related to a section of the text that talks about something specific you are looking for. 
    
This command was found on the site [swcarpentry](https://swcarpentry.github.io/shell-novice/07-find/index.html#:~:text=The%20grep%20command%20searches%20through).

## grep -n 

grep -n returns lines to matching strings

    grep -n "If you head inland" IntroIbiza.txt
    
    89:        the essence of many delights. If you head inland to the less populous
    
The command above searches through IntroIbiza.txt for the line at which the specified string occurs. This can be helpful if you want to know things about inland Ibiza, or where the article talks about inland Ibiza. 

    grep -n "religious conflicts" IntroGreek.txt
    
    13:        religious conflicts between Christianity and Islam. Although they now
    
The command above searches through IntroGreek.txt for the line at which the specified string occurs. This could be help if you wanted to know where in the text it mentions religious conflicts, or how many times the phrase religious conflicts is mentioned throuhgout the article.

This command was found on the site [swcarpentry](https://swcarpentry.github.io/shell-novice/07-find/index.html#:~:text=The%20grep%20command%20searches%20through).

## grep -r 

grep -r searches for a pattern recursively through a set of files or subdirectory

    grep -r "Winston Churchill" berlitz2
    
    berlitz2/Berlin-WhereToGo.txt:Beside the lake, north of the town center is Neuer Garten, a pleasant English-style garden. It provides the perfect setting for Schloß Cecilienhof (1916), the ivy-covered, half-timbered pastiche of an English country manor built for Crown Prince Wilhelm and his wife. Winston Churchill, Joseph Stalin, and Harry Truman met here in July 1945 to draw up the Potsdam Agreement that fixed the division of Germany for the next 45 years. Today it’s a luxury hotel and restaurant.
    berlitz2/Costa-WhereToGo.txt:Legend has it that if the apes ever leave the Rock, then British rule will come to an end. When the apes’ population declined significantly during World War II, Winston Churchill himself was worried, and the monkeys have been on special rations ever since.
    berlitz2/California-WhereToGo.txt:It was still not completed by the time of Hearst’s death in 1951. Here he entertained the movie star Marion Davies, his mistress for 30 years, and famous guests such as Charlie Chaplin, Scott and Zelda Fitzgerald, Greta Garbo, Winston Churchill, Charles Lindbergh, and the photographer Herman Mankiewicz, who recorded life at San Simeon for posterity.
    berlitz2/Berlin-History.txt:With the Soviet army already in place, American troops entered Berlin in 1945 on their national Independence Day, 4 July, followed by the British and French contingents. Four-power control of Berlin was agreed at Potsdam by Winston Churchill (replaced in mid-conference by Clement Attlee, his successor as Prime Minister), Harry Truman, and Joseph Stalin. The Soviet eastern sector covered just under half the city’s area.
    berlitz2/Bahamas-WhereToGo.txt:The oldest wooden house on the island — it was built by shipwrights around 1790 of American soft cedar — it has been restored and is now a museum that offers a delightful view of life in well-to-do Nassau in the 18th century. Once a private home visited by the likes of the Duke of Windsor and Winston Churchill, Graycliff Mansion on West Hill Street is now a fine hotel with a well regarded menu and wine list. 

The command above searches through the berlitz2 subdirectory for any file that mentions the specified string. This could be helpful if you wanted to search broadly for files that mention Winston Churchill. 

    grep -r "dilemmas that today’s parents face" Berk
    
    Berk/ch7.txt:In this chapter, I take up dilemmas that today’s parents face in rearing young children. Throughout this book, we have touched on myriad forces that make contemporary parenting highly challenging. These include one-sided, contradictory messages in the parenting-advice literature; career pressures that impinge on parent involvement in children’s lives; abysmally weak American child-care services to assist employed parents in their child-rearing roles; cultural violence and excessive materialism permeating children’s worlds; schools with less than optimal conditions for children’s learning; and impediments to granting children with deﬁcits and disabilities social experiences that maximize their development.
    
The command above searches through the Berk subdirectory for any file that mentions the specified phrase. This could be helpful if you wanted to see in which chapter that "the dilemmas that today's parents face" is mentioned. In this case we learned that it is the topic of chapter 7.

This command was found on the site [swcarpentry](https://swcarpentry.github.io/shell-novice/07-find/index.html#:~:text=The%20grep%20command%20searches%20through).

## grep -o

grep -o returns only the matched parts of a matchine line, with each match on a separate line

    grep -o Polynesian HistoryHawaii.txt 
    
    Polynesian
    Polynesian
    Polynesian
    Polynesian
    
The above command searches through HistoryHawaii.txt to find the matching lines of the specified word. This can be useful to check if you were searching through your own file and wanted to check if you capitlized the word Polynesian appropriately each time. 

    grep -r -o sunlight Kauffman
    
    Kauffman/ch3.txt:sunlight
    Kauffman/ch3.txt:sunlight
    Kauffman/ch3.txt:sunlight
    Kauffman/ch3.txt:sunlight
    Kauffman/ch3.txt:sunlight
    Kauffman/ch4.txt:sunlight
    Kauffman/ch9.txt:sunlight
    
The above command searches recursively through the Kauffman subdirectory for files that match the specified word. This could be useful if you wanted to know which files mention the word sunlight in addition to the frequeny at which they do so. 

This command was found on the site [GeeksforGeeks](https://www.geeksforgeeks.org/grep-command-in-unixlinux/).
    
    
