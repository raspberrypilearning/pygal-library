La bibliothèque pygal te permet de créer des graphiques interactifs à partir de données.

```python
from pygal import *
```

Pour créer un graphique avec pygal, tu dois utiliser l'une des fonctions fournies par la bibliothèque :
 - `Bar()` crée un histogramme
 - `Pie()` crée un camembert

```python
chart = Pie()
```

Tu dois ensuite ajouter quelques données au graphique en utilisant la fonction `add()` pour ton graphique :

```python
chart.add(item, value)
```

Où :
 - `élément` est une chaîne de caractères — il peut s'agir d'un pays, d'une personne, d'un type de voiture, etc.
 - `valeur` est un nombre lié à `élément`

Pour finir, tu dois appeler la fonction `render()` pour ton graphique afin de l'afficher.

Par exemple :

```python
from pygal import Pie
# Create a Pie chart
chart = Pie()
# Add some data
chart.add('Cats', 5)
chart.add('Dogs', 10)
chart.add('Rabbits', 10)
# Display the chart
chart.render()
```

![Camembert, avec des sections pour les chats, les chiens et les lapins](images/pie.png)


