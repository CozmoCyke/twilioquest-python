# Notes du procès de Toledo
Une brève recherche dans la zone entourant cette barrière révèle une autre entrée du journal de Toledo Van Possum.

<blockquote>
21 août 2016

<hr/>

<p>
Notre recherche dans la Chambre du Rituel d'Initiation continue, bien que je commence à douter que l'indice final existe. Heureusement, nous avons finalement rencontré une autre épreuve - l'épreuve des chemins de branchement. En utilisant ce que j'ai appris sur les booléens et la logique de comparaison, je dois maintenant apprendre à brancher mon code dans de multiples directions pour prendre en charge de nombreux scénarios différents.
</p>

<p>
Si je parviens à sortir de cette chambre, je demande au programme TwilioQuest de doubler mes honoraires habituels.
</p>

<p>
--TVP
</p>
</blockquote>

## Trucs et astuces

Tout au long de l'entrée du journal, vous trouverez quelques passages utiles.

<details>
<summary>Comment écrire un code qui se branche dans plusieurs directions ?</summary>

Nous avons déjà vu l'instruction `if` qui nous permet d'exécuter un bloc de code lorsqu'une certaine condition est vraie. Pour prendre en charge plus d'une condition, nous devons également nous familiariser avec les instructions `elif` et `else`.

```python
dinner_name = "kale"

if dinner_name == "tacos":
    print("Des tacos pour le dîner - tout à fait !")
elif dinner_name == "pizza":
    print("Pizza - on ne peut pas se tromper !")
else:
    print("Ok - c'est mieux que d'avoir faim ?")
```

Vous pouvez utiliser la [logique de comparaison] (https://docs.python.org/3/library/stdtypes.html#comparisons) pour déterminer si un bloc de code doit être exécuté ou non. Les instructions conditionnelles comme celle-ci ne peuvent avoir qu'un seul bloc `if` et `else`, mais votre code peut inclure autant de blocs `elif` que nécessaire.

Un bloc `elif` fonctionne comme une instruction if - ces comparaisons sont toutes exécutées dans l'ordre, et si la première est évaluée à `Vrai`, aucune des autres conditions ne sera évaluée. L'ordre est important dans ce cas !

Une instruction `else` déclare un bloc de code qui sera exécuté si aucune des autres conditions n'est vraie.

</details>

<details>
<summary>Comment convertir les entrées de mon script (chaînes de caractères) en nombres?</summary>.

Pour réaliser ce défi, vous devrez comparer les valeurs des nombres transmis à votre script en tant qu'arguments. Cependant, lorsque vous les lisez initialement dans `sys.argv`, ces valeurs seront des __chaînes__ et non des __nombres__. Pour effectuer des comparaisons numériques, nous devrons convertir les arguments en __entiers (nombres entiers)__ ou __floats (nombres décimaux)__. Le code ci-dessous montre comment convertir les entrées en nombres entiers.

```python
first_num = int(sys.argv[1])
second_num = int(sys.argv[2])
sum_to_use = first_num + second_num
```

</details>

<details>
<summary>Que dois-je faire pour terminer cet essai?</summary>

Créez un fichier appelé `branching.py` dans votre dossier de code situé ici : 

```bash
<%= env.TQ_PYTHON_CODE_PATH.value %>
```

Créez un programme qui __accepte deux arguments de ligne de commande__ - deux nombres entiers  que vous devez additionner. En fonction de la __somme de ces nombres__, votre code devrait afficher des messages différents.

* Si la somme des nombres est __inférieure ou égale à zéro__, affichez le texte : <div>`Vous avez choisi le chemin de l'indigence.`</div>
* Si la somme des nombres est __1 à 100 (y compris 100)__, affichez le texte suivant : <div>`Vous avez choisi le chemin de l'abondance.`</div>
* Si la somme des nombres est __plus grande que 100__, affichez le texte : <div> `Vous avez choisi le chemin de la démesure.`</div>.

Exemple d'exécution de script:

```bash
python3 branching.py 30 200
```

Exemple de résultat :

```bash
Vous avez choisi la voie de l'excès.
```

Une fois que votre script peut traiter les trois conditions correctement, cliquez sur le bouton *HACK* !

</details>