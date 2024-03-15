Met de pygal bibliotheek kun je interactieve grafieken van gegevens maken.

```python
from pygal import *
```

Om een grafiek met pygal te maken moet je een van de functies van de bibliotheek gebruiken:
 - `Bar()` maakt een staafdiagram
 - `Pie()` maakt een taartdiagram

```python
grafiek = Pie()
```

Vervolgens moet je enkele gegevens aan de grafiek toevoegen met behulp van de `add()` functie van je grafiek:

```python
grafiek.add(item, waarde)
```

Waarbij:
 - `item` is een string — het kan een land, een persoon, een type auto, enz. zijn.
 - `waarde` is een getal gerelateerd aan `item`

Tot slot moet je de `render()` functie van je grafiek aanroepen om deze weer te geven.

Bijvoorbeeld:

```python
from pygal import Pie
# Maak een taartdiagram
grafiek = Pie()
# Voeg wat gegevens toe
grafiek.add('Katten', 5)
grafiek.add('Honden', 10)
grafiek.add('Konijnen', 10)
# Toon de grafiek
grafiek.render()
```

![Een taartdiagram, die secties voor katten, honden en konijnen weergeeft](images/pie.png)


