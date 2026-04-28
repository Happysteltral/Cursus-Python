# Hoofdstuk: Lijsten in Python

## Leerdoelen

Na dit hoofdstuk kan je:

- uitleggen wat een lijst is
- elementen toevoegen aan een lijst
- elementen aanpassen en verwijderen
- door een lijst lopen met een lus
- gegevens zoeken in een lijst
- basisbewerkingen uitvoeren op lijsten

---

# 1. Wat is een lijst?

Een **lijst** is een verzameling van meerdere waarden in één variabele.

In plaats van veel losse variabelen te maken:

```python
naam1 = "Emma"
naam2 = "Lucas"
naam3 = "Noah"
```

kan je alles samen bewaren in één lijst:

```python
namen = ["Emma", "Lucas", "Noah"]
```

!!! info "Belangrijk"
    Een lijst kan meerdere waarden bevatten.
    De waarden staan tussen rechte haken `[]`.

---

# 2. Elementen in een lijst

Elk element in een lijst heeft een nummer.

Dit nummer noemen we de **index**.

Python begint te tellen vanaf **0**.

| Index | Waarde |
|---|---|
| 0 | Emma |
| 1 | Lucas |
| 2 | Noah |

```python
namen = ["Emma", "Lucas", "Noah"]

print(namen[0])
print(namen[1])
```

Uitvoer:

```text
Emma
Lucas
```

!!! warning "Opgelet"
    De eerste positie in een lijst is altijd index `0`.

---

# 3. Een element aanpassen

Je kan een waarde in een lijst wijzigen.

```python
namen = ["Emma", "Lucas", "Noah"]

namen[1] = "Liam"

print(namen)
```

Uitvoer:

```text
['Emma', 'Liam', 'Noah']
```

---

# 4. Elementen toevoegen

Met `.append()` voeg je een element toe achteraan de lijst.

```python
namen = ["Emma", "Lucas"]

namen.append("Noah")

print(namen)
```

Uitvoer:

```text
['Emma', 'Lucas', 'Noah']
```

!!! tip "Tip"
    `.append()` wordt zeer vaak gebruikt bij lijsten.

---

# 5. Elementen verwijderen

Met `.remove()` verwijder je een element.

```python
namen = ["Emma", "Lucas", "Noah"]

namen.remove("Lucas")

print(namen)
```

Uitvoer:

```text
['Emma', 'Noah']
```

---

# 6. Lengte van een lijst

Met `len()` kan je tellen hoeveel elementen een lijst bevat.

```python
namen = ["Emma", "Lucas", "Noah"]

print(len(namen))
```

Uitvoer:

```text
3
```

---

# 7. Door een lijst lopen

Vaak wil je alle elementen één voor één verwerken.

Dat doe je met een `for`-lus.

```python
namen = ["Emma", "Lucas", "Noah"]

for naam in namen:
    print(naam)
```

Uitvoer:

```text
Emma
Lucas
Noah
```

!!! info "Wat gebeurt hier?"
    De variabele `naam` krijgt telkens één element uit de lijst.

---

# 8. Controleren of iets in een lijst zit

Met `in` kan je controleren of een waarde voorkomt.

```python
namen = ["Emma", "Lucas", "Noah"]

if "Lucas" in namen:
    print("Gevonden")
```

Uitvoer:

```text
Gevonden
```

---

# 9. Lijsten met getallen

Een lijst hoeft niet enkel tekst te bevatten.

```python
punten = [12, 15, 18, 9]

print(punten[2])
```

Uitvoer:

```text
18
```

Je kan ook rekenen met lijsten.

```python
punten = [12, 15, 18, 9]

print(sum(punten))
print(max(punten))
print(min(punten))
```

Uitvoer:

```text
54
18
9
```

!!! note "Handige functies"
    - `sum()` → som van alle getallen
    - `max()` → grootste waarde
    - `min()` → kleinste waarde

---

# 10. Geneste lijsten

Een lijst kan ook andere lijsten bevatten.

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

print(matrix[1][2])
```

Uitvoer:

```text
6
```

!!! warning "Moeilijker onderwerp"
    Geneste lijsten worden later belangrijk bij tabellen, games en AI.

---

# 11. Veelgemaakte fouten

## Verkeerde index

```python
namen = ["Emma", "Lucas"]

print(namen[5])
```

Foutmelding:

```text
IndexError
```

## Haakjes vergeten

Correct:

```python
namen = ["Emma", "Lucas", "Noah"]
```

Fout:

```python
namen = "Emma", "Lucas", "Noah"
```

---

# 12. Samenvatting

| Bewerking | Voorbeeld |
|---|---|
| Lijst maken | `namen = ["Emma", "Lucas"]` |
| Element lezen | `namen[0]` |
| Element aanpassen | `namen[1] = "Liam"` |
| Toevoegen | `namen.append("Noah")` |
| Verwijderen | `namen.remove("Lucas")` |
| Lengte | `len(namen)` |
| Doorlopen | `for naam in namen:` |
| Zoeken | `"Emma" in namen` |

---

