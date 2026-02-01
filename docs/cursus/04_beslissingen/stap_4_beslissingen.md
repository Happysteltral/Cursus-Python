# Stap 4 – Beslissingen nemen met `if`, `elif` en `else`

## 4.1 Waarom beslissingen nemen?

!!! note "Concept"
    Met **beslissingen** kan een programma **verschillend gedrag vertonen** afhankelijk van een situatie.

In het echte leven:
- als het regent → paraplu
- anders → geen paraplu

👉 In Python doen we dit met `if`, `elif` en `else`.

---

## 4.2 De `if`-structuur

!!! example "Voorbeeld"
    ```python
    leeftijd = 18

    if leeftijd >= 18:
        print("Je bent meerderjarig")
    ```

!!! note "Belangrijk"
    - De voorwaarde moet `True` of `False` zijn
    - De dubbele punt `:` is verplicht
    - Alles onder de `if` moet **ingesprongen** zijn

---

## 4.3 Vergelijkingsoperatoren

!!! info
    Deze operatoren gebruik je in voorwaarden:

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

## 4.4 `else` – het andere geval

!!! example "Voorbeeld"
    ```python
    leeftijd = 15

    if leeftijd >= 18:
        print("Je bent meerderjarig")
    else:
        print("Je bent minderjarig")
    ```

!!! note
    `else` wordt uitgevoerd als de `if`-voorwaarde **onwaar** is.

---

## 4.5 Meerdere keuzes met `elif`

!!! example "Voorbeeld"
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

!!! tip
    Python test de voorwaarden **van boven naar beneden**.

---

## 4.6 Combineren met input

!!! example "Voorbeeld"
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

!!! info
    Je kan voorwaarden combineren:

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

!!! warning
    - `=` gebruiken in plaats van `==`
    - Verkeerde indentatie
    - Voorwaarden in foute volgorde testen

---

## 4.9 🧠 Test jezelf

??? question "Wat wordt er afgedrukt?"
    ```python
    x = 5

    if x > 10:
        print("A")
    elif x > 3:
        print("B")
    else:
        print("C")
    ```

    ??? success "Toon antwoord"
        **Antwoord:** `B`

        `x > 10` is onwaar, `x > 3` is waar.

---

## 4.10 Oefeningen

### Oefening 1 – Even of oneven
Vraag een getal en toon of het **even of oneven** is.

### Oefening 2 – Punten
Vraag een score op 20 en toon:
- Geslaagd (≥ 10)
- Niet geslaagd (< 10)

### Oefening 3 – Leeftijdscategorie
Vraag de leeftijd en toon:
- kind
- jongere
- volwassene

### Oefening 4 – Mini-toepassing
Maak een programma dat:
1. een wachtwoord vraagt
2. controleert of het correct is
3. een gepaste melding toont

---

## 4.11 Samenvatting

!!! summary
    - `if` test een voorwaarde
    - `else` vangt het andere geval op
    - `elif` laat meerdere keuzes toe
    - Correcte indentatie is cruciaal

---

➡️ **Volgende stap:** herhaling en lussen (`while` en `for`)

