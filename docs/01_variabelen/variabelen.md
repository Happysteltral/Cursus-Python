# Hoofdstuk 1 – Variabelen in Python

## 🎯 Leerdoelen

Na dit hoofdstuk kan je:

* uitleggen wat een variabele is
* een variabele correct aanmaken in Python
* variabelen gebruiken in berekeningen en tekst
* veelgemaakte fouten met variabelen herkennen

---

## 1️⃣ Wat is een variabele?

Stel je voor dat je een **doos** hebt met een **label** erop.
In die doos zit een waarde.

* 📦 doos = plaats in het geheugen van de computer
* 🏷️ label = naam van de variabele
* 🔢 inhoud = de waarde

In Python noemen we zo’n gelabelde doos een **variabele**.

👉 **Definitie**
Een *variabele* is een naam die verwijst naar een waarde die de computer bijhoudt.

---

## 2️⃣ Een eerste variabele maken

In Python maak je een variabele zo:

```python
leeftijd = 16
```

Wat gebeurt hier?

* `leeftijd` → naam van de variabele
* `=` → toekenning ("krijgt de waarde")
* `16` → de waarde

🧠 Lees dit als:

> *leeftijd krijgt de waarde 16*

---

## 3️⃣ Variabelen gebruiken

Je kan een variabele gebruiken in berekeningen:

```python
leeftijd = 16
volgend_jaar = leeftijd + 1
print(volgend_jaar)
```

👉 Uitvoer:

```
17
```

De computer **onthoudt** dus de waarde van `leeftijd`.

---

## 4️⃣ Variabelen en tekst (strings)

Niet alle variabelen zijn getallen. Je kan ook **tekst** opslaan.

```python
naam = "Alex"
print(naam)
```

⚠️ Let op:

* Tekst staat **altijd tussen aanhalingstekens** (`" "` of `' '`)
* Zonder aanhalingstekens denkt Python dat het een variabele is

Fout voorbeeld:

```python
naam = Alex   # ❌ fout
```

---

## 5️⃣ Verschillende soorten variabelen (datatypes)

| Type    | Voorbeeld           | Betekenis        |
| ------- | ------------------- | ---------------- |
| `int`   | `leeftijd = 16`     | geheel getal     |
| `float` | `prijs = 12.5`      | kommagetal       |
| `str`   | `naam = "Alex"`     | tekst            |
| `bool`  | `is_student = True` | waar / niet waar |

💡 Python kiest automatisch het juiste type.

---

## 6️⃣ Variabelen overschrijven

Een variabele kan **veranderen**:

```python
score = 10
score = 15
print(score)
```

👉 Uitvoer:

```
15
```

⚠️ De oude waarde (10) is weg.

---

## 7️⃣ Regels voor variabelenamen

✅ Wel toegelaten:

```python
leeftijd
studentNaam
score_1
```

❌ Niet toegelaten:

```python
1score      # begint met cijfer
voornaam!  # speciaal teken
for         # gereserveerd woord
```

📌 Tips:

* gebruik **duidelijke namen**
* schrijf in **kleine letters**
* gebruik `_` voor leesbaarheid

---

## 8️⃣ Variabelen en input van de gebruiker

Je kan een waarde vragen aan de gebruiker:

```python
naam = input("Wat is je naam? ")
print(naam)
```

⚠️ Alles wat je via `input()` krijgt is **tekst** en dus van het type **string**.

Voor getallen:

```python
leeftijd = int(input("Wat is je leeftijd? "))
```

---

## 🧠 Test jezelf

Wat doet deze code?

```python
x = 5
y = x + 3
x = 10
print(y)
```

➡️ Antwoord: `8`

---

## ✍️ Oefeningen

### Oefening 1 – Basis

Maak een variabele `voornaam` en print deze.

---

### Oefening 2 – Rekenen

* Maak een variabele `breedte`
* Maak een variabele `hoogte`
* Bereken de oppervlakte

---

### Oefening 3 – Input

Vraag de leeftijd van de gebruiker en print:

> "Volgend jaar ben je ... jaar"

---

## 🚀 Mini-uitdaging (optioneel)

Vraag de naam en leeftijd van de gebruiker en print:

> "Hallo Alex, jij bent 16 jaar."

---

## 📌 Samenvatting

* Een variabele bewaart een waarde
* Je maakt ze met `=`
* Python kiest automatisch het type
* Goede namen maken je code leesbaar

➡️ In het volgende hoofdstuk leren we **rekenen en expressies** met variabelen.
