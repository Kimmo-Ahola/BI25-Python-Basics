# BI25-Python-Basics
Första lektionen om Python för BI 25. Introduktion till Python från ett dataanalysperspektiv.

# Klona repo

För att klona detta repo klickar du på den gröna knappen "code" och kopierar länken.

1. I VSCode väljer du "Clone Git Repository" och väljer en lämplig mapp som inte befinner sig i Onedrive eller liknande.
2. I terminalen skriver du: `git remote remove origin`
4. Skapa ett eget repo på GitHub och kopiera länken som dyker upp
5. I terminalen skriver du `git remote add origin your-link-here`

Ditt repo är nu lokalt och kopplat till din egen GitHub och du kan pusha upp kod som du vill. Det rekommenderas att pusha upp efter varje löst uppgift för att öva på själva flödet.


# Fokus

Målen med dessa övningar är att ge Python-kunskap som fokuserar på dataanalys. Detta är helt annorlunda jämfört med applikationsutveckling i Python. Vi kommer därför idag **inte** att prata någonting om:

- Objektorienterad Programmering utöver att jag visar punktnotation
- Felhantering av användarinput
- Import mellan egna moduler
- Virtuella miljöer

Dagens fokus kommer istället att ligga på:

- Variabeldeklaration
- Pythons kodflöde i enkla scripts
- Scope
- Datastrukturer som är användbara för er:
    - Listor
    - Dictionaries
- Loopar och if/else
- Stränghantering
- Funktioner

Eftersom att ni tidigare har kodat en del i TSQL är ni redan bekanta med vissa programmeringstermer och kodflöde. Detta skiljer sig något i Python men mycket kan ni redan konceptuellt.


# Övningsuppgifter


## Variabler, Typer & Print

1. Skapa variabeln name och age och skriv ut: "Hej, jag heter [name] och är [age] år".
2. Konvertera strängen "1500" till ett heltal och addera 500.
3. Skapa en variabel med värdet 3.14159. Skriv ut den avrundad till två decimaler (tips: round()).
4. Ta emot ett namn via input() och skriv ut det i bara stora bokstäver.
5. Skapa en variabel för price och quantity. Beräkna total och skriv ut med f-string.
6. Kontrollera vilken datatyp variabeln x = "10" har med type().
7. Skapa en variabel is_active = True. Skriv ut den som en sträng.
8. Slå ihop två strängar: "Business" och "Intelligence" med ett mellanslag mellan.

---

## Logik (If/Elif/Else)

1. Kolla om ett tal är positivt, negativt eller noll.
2. Skriv en if-sats som kollar om en användare är "admin" för att få logga in.
3. Skapa en "Rabatt-kalkylator": Om köpet > 1000 kr, ge 10% rabatt.
4. Kolla om ett tal är jämnt eller udda (tips: % 2).
5. Skapa en betygsättare: 0-49 (F), 50-74 (G), 75-100 (VG).
6. Kolla om en sträng innehåller mer än 10 tecken.
7. Skriv en logisk sats som kollar om ett tal är mellan 10 OCH 20.
8. Kolla om en variabel x är av typen int.

---

## Listor

1. Skapa en lista med fem städer. Skriv ut den tredje staden.
2. Lägg till en stad i slutet av din lista med .append().
3. Byt ut den första staden i listan mot "Stockholm".
4. Ta bort den sista staden i listan med .pop().
5. Skapa en lista med siffror och skriv ut listans längd (len()).
6. Sortera en lista med osorterade tal.
7. Skapa en lista colors. Kolla om "Blue" finns i listan (använd in).
8. Skapa en lista av listor (en enkel matris) och hämta ett värde ur den inre listan.

---

## Loopar

1. Skriv ut talen 1 till 10 med en for-loop.
2. Loopa igenom en lista med namn och skriv ut "Välkommen [namn]".
3. Summera alla tal i en lista med hjälp av en loop.
4. Skapa en loop som bara skriver ut jämna tal mellan 1 och 20.
5. Avbryt en loop med break när den når talet 7.
6. Använd continue för att hoppa över siffran 5 i en loop 1-10.
7. Skapa en lista med priser. Loopa och skapa en ny lista där varje pris har fått 25% moms pålagt.
8. Skapa en "Nedräknare" som räknar från 10 till 1 (tips: range(10, 0, -1)).

---

## Funktioner & Scope

1. Skriv en funktion say_hi() som skriver ut "Hej!".
2. Skriv en funktion som tar base och height och returnerar arean på en triangel.
3. Skapa en funktion som tar en lista och returnerar det största talet.
4. Scope-test: Skapa en global variabel x. Försök ändra den inuti en funktion utan global och se vad som händer.
5. Skriv en funktion som kollar om en e-postadress innehåller ett "@".
6. Skapa en funktion med ett default-argument (t.ex. currency="SEK").
7. Skriv en funktion som tar en sträng och returnerar den baklänges.
8. Skapa en funktion calculate_tax som anropar en annan funktion get_tax_rate internt.
