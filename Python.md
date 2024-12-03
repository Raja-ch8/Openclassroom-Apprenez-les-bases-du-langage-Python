
# *PYTHON*

### **VARIABLE**

Les **variables** sont un moyen d'enregistrer des données dans un programme. Elles permettent de sauvegarder des informations avec un nom, afin de pouvoir les réutiliser plus tard.

Une variable en Python est constituée de trois éléments principaux :

**1. Type :** Détermine la catégorie de données que la variable contient.

**2.  Nom :** Indique le nom associé à la variable, facilitant son identification.

**3. Valeur :** Contenu de la variable.

* ex:

```python
nom = "Choukri"
prénom = "Raja"
age = 30
print (f"Je m'appelle {nom} {prénom} et j'ai {30} ans") # Je m'appelle Choukri Raja et j'ai 30 ans.
```
### **TYPE DE DONNÉE**

Les types de données permettent de classer les variables selon leur contenu.

**<u>Le module `Les entiers(integers)`</u>**: Représentent des nombres entiers.
Exemple:  1  - 4 - 7 - 12

**<u>Le module `Les virgule flosttantes (floats)`</u>**: Représentent des nombres décimaux.
Exemple: 3.14 - 6.67 - 10.3.

**<u>Le module `Les chaînes de caractères (string)`</u>**: Représentent du texte, entouré de guillemets.
Exemple: "Bonjour" - "Salut".

**<u>Le module `Les booléens`</u>**: Représentent des valeurs logiques. 
Exemple: Faux ou Vrai.

### **LISTE**

Une **liste** permet de regrouper plusieurs éléments dans une seule variable. Elle est définie à l'aide de crochets [], et chaque élément de la liste a un indice pour y accéder.

* ex : 

```python

Fruits = ["Pomme", "Orange", "Poire"]
Fruits[0]
print(Fruits[0]) # Pomme

```

Indices et chaînes de caractères :

Les **indices** fonctionnent également avec les chaînes de caractères.

* ex:

```python
Langage = "PYTHON"
Langage[2]
print(Langage[2]) # Affiche : T
```

```python
Langage = "PYTHON"
Langage[-4]
print(Langage[-4]) # Affiche: T
```
* Les indices positifs commencent à 0.
* Les indices négatifs commencent à -1, en comptant à parti

#### **<u>Le module `Modifiez les éléments d'une liste`</u>**

Pour modifier un élément dans une liste, il suffit d'utiliser son indice.

* ex: 

```python

sociales = ["Facebook", "Instagram", "Twitter", "Snapchta"]
sociales[2] = "TikTok"
print(sociales)  # ['Facebook', 'Instagram', 'TikTok', 'Snapchta']

```

#### **<u>Le module `Ajouter le listes`</u>**

Pour **ajouter** un élément à la fin d'une liste, utilisez la méthode append().

* ex: 

```python

sociales = ["Facebook", "Instagram", "Twitter", "Snapchta"]
sociales.append("TikTok")
print(sociales) # ['Facebook', 'Instagram', 'Twitter', 'Snapchta', 'TikTok']

```

#### **<u>Le module `Retirez le listes`</u>**

Pour supprimer un élément spécifique dans une liste, utilisez la méthode **remove().**

* ex: 

```python

sociales = ["Facebook", "Instagram", "Twitter", "Snapchta"]
sociales.remove("Twitter")
print(sociales) # ['Facebook', 'Instagram', 'Snapchta']

```

#### **<u>Le module `Trier les éléments d'une liste`</u>**

La méthode sort() permet de trier les éléments d'une liste. Elle peut être utilisée avec l'argument key pour une logique de tri personnalisée.

```python

sociales = ["Facebook", "Instagram","Snapchat"]
sociales.sort(key=lambda x: x.startswith("I"), reverse=True)
print(sociales) #['Instagram', 'Facebook', 'Snapchat']

```
### **TUPLE**


Les **tuples** sont une autre structure de données en Python utilisée pour stocker des informations. Ils se distinguent par l'utilisation de parenthèses () et sont immuables, c'est-à-dire que leur contenu ne peut pas être modifié après leur création.

* ex: 

```python 
sociales = ("Facebook", "Instagram", "Snapchat")
```

#### **<u>Le module `Trouvez un élément`</u>**

Pour vérifier si un élément est présent dans un tuple, on peut utiliser l'opérateur in. Si l'élément est présent, le résultat sera **True** (Vrai) ; sinon, le résultat sera **False** (Faux).

* ex:

```python
nombres = (1,2,3,4,5) # AAffiche False, car 6 n'est pas dans le tuple
print(6 in nombres) # Affiche le tuple : (1, 2, 3, 4, 5)
print(nombres) # False 
               # (1, 2, 3, 4, 5)

```
## **DICTIONNAIRE**

