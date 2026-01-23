# Stap 2 – Expressies en berekeningen in Python

## 🎯 Doel van deze stap
Na deze stap kan je:
- uitleggen wat een **expressie** is
- berekeningen maken met variabelen
- de **volgorde van bewerkingen** correct toepassen
- expressies combineren met input en output

🧠 **Denkidee van deze stap**  
> *Ik kan waarden combineren en ermee rekenen.*

---

## 0️⃣ Overzicht

In de vorige stap leerde je **waarden opslaan** in variabelen.  
Nu gaan we die waarden **gebruiken**.

👉 Dat doen we met **expressies**.

---

## 1️⃣ Wat is een expressie?

Een **expressie** is een stukje code dat door Python wordt **uitgerekend**.

Voorbeelden van expressies:
```python
5 + 3
leeftijd + 1
prijs * aantal
```

👉 Python vervangt een expressie altijd door **één resultaat**.

---

## 2️⃣ Rekenen met getallen

Python kan rekenen zoals een rekenmachine.

```python
print(10 + 5)
print(10 - 5)
print(10 * 5)
print(10 / 5)
```

👉 Uitvoer:
```
15
5
50
2.0
```

⚠️ Let op: delen (`/`) geeft altijd een **kommagetal**.

---

## 3️⃣ Rekenen met variabelen

Je kan variabelen gebruiken in expressies:

```python
breedte = 5
hoogte = 3
oppervlakte = breedte * hoogte
print(oppervlakte)
```

🧠 Python kijkt eerst naar de **waarden**, niet naar de namen.

---

## 4️⃣ Expressies opslaan in variabelen

Het resultaat van een expressie kan je opslaan:

```python
a = 10
b = 4
c = a + b
print(c)
```

👉 `a + b` is een expressie
👉 `c` bewaart het resultaat

---

## 5️⃣ Volgorde van bewerkingen

Python volgt dezelfde regels als in de wiskunde:

1. haakjes `()`
2. vermenigvuldigen en delen `* /`
3. optellen en aftrekken `+ -`

Voorbeeld:
```python
resultaat = 10 + 2 * 3
print(resultaat)
```

👉 Uitvoer:
```
16
```

Met haakjes:
```python
resultaat = (10 + 2) * 3
print(resultaat)
```

👉 Uitvoer:
```
36
```

---

## 6️⃣ Expressies en input

Je kan input combineren met berekeningen:

```python
leeftijd = int(input("Wat is je leeftijd? "))
volgend_jaar = leeftijd + 1
print(volgend_jaar)
```

⚠️ Vergeet `int()` niet, anders kan Python niet rekenen.

---

## 7️⃣ Veelgemaakte fouten

### ❌ Tekst + getal combineren

```python
leeftijd = 16
print("Je bent " + leeftijd)
```

👉 FOUT

✔️ Correct:
```python
print("Je bent", leeftijd)
```

---

### ❌ Verkeerde volgorde

```python
resultaat = 10 + 2 * 5
```

👉 Verwacht je 60? Dan moet je haakjes gebruiken.

---

## 🧠 Test jezelf
Wat wordt er geprint?

```python
x = 4
y = 2
z = x * y + 1
print(z)
```

➡️ Antwoord: `9`

---

## ✍️ Oefeningen

### Oefening 1 – Basis
Bereken de som van twee getallen en print het resultaat.

---

### Oefening 2 – Oppervlakte
Vraag de breedte en hoogte van een rechthoek en bereken de oppervlakte.

---

### Oefening 3 – Leeftijd
Vraag de leeftijd van de gebruiker en print hoe oud hij/zij volgend jaar is.

---

## 🚀 Mini-toepassing

Maak een programma dat:
- de prijs van één product vraagt
- het aantal vraagt
- de totale prijs berekent

Voorbeeld uitvoer:
> Totale prijs: 24 euro

---

## 📌 Samenvatting
- Een expressie wordt **uitgerekend** door Python
- Je kan expressies opslaan in variabelen
- Python volgt vaste rekenregels
- Haakjes maken je code duidelijk

➡️ In de volgende stap leren we **input en output** uitgebreider gebruiken.

