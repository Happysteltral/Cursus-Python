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

Je kan ook variabelen afdrukken:

```python
naam = "Alex"
leeftijd = 16
print(naam)
print(leeftijd)
```

---

## 3.3 Tekst en variabelen combineren

!!! warning "Let op"
    Je kan **geen tekst en getallen rechtstreeks optellen**.

❌ Fout:
```python
leeftijd = 16
print("Ik ben " + leeftijd + " jaar")
```

✅ Oplossing 1 – komma’s:
```python
print("Ik ben", leeftijd, "jaar")
```

✅ Oplossing 2 – `str()`:
```python
print("Ik ben " + str(leeftijd) + " jaar")
```

---

## 3.4 f-strings (aanbevolen)

!!! tip "Goede gewoonte"
    Gebruik **f-strings** om tekst en variabelen netjes te combineren.

```python
print(f"Ik ben {leeftijd} jaar")
```

👉 Alles tussen `{ }` wordt automatisch omgezet naar tekst.

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
    Gebruik deze functies om tekst om te zetten:

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

## 3.9 Oefeningen

### Oefening 1 – Begroeting
Vraag de naam van de gebruiker en toon een begroeting.

### Oefening 2 – Leeftijd
Vraag de leeftijd en toon hoe oud de gebruiker volgend jaar is.

### Oefening 3 – Rekenmachine
Vraag twee getallen en toon:
- de som
- het verschil
- het product

### Oefening 4 – Mini-toepassing
Maak een programma dat:
1. de naam vraagt
2. het geboortejaar vraagt
3. de leeftijd berekent
4. een zin toont met f-string

---

## 3.10 Samenvatting

!!! summary
    - `print()` toont output
    - `input()` vraagt informatie aan de gebruiker
    - Input is altijd tekst
    - Gebruik `int()` of `float()` om te rekenen
    - f-strings zijn de duidelijkste oplossing

---

➡️ **Volgende stap:** beslissingen nemen met `if` en `else`

