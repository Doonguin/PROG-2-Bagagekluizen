# PROG-2-Bagagekluizen
Op veel stations kun je een bagagekluis huren. We willen graag dat jij de software realiseert voor de verhuur van de kluizen. Er zijn door de beheerders de volgende randvoorwaarden gesteld aan het systeem:

- Er zijn in totaal 12 kluizen (nr. 1 t/m 12).
- Elke kluis moet beveiligd zijn met een code (minimaal 4 tekens, en GEEN ';') die de klant zelf bedenkt.
- Als de stroom uitvalt mag de data niet verloren gaan en daarom moet je een bestand gebruiken voor de opslag van gegevens zoals kluisnummers en wachtwoorden.

Een voorbeeld van zo’n bestand (bijv. ‘kluizen.txt’) zie je hieronder:
```
11;6754 
1;geheim 
5;kluisvanpietje 
12;z@terd@g 
```
In het voorbeeld zijn er 4 kluizen in gebruik (nummer 11, 1, 5 en 12). Het nummer wordt gevolgd door een puntkomma, waarachter de code staat die de gebruiker heeft ingevoerd voor de betreffende kluis. Op elke regel staat informatie van maximaal 1 kluis! Let op: kluizen die niet in gebruik zijn, staan NIET in het bestand!

Als je programma start, moet je het onderstaande menu te zien krijgen:
```
1: Ik wil weten hoeveel kluizen nog vrij zijn 
2: Ik wil een nieuwe kluis 
3: Ik wil even iets uit mijn kluis halen 
4: Ik geef mijn kluis terug
```
Schrijf voor elke menukeuze een functie die het echte werk doet. Voor...

- ... optie 1: def ```aantal_kluizen_vrij();``` de returnwaarde van de functie is een int met het aantal beschikbare kluizen.
- ... optie 2: def ```nieuwe_kluis();``` indien er nog kluizen vrij zijn, kan de gebruiker een zelfgekozen, geldige, code invoeren. In dat geval wordt de code automatisch gekoppeld aan een vrij kluisnummer. De returnwaarde is het gekoppelde kluisnummer.  Als de code ongeldig is, is de returnwaarde -1. Als er geen kluizen beschikbaar zijn is de returnwaarde -2.
- ... optie 3: def ```kluis_openen();``` hier moet EERST een kluisnummer en DAARNA de code ingevoerd worden. Is de combinatie correct, dan is de returnwaarde True, anders False.
- ... optie 4: def ```kluis_teruggeven();``` hier moet EERST een kluisnummer en DAARNA de code ingevoerd worden. Is de combinatie correct, dan wordt de kluis weer vrijgegeven, en is de returnwaarde True, anders False. Deze menukeuze is optioneel!

Geef op basis van de returnwaarde van de functie een nette melding aan de gebruiker.