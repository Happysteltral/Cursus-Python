# Stap 3 – Input en output in Python

## 3.1 Wat is input en output?

!!! note "Concept"
    **Input** is informatie die het programma **ontvangt van de gebruiker**.
    **Output** is informatie die het programma **toont aan de gebruiker**.

Zonder input en output kan een programma niet communiceren.

---

## 3.2 Output tonen met `print()`

!!! example "Voorbeeld"
    ```python
    print("Hallo wereld")
    ```
    Deze code toont de tekst "Hallo wereld" op het scherm. Dit is het eerste programma dat veel mensen leren!

Je kan ook variabelen afdrukken:

```python
naam = "Alex"
leeftijd = 16
print(naam)
print(leeftijd)
```

---

## 3.3 Tekst en variabelen combineren

Je wilt vaak tekst en variabelen samen tonen. Bijvoorbeeld: "Ik ben 16 jaar".

✅ eerste manier:
```python
print("Ik ben", leeftijd, "jaar")
```

---

## 3.4 f-strings (aanbevolen)

!!! tip "Goede gewoonte"
    Gebruik **f-strings** om tekst en variabelen netjes te combineren. De f staat voor formatted (opgemaakt).

```python
print(f"Ik ben {leeftijd} jaar")
```

👉 Alles tussen `{ }` wordt automatisch omgezet naar tekst (string).

---

## 3.5 Input vragen met `input()`

!!! example "Voorbeeld"
    ```python
    naam = input("Wat is je naam? ")
    print(f"Hallo {naam}")
    ```

!!! note "Belangrijk"
    Alles wat met `input()` wordt ingevoerd is **altijd tekst (string)**.

---

## 3.6 Rekenen met input

!!! warning "Veelgemaakte fout"
    Je kan **niet rekenen met input** zonder omzetting.

❌ Fout:
```python
leeftijd = input("Wat is je leeftijd? ")
volgend_jaar = leeftijd + 1
```

✅ Correct:
```python
leeftijd = int(input("Wat is je leeftijd? "))
volgend_jaar = leeftijd + 1
print(f"Volgend jaar ben je {volgend_jaar} jaar")
```

---

## 3.7 Getallen omzetten

!!! info
    Gebruik deze "type casting" functies om tekst om te zetten:

| Functie | Resultaat |
|------|---------|
| `int()` | geheel getal |
| `float()` | kommagetal |
| `str()` | tekst |

Voorbeeld:
```python
prijs = float(input("Prijs? "))
```

---

## 3.8 🧠 Test jezelf

??? question "Wat gebeurt hier?"
    ```python
    a = input("Geef een getal: ")
    b = input("Geef nog een getal: ")
    print(a + b)
    ```

    ??? success "Toon antwoord"
        **Antwoord:** de twee invoeren worden **aan elkaar geplakt**.

        `input()` levert tekst op, dus `+` betekent hier samenvoegen.

---
#3.10 Debuggen met variabelen 
!!! tip "Debuggen"
    Als je code niet werkt zoals verwacht, kan je tussentijds variabelen afdrukken om te zien wat er misgaat.

Een veelvoorkomende oorzaak van functionele fouten in programma’s is dat variabelen
blijken niet de waardes te bevatten waarvan je dacht dat ze ze bevatten. Een goede manier
om je code te “debuggen” (dat wil zeggen, uit te vinden waar in je code fouten staan en
die te verbeteren) is het printen van variabele namen op geschikte plaatsen. Bijvoorbeeld:

```python
nr1 = 5
nr2 = 4
nr3 = 5
print( nr3 / (nr1 % nr2) )
nr1 = nr1 + 1
print( nr3 / (nr1 % nr2) )
nr1 = nr1 + 1
print( nr3 / (nr1 % nr2) )
nr1 = nr1 + 1
print( nr3 / (nr1 % nr2) )
## Dit programma veroorzaakt een foutmelding bij de vierde print-opdracht. Snap je waarom? Kopier deze code naar je Python-omgeving en voer het uit om het te testen.
```
Er zijn beter manieren om te debuggen, maar die zien we later in de cursus.

## 3.11 Samenvatting

!!! summary
    - `print()` toont output
    - `input()` vraagt informatie aan de gebruiker
    - Input is altijd tekst
    - Gebruik `int()` of `float()` om te rekenen
    - f-strings zijn de duidelijkste oplossing

---

➡️ **Volgende stap:** beslissingen nemen met `if` en `else`

