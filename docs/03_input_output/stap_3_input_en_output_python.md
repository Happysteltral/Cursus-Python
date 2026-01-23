# Stap 3 – Input en Output (Python)

## 3.1 Waarom input en output?
Tot nu toe hebben we gewerkt met **vaste waarden** in ons programma. Dat is handig om te oefenen, maar echte programma’s worden pas interessant wanneer:
- 👤 **de gebruiker iets kan invoeren** (input)
- 🖥️ **het programma iets terug toont** (output)

👉 In deze stap leren we hoe een Python-programma kan **communiceren met de gebruiker**.

---

## 3.2 Output tonen met `print()`

### 3.2.1 Basisgebruik
Met `print()` toon je tekst of waarden op het scherm.

```python
print("Hallo wereld")
```

Je kan ook een **variabele** afdrukken:

```python
leeftijd = 16
print(leeftijd)
```

---

### 3.2.2 Tekst en variabelen combineren

❌ Dit werkt **niet**:
```python
print("Ik ben " + leeftijd + " jaar oud")
```

Waarom niet? 👉 `leeftijd` is een **getal**, geen tekst.

✅ Oplossing 1: komma’s gebruiken (simpel en veilig)
```python
print("Ik ben", leeftijd, "jaar oud")
```

✅ Oplossing 2: `str()` gebruiken
```python
print("Ik ben " + str(leeftijd) + " jaar oud")
```

---

### 3.2.3 f-strings (aanbevolen)

Dit is de **modernste en duidelijkste manier**:

```python
print(f"Ik ben {leeftijd} jaar oud")
```

👉 Alles tussen `{ }` wordt automatisch omgezet naar tekst.

---

## 3.3 Input vragen met `input()`

### 3.3.1 Basisgebruik

```python
naam = input("Wat is je naam? ")
print(f"Hallo {naam}")
```

⚠️ **Belangrijk:** alles wat met `input()` binnenkomt is **tekst (string)**.

---

### 3.3.2 Rekenen met input

❌ Dit gaat fout:
```python
leeftijd = input("Wat is je leeftijd? ")
volgend_jaar = leeftijd + 1
```

Waarom? 👉 `leeftijd` is een string.

✅ Correcte aanpak:
```python
leeftijd = int(input("Wat is je leeftijd? "))
volgend_jaar = leeftijd + 1
print(f"Volgend jaar ben je {volgend_jaar} jaar")
```

---

## 3.4 Veelgemaakte fouten

| Fout | Verklaring |
|----|-----------|
| `input()` vergeten om te zetten | Input is altijd tekst |
| `+` gebruiken bij tekst en getallen | Typefout |
| Geen duidelijke vraag stellen | Slechte gebruikerservaring |

---

## 3.5 Oefeningen

### Oefening 1 – Begroeting
Vraag de naam van de gebruiker en toon:
> Hallo ___!

---

### Oefening 2 – Leeftijd
Vraag de leeftijd en toon:
> Jij bent ___ jaar oud

---

### Oefening 3 – Rekenen met input
Vraag twee getallen en toon:
- de som
- het verschil
- het product

---

### Oefening 4 – Mini-toepassing
Maak een programma dat:
1. de naam van de gebruiker vraagt
2. het geboortejaar vraagt
3. de leeftijd berekent
4. een zin toont zoals:

> Hallo Alex, jij bent ongeveer 16 jaar oud.

---

## 3.6 Samenvatting

- `print()` = output tonen
- `input()` = gegevens vragen aan de gebruiker
- Input is **altijd tekst**
- Gebruik `int()` of `float()` voor berekeningen
- f-strings maken code leesbaar

---

➡️ **Volgende stap:** voorwaarden (`if`, `else`) – het programma laten beslissen

