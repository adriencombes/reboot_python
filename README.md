# Python Reboot

Ce repo comporte plusieurs enoncés d'exercices. Pour chaque enoncé, plusieurs reponses sont proposées. Celles-ci comportent une ou plusieurs erreurs, sont soit mal optimisées (ou comportent des mauvaises pratiques), soit carrément buggées.

L'idée est donc de chercher à imaginer si chacune de ses reponses planterai, auquel cas quelle serait l'erreur ? Dans le cas contraire donnerai-t-elle le resultat attendu, et comment pourrai-t-elle être corrigée ou ameliorée ? Quelle partie au contraire est juste (vous pouvez procéder par elimination à partir de ce que vous jugez correct). (Certaines reponses contiennent parfois plusieurs erreurs.

Prenez le temps de bien reflechir avant d'executer du code.
Dans la mesure du possible faites des tests pour verifier vos solutions proposées.

---


### .1 Créez un dossier notebooks dans ce repo

```bash
pwd notebooks
```

```bash
touch /notebooks
```

```bash
mkdir -p../notebooks
```

```bash
cd ../notebooks
```



### .2 **Copiez** le fichier notebook à la racine du repo dans le dossier créé

```bash
cd .reboot_python.ipynb notebooks
```

```bash
cp reboot_python.ipynb /notebooks
```

```bash
mv ../reboot_python.ipynb notebooks
```



### .3 Verifiez qu'aucune libaririe n'est installée sur l'environnement virtuel actuel (créé au préalable)

```bash
import .
```



### .4 Installez la librairie requests (2.28.1)

```bash
pip requests
```

```bash
pip import requests
```

```bash
python get "requests"
```



### .5 Supprimez le fichier notebook vierge à la racine du repo (attention à pas supprimer celui que vous avez complété)

```bash
rm -r ./notebooks
```

```bash
mv .reboot_python ..
```

```bash
rm .reboot_python.ipynb
```



### .6 Verifiez que l'environnement virtuel tourne bien sur python 3.10.6

```bash
pip version
```

```bash
pip --version
```



### .7 Ouvrez le jupyter notebook dans le dossier notebooks *(de maniere à ce qu'il s'ouvre dans votre navigateur)*

La plupart des enoncés suivants traitent de Python et peuvent etre exécutés dans ce notebook.

```bash
open reboot_python.ipynb
```



### 8. Importez la librairie requests

```python
from requests as requests
```

```python
pip install requests
```



### 9. Assignez la liste suivante à une variable `[1, -3, "jeanmich", -6, "toto", 8, 2]`

```python
list(1, -3, "jeanmich", -6, "toto", 8, 2)
```

```python
list = [1, -3, "jeanmich", -6, "toto", 8, 2]
```

```python
my_list = list[1, -3, "jeanmich", -6, "toto", 8, 2]
```



### 10. Editez cette liste pour remplacer `"jeanmich"` par la **string** `"10"`

```python
my_list["jeanmich"] = 10
```

```python
my_list.drop("jeanmich") = "10"
```



### 11. Supprimez de la liste `'toto'`

```python
remove(my_list[5])
```

```python
numbers.del[2]
```


### 12. Rajoutez `-15` à la fin de cette liste

```python
my_list[6] = -15
```

```python
my_list[6] = -15
```



### 13. Editez cette liste pour convertir la string `"10"` en nombre *(sans toucher au chiffre 1 de votre clavier)*

```python
my_list.drop() = 10
```



### 14. A partir de votre premiere liste, créer une seconde liste qui ne contient que les valeurs positives de la première

```python
my_second_list = []
for number in my_list:
    if (number > 0):
    return my_second_list.append(number)
```

```python
my_second_list = []
for number in my_list:
    if number > 0:
        my_second_list += 1
    else:
        none
```

```python
i = 0
for number in my_list
    if my_list[i] > 0:
        my_second_list.append(my_list[i])
        i += 1
    else:
        i += 1
```

```python
for number in my_list:
    if number > 0
        my_list[i].append(1)
    else:
        return
```



### 15. Transformer ce code en une list comprehension

```python
my_second_list = [number for number if number > 0 in my_list]
```

```python
my_second_list = [x: x>=0 for x in numbers]
```

```python
my_second_list = [number > 0 for number in my_list]
```



### 16. Créez une fonction qui prend un nombre en argument et renvoie ce nombre à la puissance 4


```python
def my_fonction:
    print(number*number*number*number)
```

```python
def my_fonction()
    return(number**4)
```



### 17. Testez cette fonction en lui passant le chiffre `n` de votre choix et en affichant le resultat sous la forme :

`A la puissance 4 le nombre 3 est égal à 81`


```python
def my_fonction(number):
print(number**4)
```

```python
n = 4
n_power = my_function(n)
print('A la puissance 4 le nombre {n} est égal à {n_power}')
```

```python
n = 4
n_power = my_function(n)
print(f'A la puissance 4 le nombre {n} est égal à {n_power}')
# indice : refactorisez
```



### 18. Toujours en list comprehension, créez une troisieme list qui contiendrait toutes les puissances 4 de votre seconde liste

```python
my_third_list = [number**4 for number in my_list]
```



### 19. Si `my_function()` comportait des operations plus complexes, comment pourriez vous l'integrer à votre liste comprehension ?

*Pas de réponse proposée*



### *A partir d'ici certains énoncés necessiteront de repasser dans le terminal, a vous de trouver quand*



### 20. Requetez l'[API suivante](https://opengraph.lewagon.com/?url=https://www.lewagon.com) afin d'avoir un json dans un dictionnaire

```python
my_dict = requests.get(https://opengraph.lewagon.com/?url=https://www.lewagon.com)
```

```python
data = [{key:value}]
response = request.get("https://opengraph.lewagon.com/?url=https://www.lewagon.com").json()
result = response.append(data)


### 21. Affichez les clés de ce dictionnaire. Quel est le type de la valeur associée à la clé `data` ? Combien d'éléments comporte-t-elle ?

*Pas de réponse proposée*



### 22. Depuis votre notebook, installez la librairie beautifulsoup4 (4.11.1) et importez là

```python
pip import beautifulsoup
```

```python
curl beautifulsoup4
```



### 23. Quel langage venez-vous d'utiliser ?

```
l'anglais (lol)
```



### 24. Telechargez le code html de [cette page](https://recipes.lewagon.com/) dans un fichier page.html

```bash
curl https://recipes.lewagon.com/
```



### 25. Puis supprimez ce même fichier

*(Oui oui, ça n'a servi à rien de le télécharger)*

```bash
del page.html
```



### 26. Telechargez le code html de [cette page](https://recipes.lewagon.com/), cette fois ci dans un objet beautifulsoup, assigné dans une variable

```python
code_html = BeautifulSoup.get("https://recipes.lewagon.com/")
```

```python
html = requests.get("https://recipes.lewagon.com/").json()
data = BeautifulSoup(html)
```



### 27. Corrigez ce code permettant de recuperer le titre de la premiere recette dans une string

<details><summary>Indice</summary>

**Balise de la premiere recette :**

```hmtl
<div class="recipe-details">[...]</div>
```
**Balise contenant le titre :**

```hmtl
<p class="recipe-name">10 Minute Brownies</p>
```

</details>

```python
url = https://recipes.lewagon.com/
html = requests.get(url).text
data = BeautifulSoup(html, "html.parser")
data = data.find_all('div', class_= 'recipe-details')[0])
data.find('p', class_= 'recipe-name').string
```

<details><summary>Solution</summary>

```python
# avec l'import
from bs4 import BeautifulSoup
url = "https://recipes.lewagon.com/"
html = requests.get(url).text
data = BeautifulSoup(html, "html.parser")
data = data.find_all('div', class_= 'recipe-details')[0]
print(data.find('p', class_= 'recipe-name').string)
```

</details>



### 28. Adaptez et packagez le code précedent en une fonction qui permettrai de recuperer n'importe quelle titre de recette en donnant son numero

*(1 -> premier titre, 3 -> troisieme titre etc)*


<details><summary>Solution</summary>

```python
def scrape_title(recipe_number):
    url = "https://recipes.lewagon.com/"
    html = requests.get(url).text
    data = BeautifulSoup(html, "html.parser")
    data = data.find_all('div', class_= 'recipe-details')[recipe_number-1]
    return data.find('p', class_= 'recipe-name').string
```

</details>



### 29. Testez cette fonction sur la 5e recette, et affichez le resultat

*Pas de réponse proposée*



### 30. (Optionnel) Réordonnez les cellules de ce notebook de façon plus logique qu'actuellement

*Pas de réponse proposée*



### 31. Après l'avoir sauvegardé, quittez votre jupyter notebook

*Pas de réponse proposée*



### 32. Quelle commande utiliser pour verifiez les modifications apportées au repo ?

*Pas de réponse proposée*



### 33. Quelle commande utiliser pour ajouter votre fichier jupyter notebook à git

*Pas de réponse proposée*



### 34. Quelle commande utiliser pour créez un commit propre contenant cet ajout

*Pas de réponse proposée*



### 35. Quelle commande utiliser pour pousser ce commit sur git

*Pas de réponse proposée*
