# Stap 1 – Variabelen in Python

## 1.1 Wat is een variabele?

!!! note "Concept"
    Een **variabele** is een naam die verwijst naar een waarde die in het geheugen wordt opgeslagen.
    
    Je kan het zien als een **doosje met een label**:
    - het label = de naam van de variabele
    - de inhoud = de waarde

Voorbeeld:

```python
leeftijd = 16
```

Hier maken we een variabele met de naam `leeftijd` en geven we die de waarde `16`.

---

## 1.2 Waarom gebruiken we variabelen?

!!! info
    Variabelen maken je programma:
    - leesbaarder
    - flexibeler
    - makkelijker aan te passen

Vergelijk:

```python
print(16)
```

met:

```python
leeftijd = 16
print(leeftijd)
```

👉 In het tweede voorbeeld is meteen duidelijk **wat** die 16 betekent.

---

## 1.3 Namen van variabelen

!!! tip "Goede gewoontes"
    - Gebruik duidelijke namen
    - Start met een kleine letter
    - Gebruik geen spaties
    - Gebruik `_` als scheiding

Voorbeelden:

```python
naam = "Alex"
geboortejaar = 2008
is_ingelogd = True
```

!!! warning "Let op"
    Deze namen zijn **fout of slecht gekozen**:

    ```python
    2naam = "Alex"   # mag niet starten met een cijfer
    mijn naam = "Alex"  # spaties zijn niet toegelaten
    print = 5         # overschrijft een Python-functie
    ```

---

## 1.4 Waarden aanpassen

Een variabele kan tijdens het uitvoeren van het programma **van waarde veranderen**.

```python
score = 10
print(score)

score = 15
print(score)
```

👉 De **laatste toekenning** telt.

---

## 1.5 Soorten waarden (datatypes)

!!! note "Belangrijk"
    Python bepaalt automatisch het **datatype** van een variabele.

| Type | Voorbeeld | Betekenis |
|----|----|----|
| `int` | `10` | geheel getal |
| `float` | `3.14` | kommagetal |
| `str` | `"Hallo"` | tekst |
| `bool` | `True`, `False` | waar / onwaar |

Voorbeelden:

```python
aantal = 5
prijs = 2.5
naam = "Sam"
is_geldig = True
```

---

## 1.6 Afdrukken met `print()`

!!! example "Voorbeeld"
    ```python
    naam = "Alex"
    leeftijd = 16
    print(naam)
    print(leeftijd)
    ```

!!! tip
    Gebruik `print()` vaak tijdens het programmeren om te zien wat je code doet.

---

## 1.7 Veelgemaakte fouten

!!! warning
    - Variabele gebruiken zonder ze eerst te maken
    - Namen door elkaar gebruiken (`Leeftijd` ≠ `leeftijd`)
    - Denken dat een variabele haar oude waarde onthoudt na overschrijven

---

## 1.8 🧠 Test jezelf

??? question "Wat doet deze code?"
    ```python
    x = 3
    y = x
    x = 7
    print(y)
    ```

    ??? success "Toon antwoord"
        **Antwoord:** `3`

        `y` krijgt de waarde van `x` op het moment van toekennen.
        De latere wijziging van `x` heeft geen invloed meer op `y`.

---

## 1.9 Oefeningen

### Oefening 1
Maak een variabele `naam` en geef ze je voornaam. Druk deze af.

### Oefening 2
Maak een variabele `leeftijd` en druk af:
> Ik ben ___ jaar oud

### Oefening 3
Maak twee variabelen en verwissel hun waarden.

---

## 1.10 Samenvatting

!!! summary
    - Een variabele slaat een waarde op
    - Je gebruikt `=` om een waarde toe te kennen
    - Python bepaalt automatisch het datatype
    - De laatste toekenning telt

---

➡️ **Volgende stap:** expressies en berekeningen