Un **dictionnaire** en Python est une structure de données qui permet de stocker des **paires clé-valeur**. Chaque clé est unique et agit comme un identifiant pour sa valeur correspondante. Les dictionnaires sont définis à l'aide des accolades {} et sont très utiles pour organiser et récupérer des données de manière efficace.

* ex: 

Imaginons que vous souhaitiez enregistrer des informations sur une nouvelle campagne de marketing pour une entreprise de vêtements. Vous pourriez avoir besoin de sauvegarder le nom de la campagne, les dates de début et de fin, le responsable de la campagne, et les plateformes utilisées. Un dictionnaire est idéal pour organiser ces informations de manière claire et structurée.

```python
# Création d'un dictionnaire pour une campagne marketing
campagne_marketing = {
    "nom_campagne": "Mode Automne 2024",
    "date_debut": "2024-05-08",
    "date_fin": "2024-12-31",
    "responsable": "Alice Dupont",
    "plateformes": ["Instagram", "Facebook", "TikTok"],
}

# Accéder aux informations
print(f"Nom de la campagne : {campagne_marketing['nom_campagne']}")
print(f"Dates : du {campagne_marketing['date_debut']} au {campagne_marketing['date_fin']}")
print(f"Responsable : {campagne_marketing['responsable']}")
print(f"Plateformes utilisées : {', '.join(campagne_marketing['plateformes'])}")

# Nom de la campagne : Mode Automne 2024
# Dates : du 2024-05-08 au 2024-12-31
# Responsable : Alice Dupont
# Plateformes utilisées : Instagram, Facebook, TikTok
```
Un dictionnaire est parfait pour ce type de données car :

- **Clarté :** Les informations sont organisées en paires clé-valeur, ce qui les rend faciles à lire et à comprendre.

- **Flexibilité :** Vous pouvez ajouter ou modifier les clés et valeurs selon vos besoins.

- **Accès rapide :** Vous pouvez récupérer n'importe quelle information en utilisant sa clé.

Vous pouvez également créer un dictionnaire vide de deux façons : en utilisant des accolades {} ou la fonction dict(). Ces méthodes permettent de créer un dictionnaire initialement vide, que vous pourrez remplir plus tard.

* ex: Utiliser des accolades {}

```python
campagne = {}  # Création d'un dictionnaire vide
campagne["nom"] = "Promo Été 2024"  # Ajout d'une clé et d'une valeur
campagne["date_debut"] = "2024-06-01"
print(campagne)

# {'nom': 'Promo Été 2024', 'date_debut': '2024-06-01'}
```

* ex: Utiliser la fonction dict()

```python
campagne = dict()  # Création d'un dictionnaire vide avec dict()
campagne["nom"] = "Black Friday"
campagne["date_fin"] = "2024-11-30"
print(campagne)
# {'nom': 'Black Friday', 'date_fin': '2024-11-30'}

```
Pourquoi utiliser des dictionnaires vides ?

- **Flexibilité :** Créer un dictionnaire vide vous permet de le remplir dynamiquement, par exemple en ajoutant des données collectées à partir de l'entrée utilisateur ou d'une API.

- **Clarté :** Vous pouvez commencer par une structure vide et ajouter des informations au fur et à mesure qu'elles deviennent disponibles.

#### **<u>Le module `Accédez à une valeur`</u>**

Pour récupérer une valeur dans un dictionnaire, utilisez la clé associée à cette valeur.

* ex: 

```python
campagne = {
    "nom": "Black & White"
}
campagne = campagne["nom"]
print(campagne)

#  Black & White
```
#### **<u>Le module `Ajouter une paire clé-valeur`</u>**

Pour **ajouter** une paire clé-valeur à un dictionnaire, il suffit d'affecter une valeur à une nouvelle clé. Si la clé existe déjà, sa valeur sera mise à jour.  Le code suivant crée un dictionnaire appelé **info**

* ex: 

```python
info_valise = {
    "H": "50 cm",
    "L": "29 cm"
}
info_valise["P"] = "25 cm" 
print(info_valise)

# {'H': '50 cm', 'L': '29 cm', 'P': '25 cm'}
```

#### **<u>Le module `Supprimez une paire clé-valeur`</u>**

Pour **supprimer** une paire clé-valeur dans un dictionnaire, vous pouvez utiliser le mot-clé **del** suivi de la clé que vous souhaitez supprimer. Une autre option est d'utiliser la méthode **pop()**, qui permet de supprimer une paire clé-valeur et de récupérer la valeur associée à la clé supprimée.

* ex: 
Pour supprimer la paire clé-valeur  "P"  de la paire  clé-valeur:

```python
info_valise = {
    "H": "50 cm",
    "L": "29 cm"
}
del info_valise["L"]
print(info_valise)

# {'H': '50 cm'}
```
