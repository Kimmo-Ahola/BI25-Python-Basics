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

Slå av Copilot i VSCode för dessa uppgifter. Många av dessa övningar kräver google. Googla först, ChatGPT sist.

## Variabler, Typer & Print

Skapa ex_variables.py för dessa uppgifter.

1. Skapa variablerna name och age och skriv ut till konsolen: "Hej, jag heter [name] och är [age] år gammal".
2. Konvertera strängen "1500" till ett heltal och addera 500.
3. Skapa en variabel med värdet 3.14159. Skriv ut den avrundad till två decimaler.
5. Skapa en variabel för price och quantity. Beräkna total och skriv ut med f-string.
6. Kontrollera vilken datatyp variabeln x = "10" är. Googla på check data type Python.
7. Skapa en variabel is_active = True. Skriv ut den som en sträng.
8. Slå ihop två strängar: "Business" och "Intelligence" med ett mellanslag mellan.
9. Vad händer om du försöker att summera en sträng med en siffra och kör ditt script? Vad står det i terminalen?

---

## Jämförelser

Skapa ex_comparisons.py för dessa uppgifter.

1. Jag anser att 0.1 + 0.2 = 0.3 men vad tycker Python om detta? Testa att skriva ut till konsolen och ta reda på varför det är så.
2. För att jämföra om två tal är lika använder vi oss av ==. Detta fungerar utan problem för heltal men ta reda på hur man måste göra när det kommer till flyttal.

3. Fundera på koden nedan och vad den kommer att skriva ut innan du kör den. Hade du rätt?

```Python

if 5 > 4:
    print("Five is larger than 4")

```

Fundera på koden nedan och vad den kommer att skriva ut innan du kör den. Varför är det så?

```
if 5:
    print("Five is?")
else:
    print("This should be printed")

if "":
    print("Empty string is?")
else:
    print("This should not be printed?")
```

4. Fundera på denna kod och varför den beter sig som den gör

```Python
x = "A"
y = "A"
a = [1, 2, 3] # list of 1, 2 and 3
b = [1, 2, 3] # list of 1, 2 and 3

print("a == b", a == b) # this prints what?
print("x is y", x is y) # this prints what?
print("a is b", a is b) # this prints what?
```

---

## Logik (If/Elif/Else)

Skapa ex_if_else.py för dessa uppgifter.

1. Kolla om ett tal är positivt, negativt eller noll och skriv ut till konsolen.
3. Skapa en "Rabatt-kalkylator" som kollar en variabel: Om variabeln > 1000 kr, dra av 10% rabatt.
4. Kolla om ett tal är jämnt eller udda.
5. Skapa en betygsättare som skriver ut bokstaven inom parentes till konsolen: 0-49 (F), 50-74 (G), 75-100 (VG). Vad händer med tal under 0 och tal större än 100?
6. Kolla om en sträng innehåller mer än 10 tecken.
7. Skriv en logisk sats som kollar om ett tal är mellan 10 OCH 20.
8. Kolla om en variabel x är av typen int. Skriv ut True till konsolen om den är det.

---

## Listor

Skapa ex_lists.py för dessa uppgifter.

1. Skapa en lista med fem städer. Skriv ut den tredje staden i listan.
2. Lägg till en stad i slutet av din lista med och ta bort den första staden från listan.
3. Byt ut den första staden i listan mot "Stockholm".
4. Ta bort den sista staden i listan med.
5. Skapa en lista med siffror och skriv ut listans längd.
7. Skapa en lista colors som du fyller med färger. Kolla om "Blue" finns i listan.
8. Skapa en lista av listor och försök att hämta ett värde ur en nästlad lista.

---

## Loopar

Skapa ex_loops.py för dessa uppgifter.

1. Ta reda på vilka loop-typer som är vanligast i Python.
1. Skriv ut talen 1 till 10 med en lämplig loop.
2. Loopa igenom en lista med namn och skriv ut "Välkommen [namn]" om namnet finns i listan. Om namnet förekommer flera gånger ska det bara skrivas ut en gång.
3. Summera alla tal i en lista med hjälp av en loop. Testa sedan att lägga till en sträng i listan och att summera igen. Vad händer?
4. Skapa en loop som bara skriver ut jämna tal mellan 1 och 20.
5. Avbryt en loop när den når talet 7.
6. Skriv kod som hoppar över siffran 5 i en loop 1-10.
7. Skapa en lista med priser. Loopa och skapa en ny lista där varje pris har fått 25% moms pålagt.
8. Skapa en "Nedräknare" som räknar från 10 till 1.
9. Googla på om det finns något sätt att göra en lista i omvänd ordning.
10. Läs följande kod och fundera på vad som kommer att skrivas ut:
```Python
x = "My Name is"

for y in x:
    print(y)
```

Kör sedan koden och ta reda på varför den skrev ut resultatet på det sättet.

---

## Funktioner & Scope

Skapa ex_func_scope.py för dessa uppgifter.

1. Skriv en funktion say_hi() som skriver ut "Hej!".
2. Skriv en funktion som tar base och height och returnerar arean på en triangel.
3. Skapa en funktion som tar en lista och returnerar det största talet.
5. Skriv en funktion som kollar om en e-postadress innehåller ett "@".
7. Skriv en funktion som tar en sträng och returnerar den baklänges.
8. Skapa en funktion calculate_tax som anropar en annan funktion get_tax_rate internt.

Scope i Python kan vara lurigt. Testa dessa exempel, ett i taget, och se vad ni får utskriver till konsolen.
```Python
x = "Kimmo"

if True:
    x = "Orange"

print(x)
```

```Python
x = "Kimmo"

def test():
    x = "Orange"

print(x)
```

```Python
x = "Kimmo"

def test():
    y = "Orange"
    return y

y = test()
x = y
print(x)
```

```Python
def test():
    x = "Kimmo"
    return "Orange"

print(test())
print(x)
```

---

## Att googla på

I SQL är ni vana vid kolumnnamn men i Python använder vi ofta Dictionaries för att mappa data.
1. Vad är dictionaries?
2. Hur fungerar de rent konceptuellt?
3. Hur sparas en dictionary i ett Python-script?
4. Vad är skillnaden på en dictionary och JSON?

---

I SQL använder vi ofta oss av like '%something%' eller '__ab%' för att hitta mönster i strängar. Hur ska vi göra om vi ska söka på mer avancerade mönster?
Fundera på:
1. Hur ska vi till exempel ta bort whitespace (mellanslag) i början och i slutet av strängar?
2. Hur ska vi dela upp en sträng till ett antal ord? "Jag heter Kimmo" -> Ska resultera i tre ord. Hur gör vi detta och hur kan vi spara dessa tre ord på ett smidigt sätt?
3. Hur kan jag kolla om en sträng innehåller ett specifikt tecken, till exempel ett @, och sedan sparar detta tecken och ingenting annat till en variabel?
4. Hur kan jag kolla om en sträng innehåller ett mer avancerat mönster, till exempel (ett till tre siffror)-(en siffra)-(@ eller , eller .)

```
Giltiga:
123-1-@
1-1-@
12-1-.

Ogiltiga:
1234-1-@ <- Får inte ha fler än 3 siffror i första delen
123-1-@, <- Får inte sluta med @ och , utan bara en av dem.
```

Vi måste hitta på något nytt nästa vecka för att kunna extrahera mönster från textsträngar.
