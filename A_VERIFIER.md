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

## Chapitre II — Afficher et demander (relecture du 2026-09-23)

Appliqués : `input()` enseigné (3 temps, « Saisir x », réponses simulées),
piège corrigé (`age + 1` → TypeError, pourquoi du texte), 2-6 (espace des
questions), 2-7 remplacé (un seul ordre valide sur 24, pratique `int()`),
`int()` et « renvoie » définis, `str()` enseigné, `end=""` expliqué, rappel
du chapitre I, « pourquoi demander », résumé « À retenir », nouvel exercice
2-8 (carré, `int(input())`). Restent :

- [ ] **2-2 et 2-4** : refont ce que le chapitre I a déjà fait faire, et leurs
  indices donnent la solution. Indices proposés — 2-2 : « Hello est un texte
  fixe, pas une boîte : qu'est-ce qui dit à Python de le recopier tel quel ? » ;
  2-4 : « Mélange un texte fixe et le contenu d'une boîte, séparés par une
  virgule, comme print("Level:", level) au chapitre I. Le nom de la boîte ne
  prend pas de guillemets. » Ou remplacer 2-4 par un exercice avec `+`
  (prenom = "Alice", nom = "Martin" → AliceMartin).
- [ ] **2-5** : `name = input("Name? ")` puis `print("Hi Alice")` en dur est
  accepté. Ajouter `useVars:["name"]` (comme 1-6 et 2-8).
- [ ] **ValueError** (explication d'erreur, ~l.2044) : si l'élève tape 2.5,
  `int("2.5")` plante. Ajouter « Si c'est un nombre à virgule, utilise
  `float()` au lieu de `int()` », et citer `float(input(...))` une fois dans le
  cours ou l'aide-mémoire. « uniquement des chiffres » est approximatif
  (`int(" -7 ")` vaut -7).
- [x] **TypeError hors collage** (`"7" * "7"`) → carte dédiée ajoutée
  (« Multiplication impossible avec ce texte »), et la carte « can only
  concatenate » conseille d'abord `int()` si le texte vient d'`input()`.
- [ ] **Carte « can only concatenate »** (défaut ancien) : pour `"a" + [1]`, le
  texte dit « un nombre de l'autre » alors que c'est une liste. N'écrire
  « un nombre » que si `m[1]` vaut `int` ou `float`, sinon « une valeur de
  type ${m[1]} ».
- [ ] **Glossaire** : « Fonction » ne parle que de `def` (contredit les
  chapitres I et II, qui appellent déjà fonctions `type()`, `print()`, `int()`).
  Proposition : « Une machine à laquelle on donne des valeurs entre
  parenthèses, et qui fait une action (print affiche) ou te renvoie un résultat
  (int("15") donne 15), comme f(x) en maths. Certaines existent déjà ; tu
  apprendras à construire les tiennes avec def. » Ajouter « Saisie (input) » et
  « Conversion » ; dans « Retourner », préciser que input() renvoie aussi une
  valeur.
- [ ] **Image bouche / oreille** (1er paragraphe du cours) : « il ne voit
  rien » puis « oreille » → « il n'entend rien et ne dit rien ». Préciser que
  input pose une question et écoute ce que tu tapes.
- [ ] **Textes en anglais dans les consignes FR** (« Name? », « Hi », « Line
  1 ») : ajouter une phrase dans le cours — « Dans les exercices, les textes
  affichés sont en anglais, pour que la réponse attendue soit la même dans les
  deux langues. » Dans la version EN du cours, l'exemple garde « Bonjour ».
- [ ] **EN, explication d'erreur** (~l.1999) : « Python is adding a int and a
  str » → article et types traduits (« a whole number and text »).

## Chapitre III — Conditions (relecture du 2026-09-23)

Appliqués (points 1 à 12) : `=` / `==` démêlés (← contre « est égal à »,
image du serveur, piège dans les deux sens), carte d'erreur `=`/`==` élargie,
`else` enseigné (Si / Alors / Sinon), ordre des `elif` (fonction par
morceaux, contre-exemple), indentation (même décalage, 4 espaces = convention,
piège de la 2e ligne non décalée), `%` (reste de la division euclidienne),
3-2 / 3-3 / 3-4 / 3-6 passés à `input()` avec essais « deuxième réponse »
(3-4 : deux essais, un par branche), 3-5 consigne + `useVars`, `and`/`or`,
≤ ≥ ≠, résumé « À retenir », indices 3-2 / 3-4 / 3-7. Restent :

- [ ] **13. 3-3 et 3-7 refont le programme du schéma** (age ≥ 18 → Adult /
  Minor), qui est aussi l'exemple du `else` dans le cours. Proposition pour
  3-7 : ajouter une ligne `print("End")` hors du bloc (sortie `Adult` puis
  `End`, consigne « une ligne n'est pas décalée, elle s'exécute dans tous les
  cas »). Pour 3-3, choisir un autre seuil ou un autre contexte.
- [ ] **14. « emprunte l'une des deux voies »** (1er paragraphe) : ajouter
  « Parfois, la voie « faux » est simplement : ne rien faire et continuer. »
- [ ] **15. Aide-mémoire, section Conditions** : ajouter la ligne
  `x = 5  /  x == 5` (« range 5 dans x (←) / demande « x est-il égal à 5 ? » ») ;
  `elif` « testé seulement si **tous** les précédents sont faux » ; `not` est
  listé mais n'est enseigné nulle part (l'enseigner en une ligne ou le
  retirer) ; « Erreurs fréquentes » : ajouter « = au lieu de == ».
- [ ] **16. Glossaire** : « Booléen » emploie « renvoie » (jargon du chapitre
  des fonctions) → « C'est le résultat d'une comparaison comme 10 > 5 :
  oui (True) ou non (False) » ; ajouter « Bloc » et « Comparaison (==) » ;
  l'exemple de « Condition » double celui d'« Indentation » (en donner un avec
  `else`).
- [ ] **17. Carte « Décalage inattendu »** (unexpected indent) : l'explication
  dit qu'aucune ligne au-dessus n'ouvre de bloc, ce qui est faux quand la
  ligne est simplement plus décalée que les autres lignes de son bloc. →
  « Cette ligne est plus décalée que prévu : soit aucune ligne au-dessus
  n'ouvre de bloc avec `:`, soit elle est plus à droite que les autres lignes
  de son bloc. »
- [ ] **3-5 : le cas « faux » n'est jamais testé** (pas d'input ni de
  retest). `if age and has_license: print("Drive")` est accepté (sans le 18
  ni le else) ; `useVars` empêche seulement de recopier les valeurs en dur.
  Piste : `has_license = input("License? ") == "yes"` avec un retest, ou
  accepter cette limite.
- [ ] **Image du serveur** (section 1) : prof-pedagogue relève que « Pose
  l'assiette sur la table 5 » / « Est-ce bien la table 5 ? » mélange les rôles
  (5 y désigne la boîte, alors que dans `x = 5` c'est le contenu). Variante
  proposée : « Mets 5 couverts sur la table x » (= `x = 5`) / « Y a-t-il bien
  5 couverts sur la table x ? » (= `x == 5`). Conservée telle quelle en
  attendant la décision (image validée explicitement).
- [ ] **18. Schéma if/else** : étiquettes « vrai (True) » / « faux (False) »,
  légende « En Python : la branche vrai est sous le if, la branche faux sous
  le else ».

## Constaté ailleurs dans l'appli

- [x] **`str()` n'est enseigné dans aucune leçon** → enseigné au chapitre II
  (2026-09-23), juste après `int()`.
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
