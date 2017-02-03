# Scratch - trollkarlen Ash

Hjälp trollkarlen Ash i kampen mot dom onda Moorgerna. Skapa egna trollformler och visa hur man undviker fiender. 
Vi lär oss mer om animation, gravitation, kloner och variabler.

Utveckling: https://scratch.mit.edu/users/Ratcher05/

Grafik: https://scratch.mit.edu/users/MaEk_Animations/

## Förberedelser
* Hitta igen följande project och spara ner alla sprites i din ryggsäck: https://scratch.mit.edu/projects/142913300/
* Skapa ett nytt projekt. 
* Rensa bort katten
* Skapa en bakgrund som är lik nedanstående. Det viktiga är att marken är i en färg och himlen en annan:

![Background](images/background.png "Bakgrund")

## Ash

### Lägg till Ash
* Flytta in Ash från ryggsäcken till ditt projekt
* Ställ Ash på marken (dra ner Ash tills hen står på marken och titta vilken y-koordinat som då anges i fönstret):

![Ash ground](images/ash_groundnew.png "Ash ground")

### Få Ash att gå vänster och höger
Vi gör så att Ash kan röra sig över skärmen.

![Ash walk](images/ash_walknew.png "Ash walk")

Finns det andra sätt man kunde ha löst det på? Vad hade hänt om man gjort så här:

![Ash walk again](images/ash_walk2new.png "Ash walk again")

### Animera Ash
Vi gör så att figuren ser ut att gå över skärmen 

![Ash animate](images/ash_animate2new.png "Ash animate")

## Kasta besvärjelse
### Förberedelser
Flytta in den besvärlse du vill använda (hjärtat eller stjärnan) från ryggsäcken.


###Kasta besvärjelse version 1
När spelar trycker space så ska besvärlsen kastas mot muspekaren. Då besvärjelsen träffar kanten ska den försvinna
Se till att besvärjelsen alltid startar på samma plats som Ash och att den är gömd:

![Spell version 1](images/spell_version1.png "Spell version 1")

Problem: Det går bara att kasta en i taget!

###Kasta besvärjelse version 2
När spelar trycker space så ska en klon skapas av spriten.

![Spell version 2](images/spell_version2.png "Spell version 2")

Problem: När vi trycker på space flera ggr blir det för många besvärjelser.

###Kasta besvärjelse version 3
När vi trycker space, kolla om vi är en klon innan vi skapar en klon.

![Spell version 3](images/spell_version3.png "Spell version 3")

## Moorgerna kommer
### Förberedelser
Lägg in mark-moorgen i ditt projekt. Den som ser ut att ligga på marken.

Se till att det skapas en ny klon  vid slumpmässigt tillfälle
![Moorg Random](images/moorg_random.png "Moorg random")

### Moorg kommer version 1
* När jag startar som en klon. 
* Visa mig och lägg mig på i kanten på skärmen i höjd med marken. 
* Se till så att jag pekar in mot mitten av skärmen.
* Tills jag träffar Ash eller jag blir träffad av ett hjärta - repetera:
  * Flytta 10 steg i den riktning du pekar (mot mitten)
  * Repetera 4 ggr 
    * Nästa kostym
    * Vänta kort stund
  * Om vi träffar kanten, byt riktning
* Ta bort klonen
  
![Moorg walk 1](images/moorg_move_version1.png "Moorg walk 1")

### Moorg kommer version 2

* Välj ett slumpmässigt tal mellan 1 och 2. 
* Om det är 1, gör som vi gjorde innan.
* Om det är 2, se till att jag hamnar vid andra kanten och pekar mot mitten.

![Moorg walk 2](images/moorg_move_version2.png "Moorg walk 2")


### Moorg kommer version 3 
DRY - Don't repeat yourselves. (Refaktorering)

Flytta de delar som är lika i ett eget block.

* Skapa ett nytt block som heter MooveMoorg
* Flytta in allt från "repeat until"/"repetera till" i definitionen av det nya blocket.
* Lägg till det nya blocket.

![Moorg walk block](images/moorg_move_block.png "Moorg walk block")

![Moorg walk 3](images/moorg_move_version3.png "Moorg walk 3")








