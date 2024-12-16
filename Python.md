
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
print (f"Je m'appelle{nom} {prénom} et j'ai {30} ans") # Je m'appelle Choukri Raja et j'ai 30 ans.
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
Il y a beaucoup d’autres méthodes https://docs.python.org/fr/3/tutorial/datastructures.html.

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

# **CONDITION**

En Python, une **condition** est une expression logique qui évalue une situation donnée pour déterminer si elle est vraie (True) ou fausse (False). Les conditions sont utilisées pour contrôler le flux du programme, en exécutant différentes parties du code en fonction du résultat de l'évaluation.

Les conditions sont souvent utilisées avec des structures de contrôle comme ***if***, ***elif***, et ***else***.

#### **<u>Le module `IF`</u>**

**if** est une instruction conditionnelle qui permet d'exécuter un bloc de code uniquement si une condition donnée est vraie *(True)*. Si cette condition est fausse *(False)*, le code ne s’exécutera pas

* ex:

```python
age = 18

if age >= 18: 
    print("Vous êtes majeur")

# Vous êtes majeur.
```
- **VRAI**: le code indenté sous le if est exécuté

- **FALSE**: Python passe au reste du programme sans exécuter ce bloc.

#### **<u>Le module `ELSE`</u>**

**else** est une clause utilisée avec une instruction conditionnelle pour spécifier un bloc de code à exécuter lorsque la condition de if est fausse (False).

```python
age = 18

if age >= 18: 
    print("Vous êtes majeur.")
    
else: 
    print("Vous êtes mineur.")

# Vous êtes majeur.
```
```python
age = 15

if age >= 18: # exécute le code quand est vrai
    print("Vous êtes majeur.")
    
else: # exécute le code quand est faux
    print("Vous êtes mineur.")

# Vous êtes mineur.
```
#### **<u>Le module `ELIF`</u>**

En Python, **elif** (abréviation de "else if") est une clause utilisée dans une structure conditionnelle pour tester plusieurs conditions de manière séquentielle. 

- ***elif***: est utilisé après un if et avant un else.

```python
note = 19

if note >= 18:
    print("Excellent !")
elif note >= 12:
    print("Bon travail.")
else:
    print("Besoin d'amélioration.")

# Excellent
```

```python
note = 15

if note >= 18:
    print("Excellent !")
elif note >= 12:
    print("Bon travail.")
else:
    print("Besoin d'amélioration.")

# Bon travail
```

```python
note = 10

if note >= 18:
    print("Excellent !")
elif note >= 12:
    print("Bon travail.")
else:
    print("Besoin d'amélioration.")

# Besoin d'amélioration
```
#### **<u>Le module `Conditions multiples`</u>**

Pour veérifir plusieurs condition pour un seul résultat dans la même instruction ***if***, il faut utiliser les *opérateurs logiques*:

- **AND** : vérifie si le deux condition sont vrai.

- **OR** : vérifie si au moins une condition est vrai.

- **NOT** : vérifie si une condition est faux. 

```python
utilisateur_connecte =  True
mot_de_passe_correct = False

if utilisateur_connecte and not mot_de_passe_correct:
    print("Mot de passe incorrect. Veuillez réessayer.")
else:
    print("Connexion réussie.")

# Mot de passe incorrect. Veuillez réessayer.
```

```python
utilisateur_connecte =  False
mot_de_passe_correct = True

if utilisateur_connecte and not mot_de_passe_correct:
    print("Mot de passe incorrect. Veuillez réessayer.")
else:
    print("Connexion réussie.")

# Connexion réussie.
```

#### **<u>Le module `Conditions avec des expression compratives`</u>**

```python
tables_disponibles = 30
tables_occupees = 25

if tables_disponibles > tables_occupees:
    print("Ne pas autorise plus des tables")

else: 
    print("Autoiser plus des table")

# ne pas autorise plus des tables
```
# **BOUCLE**

En Python, une **boucle** est une structure de contrôle qui permet de répéter l'exécution d'un bloc de code plusieurs fois, soit un nombre défini de fois, soit jusqu'à ce qu'une certaine condition soit remplie. Elle est utilisée pour automatiser des tâches répétitives et manipuler des données.

#### **<u>Le module `Boucle for`</u>**

- Utilisée pour parcourir un **itérable**.

- ex: 

```python
for i in range(5):
    print(i)
# Résultat : 0 1 2 3 4 
```
- ex: 

