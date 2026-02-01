# Stap 2 – Expressies en berekeningen in Python

## 2.1 Wat is een expressie?

!!! note "Concept"
    Een **expressie** is een combinatie van waarden, variabelen en operatoren die samen **een nieuwe waarde opleveren**.

Voorbeelden van expressies:

```python
5 + 3
leeftijd + 1
prijs * aantal
```

👉 Een expressie **rekent iets uit**.

---

## 2.2 Rekenkundige operatoren

!!! info
    Python kan rekenen zoals een rekenmachine.

| Operator | Betekenis | Voorbeeld |
|--------|----------|----------|
| `+` | optellen | `5 + 3` |
| `-` | aftrekken | `10 - 4` |
| `*` | vermenigvuldigen | `6 * 2` |
| `/` | delen | `10 / 4` |
| `//` | gehele deling | `10 // 4` |
| `%` | rest (modulo) | `10 % 4` |
| `**` | macht | `2 ** 3` |

---

## 2.3 Expressies met variabelen

!!! example "Voorbeeld"
    ```python
    prijs = 2.5
    aantal = 4
    totaal = prijs * aantal
    print(totaal)
    ```

👉 `prijs * aantal` is een **expressie** waarvan het resultaat wordt opgeslagen in `totaal`.

---

## 2.4 Volgorde van bewerkingen

!!! note "Belangrijk"
    Python volgt dezelfde rekenregels als in de wiskunde:

    1. Haakjes
    2. Machten
    3. Vermenigvuldigen en delen
    4. Optellen en aftrekken

Voorbeeld:

```python
resultaat = 5 + 3 * 2
print(resultaat)  # 11
```

Met haakjes:

```python
resultaat = (5 + 3) * 2
print(resultaat)  # 16
```

---

## 2.5 Expressies opslaan in variabelen

!!! tip
    Sla tussenresultaten op in variabelen om je code leesbaar te houden.

```python
basis = 50
btw = basis * 0.21
totaal = basis + btw
print(totaal)
```

---

## 2.6 Veelgemaakte fouten

!!! warning
    - Delen door nul (`10 / 0`)
    - Verwachten dat `10 / 4` een geheel getal geeft
    - Haakjes vergeten bij complexe berekeningen

---

## 2.7 🧠 Test jezelf

??? question "Wat wordt er afgedrukt?"
    ```python
    x = 10
    y = x // 3
    z = x % 3
    print(y, z)
    ```

    ??? success "Toon antwoord"
        **Antwoord:** `3 1`

        `10 // 3` is de gehele deling → 3  
        `10 % 3` is de rest → 1

---

## 2.8 Oefeningen

### Oefening 1
Maak twee variabelen `a` en `b` en druk af:
- de som
- het verschil
- het product

### Oefening 2
Bereken de omtrek van een rechthoek met:
- lengte = 8
- breedte = 5

### Oefening 3
Bereken het aantal seconden in:
- 2 uur
- 3 minuten

---

## 2.9 Samenvatting

!!! summary
    - Een expressie rekent een waarde uit
    - Expressies gebruiken operatoren
    - Haakjes bepalen de volgorde
    - Resultaten kan je opslaan in variabelen

---

➡️ **Volgende stap:** input en output

