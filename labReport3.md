# Researching the Grep Command 

## grep -w 

grep -w returns matches to word boundaries

    grep -w "fun" Costa-WhatToDo.txt
    
    Alternative diversions for children include the aquariums in Benalmádena and Puerto Banús, the Eagle Park in Benalmádena, the Cueva (cave) De Nerja, and Mini- Hollywood near Almería. In the evenings, Tívoli World near Benalmádena provides all the fun of the fair, with carnival rides and a roller coaster, and there’s also a bar and flamenco show for the grown-ups. The Crocodile Park just north of Málaga will intrigue most children, as will the horse shows of El Ranchito in Benalmádena and Aires del Sur in Estepona.
    
The command above is searching through the Costa-WhatToDo.txt file for text that appears near the word "fun". This can be useful if you are strictly looking for what the author describes as fun things to do in Costa del Sol. 

    grep -w habitually chM.txt
    
    Death, personified as a woman and dressed in white clothing, is a well-known character in Chicano and Mexicano folklore. Commonly accepted as just La Muerte, she is a frequent personality in legends, urban belief tales, and is integrated into many family folk belief systems. Death is sometimes feared, but it is also accepted as the transition to another stage of the life cycle. A common saying is “De la muerte y la suerte nadie se escapa” (No one escapes from death or luck) (Espinosa, A. M., 1910, 404). She habitually appears late at night, to men who are out alone, some intentionally, others innocently on their way home from work. In tales collected in the Southwest, La Muerte is seen standing at streetlights, or waiting by a bridge or the side of the road.
    
The command above is searching through chM.txt for text that appears near the word "habitually". This could be useful if you remember that word "habitually" being related to a section of the text that talks about something specific you are looking for. 
    
This command was found on a GitHub site called [swcarpentry](https://swcarpentry.github.io/shell-novice/07-find/index.html#:~:text=The%20grep%20command%20searches%20through).
