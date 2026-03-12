# Hoofdstuk 6 -- Functies in Python

## 🎯 Wat leer je in dit hoofdstuk?

-   Wat een functie is
-   Waarom functies belangrijk zijn
-   Hoe je een functie definieert
-   Wat parameters zijn
-   Wat een returnwaarde is
-   Het verschil tussen lokale en globale variabelen

------------------------------------------------------------------------

## 1️⃣ Waarom functies gebruiken?

Stel dat je meerdere keren dezelfde berekening nodig hebt in je
programma.\
Zonder functies moet je telkens dezelfde code opnieuw schrijven.

Dat is:

-   ❌ Onoverzichtelijk\
-   ❌ Gevoelig voor fouten\
-   ❌ Moeilijk aan te passen

Met functies kan je:

-   ✅ Code hergebruiken\
-   ✅ Je programma overzichtelijk maken\
-   ✅ Grote problemen opsplitsen in kleine stukjes

!!! note Een functie is een **stukje code met een naam** dat je kan
oproepen wanneer je het nodig hebt.

------------------------------------------------------------------------

## 2️⃣ Een eerste functie

### 🔹 Structuur

``` python
def naam_van_de_functie():
    # code die uitgevoerd wordt
```

### 🔹 Voorbeeld

``` python
def begroet():
    print("Hallo leerling!")
```

Deze functie doet nog niets zolang we ze niet oproepen.

### 🔹 Functie oproepen

``` python
begroet()
```

Volledig programma:

``` python
def begroet():
    print("Hallo leerling!")

begroet()
```

!!! example Wat wordt er geprint als je `begroet()` drie keer onder
elkaar zet?

------------------------------------------------------------------------

## 3️⃣ Functies met parameters

``` python
def begroet(naam):
    print("Hallo", naam)
```

Gebruik:

``` python
begroet("Nicky")
begroet("Sarah")
```

!!! note Een parameter is een variabele die tijdelijk bestaat binnen de
functie.

------------------------------------------------------------------------

## 4️⃣ Meerdere parameters

``` python
def som(a, b):
    print(a + b)

som(3, 5)
```

!!! tip De volgorde van de parameters is belangrijk!

------------------------------------------------------------------------

## 5️⃣ Returnwaarde

``` python
def som(a, b):
    return a + b
```

Gebruik:

``` python
resultaat = som(4, 6)
print(resultaat)
```

!!! important `return` geeft een waarde terug en stopt onmiddellijk de
functie.

------------------------------------------------------------------------

## 6️⃣ Print vs Return

### ❌ Met print

``` python
def som(a, b):
    print(a + b)
```

### ✅ Met return

``` python
def som(a, b):
    return a + b
```

------------------------------------------------------------------------

## 7️⃣ Lokale en globale variabelen

``` python
def test():
    x = 5
    print(x)

test()
```

!!! warning Variabelen die in een functie gemaakt worden, bestaan alleen
binnen die functie.

------------------------------------------------------------------------

# 💻 Oefeningen

## Oefening 1 -- Vierkant berekenen

Schrijf een functie `vierkant(getal)` die het kwadraat teruggeeft.

## Oefening 2 -- Celsius naar Fahrenheit

F = C \* 9/5 + 32

Maak een functie `naar_fahrenheit(celsius)`.

## Oefening 3 -- Grootste van twee getallen

Maak een functie `grootste(a, b)` die het grootste getal teruggeeft.

## Oefening 4 -- Gemiddelde van drie getallen

Maak een functie die het gemiddelde teruggeeft van drie getallen.

------------------------------------------------------------------------

## 🚀 Uitdaging

Maak een functie `is_even(getal)` die True teruggeeft als het getal even
is.
