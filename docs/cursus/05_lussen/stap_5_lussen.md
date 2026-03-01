# 🧠 stap 5 – Lussen (while & for)

In dit hoofdstuk leer je hoe je stukken code kan **herhalen** met behulp van lussen.

---

## 5.1 Wat is een lus?

!!!info
    Een **lus** (loop) zorgt ervoor dat een stuk code meerdere keren wordt uitgevoerd.


Voorbeeld:
```python
for i in range(5):
    print("Hallo")
```
Deze code print 5 keer "Hallo".

---

## 5.2 De `while` lus

Een `while` lus blijft herhalen zolang een voorwaarde **waar** is.

```python
x = 1

while x <= 5:
    print(x)
    x = x + 1
```

!!!tip
    Vergeet niet om je variabele in de lus aan te passen, anders krijg je een **oneindige lus**.

---

## 5.3 De `for` lus

Een `for` lus gebruik je wanneer je **op voorhand weet hoe vaak** je wil herhalen.

```python
for i in range(1, 6):
    print(i)
```

!!! info
    `range(1, 6)` betekent: start bij 1 en ga tot 5 (6 wordt niet meer meegerekend).

---

## 5.4 Tellers en accumulators

Een **teller** telt hoe vaak iets gebeurt.  
Een **accumulator** telt waarden op.

```python
som = 0

for i in range(1, 6):
    som = som + i

print(som)
```

!!!tip
    Gebruik een accumulator wanneer je een **som of totaal** wil berekenen.


---

## 5.5 Veelgemaakte fouten

!!! warning
    - Vergeten om de variabele in een `while` lus aan te passen  
    - Verkeerd bereik in `range()`  
    - Oneindige lus zonder stopvoorwaarde


---

## 5.6 Test jezelf

??? question "Wat zal deze code afdrukken?"
    ```python
    x = 0

    while x < 3:
        print(x)
        x = x + 1
    ```

    ??? success "Toon Antwoord
        De output is:
        ```
        0
        1
        2
        ```
---

## 5.7 Samenvatting

!!! info
    - Gebruik **while** als je niet weet hoe vaak je moet herhalen  
    - Gebruik **for** als je exact weet hoe vaak  
    - Gebruik een **teller** om te tellen  
    - Gebruik een **accumulator** om op te tellen