```python
for x in range(100):
    print(f"{x} bouteilles de sprite au mur !")

# bouteilles de sprite au mur !
# .
# 99 bouteilles de sprite au mur !
```
Les accolades  {}  ci-dessus prennent n’importe quelle valeur dans la variable   x  et la remplacent n’oubliez pas le   “f”  au début de la string, qui signifie  format

La fonction ***range()*** est réglée sur 0 par défaut.
Vous pouvez la modifier en ajoutant un autre nombre entier comme ça : **range(4, 10)**

* ex:

```python
for x in range(50, 100):
    print(f"{x} bouteilles de sprite au mur !")

# 50 bouteilles de sprite au mur !
# .
# 99 bouteilles de sprite au mur !
```

#### **<u>Le module `Boucle  while`</u>**

Répète un bloc de code tant qu'une condition est **vraie.**

- ex: 

```python
capacite_maximale = 10
capacite_actuelle = 3
while capacite_actuelle < capacite_maximale:
    capacite_actuelle += 1
    print(capacite_maximale)
# Résultat : 4 5 6 7 8 9 10

```


#### **<u>Le module `Boucles infinies`</u>**

Une **boucle infinie** est une structure de contrôle en programmation qui s'exécute sans fin, car sa condition est toujous **vrai**.

- ex: :

```python
i = 0
while i !=10:
    i += 0
    print(i)
# Résultat : 0 0 0 0 infinie
```

- **Boucle for**

Utilisez une ***boucle for*** lorsque vous savez à l'avance combien de fois vous devez exécuter le bloc de code.

- **Boucle while**

Utilisez une ***boucle while*** lorsque vous ne savez pas à l'avance combien de fois le bloc sera exécuté, mais vous avez une condition qui doit être vérifiée à chaque itération.


#### **<u>Le module `Break`</u>**

La commande **break** est utilisée pour interrompre une boucle immédiatement. Quand elle est exécutée, la boucle en cours se termine, même si la condition ou les itérations prévues ne sont pas terminées.

- ex: 

```python 
for i in range(10):
    if i == 5:
        break  # Arrête la boucle lorsque `i` vaut 5
    print(i)

# Résultat : 0 1 2 3 4 
```
#### **<u>Le module `Continue`</u>**

La commande **continue** permet de sauter l'itération actuelle et de passer directement à la suivante, sans arrêter la boucle. Cela est utile pour ignorer certaines conditions tout en continuant à parcourir le reste de la boucle.

- ex: 

```python
for i in range(10):
    if i == 5:
        continue  # Ignore le reste du code pour `i = 5`
    print(i)
# Résultat : 0 1 2 3 4 5 6 7 8 9

```
C'est on souhaite continuer la boucle sans exécuter le reste du code.

- ex: 

```python
nombres = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for nombre in nombres:
    if nombre % 2 == 0:  # Si le nombre est pair
        continue  # Passer à l'itération suivante
    print(nombre)  # Afficher uniquement les nombres impairs

# Résultat : 1 3 5 7 9
```

Dans cet exemple, les nombres pairs sont ignorés grâce à continue, et seuls les nombres impairs sont imprimés.

 # **FONCTION**

 Une **fonction** est un bloc de code conçu pour accomplir une tâche spécifique, et qui peut être identifié par un nom. Lorsqu'elle est appelée, la fonction exécute le code qu'elle contient. Elle peut également accepter des paramètres pour permettre son exécution avec des valeurs différentes, rendant le code plus modulaire et réutilisable.

 #### **<u>Le module `Définissez une fonction`</u>**


Les fonctions sont des blocs de code réutilisables qui organisent et structurent le code pour en faciliter la maintenance. En Python, elles sont créées avec le mot-clé **def**, suivi d'un nom et de paramètres optionnels entre parenthèses.

 #### **<u>Le module `Fonction sans paramètre`</u>**

Une fonction **sans paramètres** ni retour est un bloc de code autonome qui exécute une tâche spécifique lorsqu'il est appelé, sans nécessiter d'entrée ni produire de résultat.

- ex:

```python
def saluer():
    print("Bonjour !")

# Résultat : Rien
```

Elle n'a pas de valeur de retour car elle se contente d'afficher un message à l'écran en utilisant la fonction  print().

 #### **<u>Le module `Fonction avec paramètre`</u>**

