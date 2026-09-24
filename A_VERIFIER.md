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
- [x] **Listes (chapitre V)** : `b = a` puis `a.append(...)` modifie aussi `b`
  → traité au chapitre V (image du classeur et des étiquettes, `.copy()`,
  quiz 5-8), avec un renvoi d'une phrase au chapitre I (2026-09-24).

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
- [x] **Image du serveur** (section 1) : l'ancienne version (« la table 5 »)
  faisait de 5 la boîte au lieu du contenu → remplacée par « Mets 5 couverts
  sur la table x » (`x = 5`) / « Y a-t-il bien 5 couverts sur la table x ? »
  (`x == 5`).
- [ ] **18. Schéma if/else** : étiquettes « vrai (True) » / « faux (False) »,
  légende « En Python : la branche vrai est sous le if, la branche faux sous
  le else ».

## Chapitre IV — Boucles (relecture du 2026-09-23)

Appliqués (points 1 à 13) : exercices 4-2 à 4-6 passés à `n = int(input())`
avec essais « deuxième réponse » (une réponse en dur ne passe plus), nouveaux
contrôles `need` / `ban` (4-4 : while exigé, for interdit), syntaxe du `for`
(« Pour i allant de »), `range` = intervalle [a ; b[, `range(n)`, `while` =
« Tant que » (condition pour continuer), tableau d'état, boucle infinie,
tirelire, `print` dans / après la boucle, boucles imbriquées, suites (terme
de rang n, seuil 7 → 128, somme vérifiée par n(n+1)/2), nouvel exercice 4-8
« Seuil », 4-7 sans liste, résumé en 6 points. Restent :

- [ ] **14. Indices** : relire ceux de 4-2 et 4-4 une fois les exercices
  stabilisés (ils ont été réécrits avec les nouveaux exercices).
- [ ] **15. Aide-mémoire, section Boucles** : « `i = i + 1` indispensable dans
  un while » est trop étroit (les while suivants modifient `essai`, `u`…) →
  « dans un while, modifier la variable testée (ex. i = i + 1), sinon boucle
  infinie » ; ajouter `for i in range(n):` (n tours, i de 0 à n − 1) et
  l'accumulateur ; `for x in liste:` relève du chapitre V.
- [ ] **16. Glossaire** : ajouter Range, Compteur (employé plus loin sans
  définition), Accumulateur, Boucle infinie ; entrée Boucle : « for =
  Pour … allant de, while = Tant que ».
- [ ] **17. Carte d'erreur `range(n / 2)`** (`'float' object cannot be
  interpreted as an integer`) : elle conseille « range(3) et non range("3") »,
  hors sujet. Tester `m[1]==="float"` → « tu as donné un nombre à virgule ;
  `/` donne toujours un float, convertis avec int(...) ».
- [ ] **18. TIMEOUT** : afficher les ~20 premières lignes de la sortie sous le
  message (voir « 1 1 1 1… » est le meilleur indice d'une boucle infinie) ;
  envisager de plafonner le tampon de sortie (plusieurs Mo en 5 s).
- [ ] **19. Détails** : schéma whileloop sans flèche de sortie (« faux → on
  sort ») et étiquette « 3. modifier la variable » peut-être trop large pour
  sa boîte ; second quiz sur un `print` décalé dans la boucle ;
  `range(a, b, pas)` jamais enseigné (pourrait illustrer une suite
  arithmétique de raison 2).

## Chapitre V — Listes (relecture du 2026-09-24)

Appliqués (points 1 à 13) : `b = a` et les listes (classeur, étiquettes,
classeur scellé, réaffecter ≠ modifier, `.copy()`, renvoi au chapitre I,
quiz 5-8), indice = rang (u₀, rez-de-chaussée), IndexError (u₅ jamais
calculé, `range(len(L))`, `L[-1]`), `L[i] = v`, `append` et la notation
« méthode » (piège `L = L.append(x)` → None), listes en compréhension
({x² | x ∈ …}, filtre `if`), séries statistiques (effectif, moyenne, max,
min) et termes d'une suite gardés, `for x in L` relié à `range`, cartes
d'erreur « None » et « texte + liste », `useVars` / `need` sur 5-2 à 5-6,
5-3 et 5-4 autonomes, 5-3 et 5-7 distincts du cours, résumé en 6 points.
Restent :

- [ ] **14. Fruits en anglais dans les exercices FR** (`"apple"`) alors que le
  cours FR dit « pomme » ; le schéma EN affiche `["apple", …]` alors que le
  code (commun aux deux langues) utilise `"pomme"`.
- [ ] **15. Quiz 5-1** : l'option `["b"]` → `['b']` (Python n'affiche jamais
  de guillemets doubles pour une liste) ; son explication « Les crochets
  simples renvoient… » est obscure → « fruits[1] donne le contenu de la case
  1, c'est-à-dire b tout seul ; print n'affiche des crochets que pour une
  liste entière ».
- [ ] **16. 5-6 classé « hard »** alors qu'il est le plus facile du chapitre
  (surtout maintenant que le cours montre `len` et `sum`) : le passer en
  « easy », ou le transformer en moyenne d'une série (notes = [12, 15, 9, 14]
  → effectif puis moyenne, sortie `4` puis `12.5`).
- [ ] **17. Cartes d'erreur manquantes** : `L["0"]` / `L[input()]` / `L[n/2]`
  (« list indices must be integers or slices, not str/float ») → « Un indice
  doit être un nombre entier ; s'il vient de input(), convertis-le avec int() ;
  pour une moitié, utilise // » ; `L = L + 3` (« can only concatenate list
  (not "int") to list ») → « Pour ajouter un élément, utilise L.append(3) ».
- [ ] **18. Aide-mémoire et glossaire** : `l` se confond avec `1` (utiliser
  `L` ou `notes`) ; ajouter `L[i] = v`, `b = L.copy()`,
  `[n * n for n in range(5)]` ; la ligne TypeError « entre un texte et un
  nombre » → « … ou une liste » ; glossaire : entrée « Liste » avec l'image du
  classeur et `.copy()`, « Indice » = le rang comme n dans uₙ, entrées
  Élément, append, len, Liste en compréhension ; l'exemple de « Méthode »
  (`mot.upper()`) renvoie à un chapitre ultérieur et ne prévient pas que
  certaines méthodes modifient la valeur (append) et d'autres en renvoient une
  nouvelle (upper).
- [ ] **Chapitre XIII et exercice ~l.1000** : le chapitre V montre maintenant
  la liste des termes d'une suite (u₀ = 2, +3) et `sum(L) / len(L)` ; vérifier
  que les exercices ultérieurs qui demandent une moyenne par accumulateur
  précisent « sans utiliser sum », et que la liste des termes du chapitre XIII
  ne fait pas doublon.

## Chapitre VI — Fonctions (relecture du 2026-09-24)

Appliqués (points 1 à 12) : pont f(x) ↔ def (tableau maths/Python, rappel
de type() et input()), définir / appeler (def = define, « Soit f… » ne
calcule rien), paramètre / argument, variable muette, return ou print (machine
à jus / haut-parleur, fonction sans return → None, lien avec append), deux
paramètres (moyenne), portée corrigée (brouillon ; une fonction peut lire le
dehors, ce qui est créé dedans n'existe pas dehors), suites u = f(u),
résumé en 6 points ; exercices : def / return exigés (6-2 à 6-6), 6-4 avec
add(3, 4) * 10, 6-5 « False sinon », 6-6 devenu « Tableau de valeurs »
(f(x) = x² − 2x) ; cartes d'erreur : calcul avec None (plus de conseil
str()/int()), fonction appelée avant sa définition, variable locale utilisée
dehors, argument manquant (nomme le paramètre), décalage manquant après def.
Restent :

- [ ] **13. Cartes secondaires** : trop d'arguments (`square(5, 9)` →
  « takes 1 positional argument but 2 were given » : la regex actuelle exige
  « takes 0 ») ; `return` hors d'une fonction (« 'return' outside function »,
  carte générique trompeuse) ; `UnboundLocalError` (modifier une variable du
  dehors dans une fonction) → carte « passe la valeur en paramètre et renvoie
  le résultat » (ne pas enseigner `global`). Compléter aussi la carte générale
  None : « … par exemple une fonction sans return ». Dans `diagnose` : si la
  sortie contient une ligne `None` inattendue et que le code a un `def` sans
  `return`, afficher le même conseil.
- [ ] **Réponses en dur encore possibles en 6-4 et 6-5** : `def add(a, b):
  return 7` suivi des deux appels, ou la bonne fonction suivie de `print(7)` /
  `print(70)`, passent (`need def, return` ne suffit pas). Piste : exiger que le
  nom de la fonction apparaisse au moins 3 fois (définition + deux appels),
  avec un message dédié (le message `useVarsB` parle de « boîte »).
- [ ] **`nearestName`** propose à tort un nom d'une lettre (`print(y)` → « Tu
  as peut-être voulu écrire f ») : ne proposer que si la distance est
  strictement inférieure à la longueur du nom.
- [ ] **Rappels type() / input() du 1er paragraphe** : prof-pedagogue suggère
  de les sortir dans une phrase après le premier exemple de code (paragraphe
  dense) ; conservé tel quel car validé par la mère.
- [ ] **14. Schéma de la machine** : « le paramètre entre » → « la valeur 5
  entre dans n » ; la flèche `print` part d'une fonction qui ne contient aucun
  print → « print, seulement s'il est dans le bloc » ; la flèche `return` ne
  mène nulle part → « return renvoie 25 au programme » ; en EN, `square(n)`
  alors que le code dit `carre` (mettre `carre` dans les deux langues).
- [ ] **15. Niveaux et noms** : 6-1 « hard » (c'est la démonstration du
  cours), 6-7 « hard » pour trois lignes ; noms anglais (greet, add, is_even)
  dans les consignes FR — ou une phrase dans le cours : « les noms de fonctions
  sont libres ; les exercices utilisent des noms anglais ». 6-7 : indice avec
  le pourquoi (« Python lit de haut en bas, une fonction pas encore définie lui
  est inconnue ») ; 6-3 recopie presque l'exemple `bonjour(nom)` du cours ;
  quiz manquant sur le piège None (`def f(x): print(x + 1)` puis
  `y = f(2); print(y)` → 3 puis None).
- [ ] **16. Glossaire et aide-mémoire** : « Fonction » (ne parle que de def)
  → « machine qui reçoit une valeur et en renvoie une autre, comme f en
  maths » ; « Paramètre » : variable muette, le x de f(x) ; « Argument » : en
  maths, le nombre dont on calcule l'image ; « Retourner » → « Renvoyer
  (return) », « c'est l'image f(x) ; sans return, la fonction renvoie None » ;
  « Portée » : ajouter « ainsi que toute variable créée dans la fonction ».
  Aide-mémoire : `def f(x): return x*x + 1` ↔ f(x) = x² + 1 ; `y = f(3)` ;
  `print` dans la fonction → renvoie None ; « rend » → « renvoie » ; ligne
  NameError : « … ou variable qui n'existait que dans une fonction ».

## Chapitre VII — Le texte (relecture du 2026-09-24)

Appliqués (points 1 à 15) : « exactement comme une liste » corrigé (se lit
comme une liste, ne se modifie jamais : classeur scellé, « regarde à gauche
du = », `mot = "P" + mot[1:]`), les deux familles de méthodes face à face
(append seul / `mot = mot.upper()`, machine à jus, « peut-on modifier ce
classeur ? »), `len` = nombre de caractères (espaces compris), casse, rappel
input / "3" contre 3, indice = rang et IndexError pour les chaînes, tranches
([a ; b[, bornes omises), `.replace` et `.lower` montrés, parcours lettre par
lettre, compteur (tirelire conditionnelle) et fréquence = compteur / len,
palindrome, f-string (texte à trous, piège du f oublié), résumé en 7 points ;
exercices : 7-2, 7-3, 7-4, 7-6 avec input et retest, useVars / need, 7-3 à
7-7 distincts du cours, nouvel exercice 7-8 (tranches sur une date) ; cartes
d'erreur : texte non modifiable, position hors du texte, indice non entier,
méthode de liste appelée sur un texte. Restent :

- [ ] **16. Aide-mémoire « Texte »** : ajouter `len(mot)` (caractères,
  espaces compris), `mot[-1]`, `mot[:3]` / `mot[3:]`, `mot = mot.upper()`
  (« renvoie un nouveau texte : il faut le ranger »), `for lettre in mot:`,
  `mot[0] = "P"` (« impossible : TypeError ») ; remplacer « renvoie une copie
  en majuscules » par « renvoie un nouveau texte en majuscules (mot ne change
  pas) » ; ligne IndexError : « … ou du texte ».
- [ ] **17. Glossaire** : « Chaîne de caractères » → « on la lit, on ne la
  modifie jamais (immuable) » ; « Méthode » : l'entrée compare à `upper(mot)`,
  qui n'existe pas → expliquer les deux familles (liste : modifie sur place et
  renvoie None ; texte : renvoie un nouveau texte à ranger) ; nouvelles
  entrées Immuable, Tranche, f-string.
- [ ] **18. Schéma `strindex`** : les étiquettes « positions » et « positions
  depuis la fin » commencent probablement sous les premiers chiffres (0 / −6)
  et les chevauchent (estimé par calcul, pas vu à l'écran). Piste : élargir la
  zone et décaler les cases, ou raccourcir en « indice » / « depuis la fin ».
- [x] **« L'indice est le rang »** (chapitres V et VII) → uniformisé le
  2026-09-24 : « indice » pour Python (indice 0, indice 1), « rang » réservé
  aux suites (u₀ = terme de rang 0), avec le pont « l'élément d'indice i
  correspond au terme de rang i ».
- [ ] **19. EN** : le FR dit maintenant « tranche », l'EN « slice » (cohérent) ;
  les phrases d'exercice restent en français dans la version EN (7-5 le
  signale ; « Alice a 16 ans » du cours ne le signale pas).

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
