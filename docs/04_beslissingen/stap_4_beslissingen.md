# Stap 4 – Beslissingen nemen met `if`, `elif` en `else`

## 4.1 Waarom beslissingen nemen?
Tot nu toe voert ons programma **altijd dezelfde stappen** uit. Slimme programma’s kunnen echter:
- situaties **vergelijken**
- **keuzes maken** op basis van voorwaarden

👉 In deze stap leert je programma **denken in ja/nee-vragen**.

Voorbeeld uit het echte leven:
> Als het regent → neem een paraplu
> Anders → geen paraplu nodig

---

## 4.2 De `if`-structuur

### 4.2.1 Basisvorm

```python
leeftijd = 18

if leeftijd >= 18:
    print("Je bent meerderjarig")
```

🔹 De voorwaarde moet **waar (`True`) of onwaar (`False`)** zijn.
🔹 De dubbele punt `:` is verplicht.
🔹 De code **onder de if** moet ingesprongen zijn (indentatie).

---

## 4.3 Vergelijkingsoperatoren

| Operator | Betekenis |
|--------|----------|
| `==` | gelijk aan |
| `!=` | niet gelijk aan |
| `>` | groter dan |
| `<` | kleiner dan |
| `>=` | groter of gelijk |
| `<=` | kleiner of gelijk |

Voorbeeld:
```python
score = 12
if score >= 10:
    print("Geslaagd")
```

---

## 4.4 `else` – wat als de voorwaarde niet klopt?

```python
leeftijd = 15

if leeftijd >= 18:
    print("Je bent meerderjarig")
else:
    print("Je bent minderjarig")
```

👉 `else` wordt uitgevoerd **als de if-voorwaarde onwaar is**.

---

## 4.5 Meerdere keuzes met `elif`

```python
score = 14

if score >= 16:
    print("Zeer goed")
elif score >= 12:
    print("Goed")
elif score >= 10:
    print("Voldoende")
else:
    print("Onvoldoende")
```

🔹 `elif` = *else if*
🔹 Python test de voorwaarden **van boven naar beneden**

---

## 4.6 Combineren met input

```python
leeftijd = int(input("Wat is je leeftijd? "))

if leeftijd < 12:
    print("Kind")
elif leeftijd < 18:
    print("Jongere")
else:
    print("Volwassene")
```

---

## 4.7 Logische operatoren

Je kan voorwaarden combineren met:

| Operator | Betekenis |
|--------|----------|
| `and` | en |
| `or` | of |
| `not` | niet |

Voorbeeld:
```python
leeftijd = 17
heeft_toestemming = True

if leeftijd < 18 and heeft_toestemming:
    print("Je mag mee op uitstap")
```

---

## 4.8 Veelgemaakte fouten

| Fout | Uitleg |
|----|------|
| `=` gebruiken i.p.v. `==` | `=` is toekennen, `==` vergelijken |
| Verkeerde indentatie | Python is hier streng in |
| Voorwaarden in verkeerde volgorde | Eerst meest specifieke testen |

---

## 4.9 Oefeningen

### Oefening 1 – Even of oneven
Vraag een getal en toon of het **even of oneven** is.

---

### Oefening 2 – Punten
Vraag een score op 20 en toon:
- Geslaagd (≥ 10)
- Niet geslaagd (< 10)

---

### Oefening 3 – Leeftijdscategorie
Vraag de leeftijd en toon:
- kind
- jongere
- volwassene

---

### Oefening 4 – Mini-project
Maak een programma dat:
1. een wachtwoord vraagt
2. controleert of het gelijk is aan een vast wachtwoord
3. een correcte of foute melding toont

---

## 4.10 Samenvatting

- `if` controleert een voorwaarde
- `else` vangt het andere geval op
- `elif` laat meerdere keuzes toe
- Voorwaarden gebruiken vergelijkingsoperatoren
- Correcte indentatie is cruciaal

---

➡️ **Volgende stap:** herhaling met lussen (`while` en `for`)