Il est également possible de créer une fonction avec des paramètres, qui permettent de transmettre des valeurs à la fonction. Les paramètres sont listés entre parenthèses, séparés par des virgules.

- 1.ex: 

```python 
def afficher_nom_prenom(nom, prenom):
    print("Nom :", nom)
    print("Prénom :", prenom)

afficher_nom_prenom("Dupont", "Jean")

# Résultat : Nom : Dupont
#            Prénom : Jean
```
- 2.ex: 

```python
def addition(a, b):
    resultat = a + b
    print(resultat) 
    
addition(3, 10)

# Résultat : 13
```

#### **<u>Le module `Fonction avec paramètre optionnel`</u>**

- ex: 

```python
def saluer_nom(nom="Utilisateur"):
    print(f"Bonjour, {nom} !")

saluer_nom(("RJ"))

# Résultat : Bonjour, RJ !
```

#### **<u>Le module `Fonction avec valeur de retour`</u>**

Une fonction avec une valeur de retour est une fonction qui effectue une tâche et renvoie un résultat à l'endroit où elle a été appelée. Cela permet de récupérer la sortie de la fonction et de l'utiliser ultérieurement dans le programme. La valeur de retour est spécifiée avec le mot-clé return.

- ex: 

```python
def addition(a, b):
    return a + b

resultat = addition(8, 10)
print(resultat) 

# Résultat : 18
```

- Explication :

* **return a + b** permet de renvoyer le résultat de l'addition.

* L'appel **addition(8, 10)** renvoie 18, qui est ensuite stocké dans la variable resultat.

* **print(resultat)** affiche 18.

- Il est possible de renvoyer plusieurs valeurs depuis une fonction en les séparant par des virgules dans l'instruction return. Ces valeurs seront automatiquement regroupées dans un tuple. Cela permet de retourner plusieurs résultats à la fois, ce qui peut être utile pour des calculs ou des opérations complexes. 

```python
def calcul(a, b):
    somme = a + b
    difference = a - b
    produit = a * b
    return somme, difference, produit  # Retourne un tuple avec 3 valeurs

# Appel de la fonction
resultats = calcul(10, 5)

# Affichage des résultats
print("Somme:", resultats[0])
print("Différence:", resultats[1])
print("Produit:", resultats[2])

# Résultat : 15
# Résultat : 5
# Résultat : 50
```

# **CODEZ SANS ERREURS**

Écrire du code sans erreurs courantes implique d'éviter les fautes fréquentes, comme les erreurs de syntaxe, les variables mal définies, ou l'oubli de certaines étapes, afin d'assurer un fonctionnement fluide, une meilleure lisibilité et une maintenance facilitée.

#### **<u>Le module `Ne vous répétez pas`</u>**


Écrire du code sans erreurs courantes consiste à suivre des pratiques fiables pour éviter des bugs fréquents et assurer un code propre, lisible et fonctionnel.

- ex: ***code non structuré:***

```python
prix1 = produit1['prix'] * produit1['quantite']
prix2 = produit2['prix'] * produit2['quantite']
prix3 = produit3['prix'] * produit3['quantite']
```

- ex: ***code structuré*** 

```python 
# Définition de la fonction
def calculer_prix_total(produit):
    """Calcule le prix total d'un produit en fonction de son prix unitaire et de sa quantité."""
    return produit['prix'] * produit['quantite']

# Produits avec prix et quantités
produit1 = {'nom': 'Chaise', 'prix': 50, 'quantite': 4}
produit2 = {'nom': 'Table', 'prix': 150, 'quantite': 2}
produit3 = {'nom': 'Lampe', 'prix': 30, 'quantite': 5}

# Calcul des prix totaux
prix1 = calculer_prix_total(produit1)
prix2 = calculer_prix_total(produit2)
prix3 = calculer_prix_total(produit3)

# Affichage des résultats
print(f"Prix total pour {produit1['nom']}: {prix1} €")
print(f"Prix total pour {produit2['nom']}: {prix2} €")
print(f"Prix total pour {produit3['nom']}: {prix3} €")

# Résultat : Prix total pour Chaise: 200 €
# Résultat : Prix total pour Table: 300 €
# Résultat : Prix total pour Lampe: 150 €
```

#### **<u>Le module `CVS - Comma separated values`</u>**


