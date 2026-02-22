# 🔁 Stap 5 --- Lussen (herhaling in Python)

!!! info In dit hoofdstuk leer je hoe je **code kan herhalen** zonder ze
meerdere keren te moeten schrijven.

------------------------------------------------------------------------

## 🎯 Wat ga je leren?

Na dit hoofdstuk kan je:

-   code **meerdere keren laten uitvoeren**
-   werken met een **`while` lus**
-   werken met een **`for` lus**
-   het verschil uitleggen tussen beide
-   eenvoudige herhalingsproblemen oplossen

------------------------------------------------------------------------

# 🔁 Waarom lussen?

Stel dat je de getallen van 1 tot 10 wil afdrukken.

Zonder lus zou je moeten schrijven:

``` python
print(1)
print(2)
print(3)
...
print(10)
```

❌ Dat is: - veel werk - foutgevoelig - niet flexibel

👉 Met een **lus** kan dit veel eenvoudiger.

------------------------------------------------------------------------

# 🔄 De `while` lus

Een **while-lus** herhaalt code **zolang een voorwaarde waar is**.

## 🧱 Structuur

``` python
while voorwaarde:
    # code die herhaald wordt
```

------------------------------------------------------------------------

## 📌 Voorbeeld 1 --- Tellen van 1 tot 5

``` python
teller = 1

while teller <= 5:
    print(teller)
    teller = teller + 1
```

------------------------------------------------------------------------

!!! warning Vergeet nooit je teller te verhogen!\
Anders blijft de voorwaarde **altijd waar** en krijg je een **oneindige
lus**.

------------------------------------------------------------------------

## 📌 Voorbeeld 2 --- Som berekenen

``` python
som = 0
getal = 1

while getal <= 5:
    som = som + getal
    getal = getal + 1

print(som)
```

------------------------------------------------------------------------

# 🔁 De `for` lus

Een **for-lus** gebruik je wanneer je **op voorhand weet hoeveel keer**
je wil herhalen.

## 🧱 Structuur

``` python
for variabele in range(start, stop):
    # code
```

------------------------------------------------------------------------

## 📌 Voorbeeld 1 --- Tellen van 1 tot 5

``` python
for i in range(1, 6):
    print(i)
```

------------------------------------------------------------------------

!!! note `range(1, 6)` betekent:\
van **1 tot 6, maar 6 zelf niet inbegrepen**

------------------------------------------------------------------------

## 📌 Voorbeeld 2 --- Tafel van 5

``` python
for i in range(1, 11):
    print(i, "x 5 =", i * 5)
```

------------------------------------------------------------------------

# ⚖️ While vs For

  Situatie                                    Beste keuze
  ------------------------------------------- -------------
  Je weet **hoeveel keer** je moet herhalen   `for`
  Je weet dat niet op voorhand                `while`

------------------------------------------------------------------------

# 🧠 Belangrijke begrippen

## 🔢 Teller

Een variabele die bijhoudt **hoeveel keer** iets gebeurt.

``` python
teller = teller + 1
```

------------------------------------------------------------------------

## ➕ Accumulator

Een variabele die een **totaal optelt**.

``` python
som = som + getal
```

------------------------------------------------------------------------

# 🧪 Test jezelf

## Vraag 1

Wat doet deze code?

``` python
for i in range(3):
    print("Hallo")
```

A. Het woord "Hallo" wordt 1 keer getoond\
B. Het woord "Hallo" wordt 3 keer getoond\
C. Het woord "Hallo" wordt 4 keer getoond

------------------------------------------------------------------------

## Vraag 2

Wat is de uitvoer?

``` python
teller = 0

while teller < 3:
    print(teller)
    teller = teller + 1
```

------------------------------------------------------------------------

## Vraag 3

Welke lus kies je?

Je wil een programma dat blijft vragen om een wachtwoord tot het correct
is.

-   ⬜ `for`
-   ⬜ `while`

------------------------------------------------------------------------

# 💡 Tips

!!! tip Gebruik **`for`** als je een **vaste reeks** hebt (zoals 1--10)

!!! tip Gebruik **`while`** als je werkt met **voorwaarden** (zoals
blijven vragen tot iets klopt)

!!! tip Geef duidelijke namen aan je variabelen (`teller`, `som`, ...)

------------------------------------------------------------------------

# 🚀 Samenvatting

In dit hoofdstuk leerde je:

-   🔁 hoe je code kan **herhalen**
-   🔄 werken met een **`while` lus**
-   🔁 werken met een **`for` lus**
-   🔢 het gebruik van een **teller**
-   ➕ het gebruik van een **accumulator**

👉 Lussen zijn één van de **belangrijkste bouwstenen** in programmeren.
