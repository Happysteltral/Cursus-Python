# Stap 1 – Expressies en berekeningen in Python

## 1.1 Wat is een expressie?

!!! note "Theorie"
    Een **expressie** is een combinatie van waarden, variabelen en operatoren die samen **een nieuwe waarde opleveren**.

Voorbeelden van expressies:

```python
5 + 3
leeftijd + 1
prijs * aantal
```

Een expressie **rekent iets uit**, je kan het vergelijken met een vergelijking.

---

## 1.2 Rekenkundige operatoren

!!! info
    Python kan rekenen zoals een rekenmachine.

| Operator | Betekenis | Voorbeeld |
|--------|----------|----------|
| `+` | optellen | `5 + 3` |
| `-` | aftrekken | `10 - 4` |
| `*` | vermenigvuldigen | `6 * 2` |
| `/` | delen | `10 / 4` |
| `//` | delen (zonder komma) | `10 // 4` |
| `%` | rest van de deling | `10 % 4` |
| `**` | macht | `2 ** 3` |

---
## 1.3 Voorbeelden van expressies

```python
# Optellen
print(7 + 3)  # Je krijgt 10 in je terminal
# Aftrekken
print(15 - 4)  # Je krijgt 11 in je terminal
# Vermenigvuldigen
print(6 * 3)  # Je krijgt 18 in je terminal
# Delen
print(20 / 4)  # Je krijgt 5.0 in je terminal
# Gehele deling 
print(22 // 3)  # Je krijgt 6 in je terminal, alles achter de komma wordt weggelaten
# Rest van de deling
print(22 % 3)  # Je krijgt 1 in je terminal, want 3 past 7 keer in 22 met een rest van 1
# Machten
print(3 ** 4)  # Je krijgt 81 in je terminal.
```
## 1.4 Volgorde van bewerkingen

!!! note "Belangrijk"
    Python volgt dezelfde rekenregels als in de wiskunde:

    1. Haakjes
    2. Machten
    3. Vermenigvuldigen en delen
    4. Worteltrekken
    5. Optellen en aftrekken

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

## 1.5 Datatypes
!!! note "Theorie"
    In Python zijn er verschillende **datatypes** die bepalen welk soort waarde je gebruikt.
| Type | Voorbeeld | Betekenis |
|----|----|----|
| `int` | `10` | geheel getal |
| `float` | `3.14` | kommagetal |
| `str` | `"Hallo"` | tekst |
| `bool` | `True`, `False` | waar / onwaar |


## 1.6 Veelgemaakte fouten

!!! warning
    - Delen door nul (`10 / 0`)
    - het resultaat van 10/4 opslaan in een `int` variabele
    - Verkeerde volgorde van bewerkingen
    - Haakjes vergeten bij complexe berekeningen

---

## 1.7 🧠 Test jezelf

??? question "Bekijk de berekenning hieronder en probeer te bepalen wat de uitkomst is *voordat* je hem uitvoert:"
    ```python
    print( 5*2 -  3 + 4/2 )

    ```

    ??? success "Toon antwoord"
        **Antwoord:** `9.0`

        `eerst 5*2 = 10`  
        `dan 4/2 = 2.0` 
        `dan 10 - 3 + 2.0 = 9.0`
        Let op: het resultaat is een `float` omdat er een deling in de berekening zit. De computer weet niet of je een geheel getal of kommagetal wilt als resultaat, dus kiest hij automatisch voor `float` als er een deling in de berekening zit.
---

## 1.8 String expressies

!!! note "Theorie"
    Strings (tekst) kunnen ook gecombineerd worden met expressies, maar niet allemaal.
    
We kunnen strings **samenvoegen** met de `+` operator:

```python
print( "tot"+"ziens" )
print( 3* "hallo" )
print( "tot ziens" *3 )


## 1.9 Samenvatting

!!! summary
    - Een expressie rekent een waarde uit
    - Expressies gebruiken operatoren
    - Haakjes bepalen de volgorde
    - Er zijn verschillende datatypes: `int`, `float`, `str`, `bool`

---

➡️ **Volgende stap:** Variabelen