En Python, **CSV** (Comma-Separated Values) désigne un format de fichier utilisé pour stocker des données tabulaires, où chaque ligne représente un enregistrement et chaque colonne est séparée par un séparateur (souvent une virgule, d’où le nom). Ce format est simple et largement utilisé pour échanger des données entre différentes applications.

- ex: Écriture de CVS

```python
import csv

# Ouvre (ou crée) un fichier CSV nommé 'fichier.csv'
with open('fichier.csv', mode='w', newline='') as fichier:
    # Initialise l'écrivain CSV
    ecrivain = csv.writer(fichier)
    
    # Écrit une ligne d'en-tête
    ecrivain.writerow(['Nom', 'Âge', 'Ville'])
    
    # Écrit des lignes de données
    ecrivain.writerow(['Alice', 30, 'Paris'])
    ecrivain.writerow(['Bob', 25, 'Lyon'])

print("Le fichier 'fichier.csv' a été créé ou mis à jour avec succès.")

# Résultat : Nom,Âge,Ville
#            Alice,30,Paris
#            Bob,25,Lyon
```

- **Ce qu’il se passe :**
1 - Création automatique :
* Si fichier.csv n'existe pas, Python crée un nouveau fichier nommé fichier.csv dans le répertoire où le script Python est exécuté.
* Le fichier contiendra les données spécifiées dans le script.

2 - Écrasement si le fichier existe déjà :
* Si fichier.csv existe, son contenu sera effacé et remplacé.

