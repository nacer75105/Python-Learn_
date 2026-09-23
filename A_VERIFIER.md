# À vérifier / à faire — Python-Learn_

Points relevés lors des relectures (relecteur-python + prof-pedagogue),
reportés pour être traités en un seul passage. Tout le contenu est dans
`index.html`.

## Chapitre I — Variables (relecture du 2026-09-23)

Les points 1 à 12 de la relecture ont été appliqués, ainsi que la vérification
de 1-6 (valeurs recopiées en dur) et le déplacement de `int()`/`str()` dans
l'aide-mémoire. Restent :

- [ ] **1-2** : sa solution (`age = 15` / `print(age)`) est identique au premier
  exemple du cours. Seul exercice du chapitre dans ce cas (1-3 à 1-6 ont été
  corrigés). Acceptable pour un tout premier exercice, sinon variante proposée :
  « Crée une variable year qui vaut 2026, puis affiche-la » (sortie `2026`).
  Son **indice** donne aussi la solution mot pour mot. Proposition :
  « Relis le premier exemple du cours : une ligne pour ranger la valeur dans la
  boîte, une ligne pour l'afficher. Attention, `print("age")` afficherait le mot
  age, pas son contenu. »
- [ ] **1-3, consigne** : le titre annonce « Trois types » mais la consigne n'en
  parle pas. Ajouter « (un int, un float, un str) » et faire observer que les
  guillemets ne s'affichent pas.
- [ ] **1-4** : recopie exactement l'exemple `score` du cours, pour une
  difficulté « medium ». Variante proposée : `vies = 3`, afficher, puis
  `vies = vies - 1`, afficher (sortie `3` puis `2`). L'identifiant `1-4` reste
  le même : si l'exercice a déjà été réussi, il restera compté comme fait.
- [ ] **1-5, consigne** : préciser « un print par ligne ».
  `print(type(5), type(3.14), type("hello"))` est refusé alors que la consigne
  ne l'interdit pas. (Touche un peu la justesse : une réponse raisonnable est
  refusée.)
- [ ] **Piège 15 / "15"** : dire pourquoi `+` colle deux textes. Image proposée :
  deux morceaux d'un numéro de téléphone, `"06" + "12"` donne `"0612"`.
- [ ] **Glossaire** : ajouter « Affectation » (`nom = valeur`, notée ← en
  algorithmique ; réaffecter = ranger une nouvelle valeur qui remplace
  l'ancienne). Compléter « Variable » (on la remplit avec `=`, « range
  dans »), « Chaîne de caractères » (son type Python est `str`), « Booléen »
  (exemple : `10 > 5` vaut `True`).
- [ ] **Quiz 1-1, EN** : la version anglaise omet « Ne l'exécute pas » →
  "Read the program in your head before answering. Don't run it."
- [ ] **Sous-titre du cours** : « tu écriras du code juste après », alors que le
  premier exercice est un quiz → « tu t'entraîneras juste après » / "you will
  practise right after".

### Relecture de confirmation du chapitre I (2e passage, 2026-09-23)

Appliqués : A (le cours ne recopie plus les solutions de 1-4, 1-5, 1-6),
B (5 titres de section + résumé « À retenir »), C (« en lui rangeant une
nouvelle valeur »), E (« Presque ! » explique le pourquoi, indice ouvert au
2e essai), F (« pour l'instant »), G (mot réservé, ne pas nommer une boîte
print/type), H (exemple age / "age" juste après son piège). Restent :

- [ ] **D. Paragraphe `x = x + 3` trop dense** (3 images d'affilée). Le couper
  en deux : (A) l'ordre en deux temps + `x ← x + 3` ; (B) le lien avec la
  suite. Nuancer « c'est exactement une suite » : la boîte ne garde que le
  **dernier** terme. Formulation plus précise : « chaque exécution de
  `x = x + 3` fait passer du terme uₙ au terme uₙ₊₁ ».
- [ ] **I. « Tu connais déjà ce sens-là : age ← 15 »** : beaucoup d'élèves ont
  fait l'algorithmique de Seconde directement en Python. → « Si tu as déjà vu
  en maths la notation age ← 15, c'est exactement ça… »
- [ ] **J. Image g(f(x))** pour `print(type(15))` : la composée n'est formalisée
  qu'en Terminale. Remplacer par √(9 + 16) à la calculatrice (on calcule
  l'intérieur, 25, puis la racine, 5).
- [ ] **K. Ton** : « touche Ans (ou rép sur TI) » ; « pour une matheuse » →
  « quand on fait des maths » (l'EN est déjà neutre).
- [ ] **L. Raccord « posons a = 3 » / « = ne veut pas dire égal »** : ajouter
  « “Posons a = 3” s'en approche, avec une différence : en maths, a garde
  cette valeur tout l'exercice ; en Python, on pourra la changer. » Et à la fin
  du bloc « 2. Changer une valeur » : « C'est comme la touche Ans : chaque
  nouveau calcul écrase le précédent. »
- [ ] **M. `varUses` (vérification de 1-6)** : un nom écrit seul sur une ligne
  (`name` puis `print("Name: Alice")`) compte comme une utilisation ; les
  f-strings `rf"…"`, `fr"…"`, `f"""…"""` sont refusées à tort. Piste : ne
  compter que les utilisations dans les lignes contenant `print(`, et gérer
  les préfixes de deux lettres et les triples guillemets.
- [ ] **N. Consigne de 1-6** : `Affiche "Name: Alice"` — une débutante peut
  recopier les guillemets dans la sortie. → « Affiche la ligne Name: Alice
  puis la ligne Age: 16 ».
- [ ] **Listes (chapitre V)** : `b = a` puis `a.append(...)` modifie aussi `b`
  (même liste). Le chapitre I le prépare (« en lui rangeant une nouvelle
  valeur »), mais aucun passage du chapitre V ne le traite : ajouter un piège.

## Constaté ailleurs dans l'appli

- [ ] **`str()` n'est enseigné dans aucune leçon.** Il n'apparaît que dans
  l'aide-mémoire (section « Afficher et demander ») et dans les explications
  d'erreur (TypeError). À introduire dans le cours du chapitre II, qui traite
  déjà `int(input(...))`.
- [ ] **Bouton solution** : après l'avoir cliqué, les numéros de ligne restent
  à « 1 » tant que l'élève ne tape rien (`c.value=x.sol` ne déclenche pas
  `input`). Correction : appeler `drawGutter()` dans ce gestionnaire.
- [ ] **Changement de langue sur un exercice « écrire » ou « remettre en
  ordre »** : le code tapé est conservé, mais la sortie affichée, la carte de
  résultat, l'indice ouvert et la mise en évidence du bouton solution sont
  effacés.

## Programme officiel de Première (BO spécial n°1 du 22/01/2019)

- [ ] **Listes en compréhension** : au programme (« Générer une liste en
  extension, par ajouts successifs ou en compréhension »), absentes de l'appli.
- [ ] **Simulation de probabilités** : simuler une variable aléatoire, moyenne
  d'un échantillon de taille n, écart à l'espérance, Monte-Carlo (aire sous la
  parabole, π). Absent de l'appli.
- [ ] Autres exemples d'algorithmes du programme absents : factorielle,
  Syracuse / Fibonacci, sécantes, méthode d'Euler, Archimède (π), fréquence des
  lettres, espérance / variance.
- Note : la dichotomie (chapitre XIV) ne figure pas au programme de Première.