3 - Contenu final dans fichier.csv (après exécution de l'exemple ci-dessus) :

```fichier.cvs
Nom,Âge,Ville
Alice,30,Paris
Bob,25,Lyon
```
* Le fichier fichier.csv sera enregistré dans le même dossier où le script Python est exécuté.

* Si vous souhaitez spécifier un emplacement particulier, fournissez un chemin dans la fonction open(). Par exemple :

- ex: 

```python
with open('chemin/vers/dossier/fichier.csv', mode='w', newline='') as fichier:
    # Écriture du fichier
```
Voici une version améliorée du script pour informer l'utilisateur du succès de l'opération et du chemin du fichier généré :

```python
import csv
import os

# Définir le nom du fichier
nom_fichier = 'fichier.csv'

# Ouvrir (ou créer) le fichier
with open(nom_fichier, mode='w', newline='') as fichier:
    ecrivain = csv.writer(fichier)
    ecrivain.writerow(['Nom', 'Âge', 'Ville'])
    ecrivain.writerow(['Alice', 30, 'Paris'])
    ecrivain.writerow(['Bob', 25, 'Lyon'])

# Afficher un message de confirmation
chemin_complet = os.path.abspath(nom_fichier)
print(f"Le fichier '{nom_fichier}' a été créé avec succès à cet emplacement :")
print(chemin_complet)

# Résultat : Le fichier 'fichier.csv' a été créé avec succès à cet emplacement :/Users/raja/Desktop/Python/fichier.csv
```

#### **<u>Le module `Gérez les erreurs et les exceptions`</u>**

**Gérer les erreurs et les exceptions** consiste à détecter, traiter et résoudre les problèmes qui surviennent pendant l'exécution d'un programme, afin d'éviter les plantages et d'assurer un fonctionnement fiable.

Gestion des exceptions : Utiliser des mécanismes fournis par le langage de programmation, tels que **try**, **except**, et **finally**.

- ex: 

```python
try:
    num = int(input("Entrez un nombre : "))
    result = 10 / num
    print(f"Le résultat est {result}")
except ValueError:
    print("Vous devez entrer un nombre valide.")
except ZeroDivisionError:
    print("La division par zéro n'est pas autorisée.")
finally:
    print("Fin de l'exécution.")

# Résultat :  Entrez un nombre : 3
#             Le résultat est 3.3333333333333335
#             Fin de l'exécution.
```

- Le bloc **try** contient le code qui peut potentiellement provoquer une erreur.

- Les blocs **except** gèrent des types spécifiques d'exceptions.

- Le bloc **finally** est exécuté qu'il y ait ou non une exception.


# **IMPORTEZ DES PACKAGES PYTHON**

Un **package** Python peut simplement être considéré comme un répertoire contenant des **modules** Python.

#### **<u>Le module `Importez un module`</u>**

- ex: 

```python
import random  # Importe le module random

# Génère un nombre aléatoire entre 1 et 10
nombre = random.randint(1, 10)
print(f"Nombre aléatoire : {nombre}")

# Résultat :  Nombre aléatoire : 1
```    

#### **<u>Le module `Créez et importez un package`</u>**

Créer et importer un package signifie organiser plusieurs modules  dans un dossier pour structurer et réutiliser le code. Un package est simplement un dossier contenant un fichier spécial nommé __init__.py, qui peut être vide ou contenir du code pour initialiser le package. 

**Étapes pour créer et importer un package :**

1 - Créer un package :

* Créez un dossier avec un nom représentatif (par exemple, mon_package).

* Ajoutez un fichier __init__.py (il peut être vide).

* Ajoutez des fichiers Python (modules) dans ce dossier, comme **module1.py** et **module2.py.**

- Structure d'exemple :

mon_package/ #dossier
├── __init__.py
└── module2.py


- Contenu de **module1.py** :

```python
def saluer(nom):
    return f"Bonjour, {nom} !"
```
- Contenu de **main.py** :

```python
# main.py
import mon_package.module1 as m1  # Importa il modulo1 del pacchetto mon_package

# Usa la funzione del modulo
print(m1.saluer("Alice"))

# Résultat : Bonjour, Alice !
```

#### **<u>Le module `Installez les packages avec pip`</u>**

**pip** est un gestionnaire de paquets pour Python, utilisé pour installer, mettre à jour et gérer des bibliothèques externes.

```bash
pip install <nom-du-package>
```
- Exemple de sortie : 

```makefile
numpy==1.22.3
pandas==1.4.1
requests==2.26.0
```
**pip freeze**: est utilisée pour lister tous les packages installés. Cela est particulièrement utile pour créer un fichier **requirements.txt**, qui peut être utilisé pour partager ou recréer un environnement Python.

#### **<u>Le module `Créer un fichier requirements.txt`</u>**

```bash
pip freeze > requirements.txt
```

#### **<u>Le module `Installer à partir du fichier requirements.txt`</u>**

```bash
pip install -r requirements.txt
```  

# **EXTRACTION DE DONNÉES WEB**

L'**extraction de données web** (ou web scraping) est un processus automatisé qui consiste à extraire des informations spécifiques à partir de sites web. Cela se fait en utilisant des programmes ou des scripts capables de naviguer sur les pages web, d'analyser leur contenu (HTML, CSS, etc.) et de récupérer les données souhaitées.

#### **<u>Le module `ETL : Extraire, Transformer, Charger`</u>**

**ETL** signifie **extraction**, **transformation** et **chargement**. L'extraction de données web est un exemple d'ETL, où vous **récupérez** des données d'un site web, les **formatez** comme vous le souhaitez, et les stockez** dans un fichier CSV ou une base de données.

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Première Page Web</title>
</head>
<body>
    <!-- Titre principal -->
    <h1>Bienvenue sur ma page web</h1>

    <!-- Paragraphe introductif -->
    <p>Ceci est un exemple de page web utilisant les balises HTML essentielles.</p>

    <!-- Image avec description -->
    <img src="https://via.placeholder.com/150" alt="Image exemple">

    <!-- Liste ordonnée -->
    <h2>Liste de mes activités préférées :</h2>
    <ol>
        <li>Lire des livres</li>
        <li>Coder en Python</li>
        <li>Faire du sport</li>
    </ol>

    <!-- Lien hypertexte -->
    <p>Pour en savoir plus, visitez <a href="https://example.com">ce site web</a>.</p>

    <!-- Formulaire simple -->
    <h2>Contactez-moi :</h2>
    <form action="/submit" method="POST">
        <label for="nom">Nom :</label>
        <input type="text" id="nom" name="nom" placeholder="Votre nom">
        <br>
        <label for="email">Email :</label>
        <input type="email" id="email" name="email" placeholder="Votre email">
        <br>
        <button type="submit">Envoyer</button>
    </form>

    <!-- Pied de page -->
    <footer>
        <p>&copy; 2024 Mon Site Web. Tous droits réservés.</p>
    </footer>
</body>
</html>
````
- terminal: **open ex.html**

#### **<u>Le module `Le package Requests`</u>**

Le package Requests est une bibliothèque Python qui permet de faire des requêtes HTTP de manière simple et intuitive. Il est principalement utilisé pour interagir avec des sites web, télécharger des pages, envoyer des données à un serveur, ou accéder à des APIs.
