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

## Chapitre VIII — Algorithmes classiques (relecture du 2026-09-24)

Appliqués (points 1 à 8 et 11) : cinq motifs, chacun avec son image, sa
question de maths et son piège. 1 : la tirelire en rappel (IV, VII), avec du
neuf : deux tirelires combinées (moyenne des notes ≥ 10). 2 : le champion
provisoire (concours de saut), le piège du 0 fantôme, le minimum et
l'étendue. 3 : le drapeau (boîte aux lettres), le piège du `else`. 4 : le
seuil en rappel du IV, avec un tableau d'état et la vérification par
n(n + 1)/2. 5 : le balayage (mode TABLE), avec le rectangle d'aire
x(10 − x) et l'encadrement de √2 par pas de 0,1, qui ouvre vers le
chapitre XIV. Le cours ajoute aussi l'image du papier peint pour « motif »,
x̄ et Sₙ, et un récapitulatif « quelle question → quel motif ».

Côté exercices, tous ont de nouvelles données, avec need, ban, useVars et
retest :
- 8-2 : un effectif et une fréquence ;
- 8-3 : `sum` interdit ;
- 8-4 : des températures négatives, pour que `maxi = 0` soit refusé,
  et `max`/`sorted` interdits ;
- 8-1 : le piège du minimum, placé après 8-4 ;
- 8-5 : une cible tapée, présente ou absente ;
- 8-6 : un capital à 5 %, soit une suite géométrique ;
- 8-7 : le minimum ;
- 8-8 (nouveau) : le minimum de x² − m·x + 5 sur [−10 ; 10] (m plutôt
  que a, pour ne pas le confondre avec le a de ax² + bx + c). Deux
  retests : m = 2 refuse le 0 fantôme, m = 20 refuse `range(-10, 10)`.

Après la relecture de confirmation :
- 8-3 (easy) passe avant 8-2 (medium) ;
- les indices de 8-5 et 8-6 ne dictent plus le code ;
- côté cours, le 0 fantôme devient « sauteur fantôme à 0 m », et le minimum
  passe au 100 m ;
- le champion à deux boîtes est expliqué pas à pas (10 − x, f(0) n'est pas un
  0 fantôme, `range(0, 11)`) ;
- l'encadrement de √2 est justifié (0.1 + 0.2, k = 10, tableau d'état) ;
- le récapitulatif distingue « combien d'éléments ? » (compteur) et « au bout
  de combien de tours ? » (seuil) ;
- l'indice de 13-4 précise que la tirelire démarre avec u₀.

Les renvois du chapitre XIII (motifs renumérotés, « chapitre IV »
pour la tirelire et la mise à jour d'une variable) et le guide ont été
corrigés. Restent :

- [ ] **9. Aide-mémoire** : créer une section « Algorithmes » avec les cinq
  motifs (initialisation, boucle, question à laquelle chacun répond, piège).
  La description de l'aide-mémoire dit « huit chapitres », alors que l'appli
  en compte quinze.
- [ ] **10. Glossaire** : les entrées Motif, Compteur, Accumulateur (tirelire),
  Champion provisoire (maximum/minimum), Drapeau, Seuil, Balayage et Étendue
  sont absentes.
- [ ] **12. Détails** :
  - le schéma `maxscan` : ses étiquettes chevauchent probablement les cases
    (non vu à l'écran) ;
  - 8-3 refuse `//` sans l'expliquer (la sortie 12.0 attend `/`) ;
  - sur une liste vide, `L[0]` et la moyenne plantent. Le cours le signale en
    une parenthèse (« cela suppose que la liste n'est pas vide ») ; à
    approfondir éventuellement avec `if len(L) > 0`.
- [ ] **Raccourcis encore acceptés** (relecteur-python, jugés acceptables) :
  - 8-4 et 8-3 n'ont pas d'input, donc pas de retest. Un « fantôme −100 »
    (`maxi = -100`), `.sort()` avec une boucle factice, ou `print(12.0)` après
    une boucle factice passent ; on peut rendre la liste variable si
    nécessaire.
  - 8-5 : `trouve = cible in nombres` plus une boucle factice passe (`in` ne
    peut pas être interdit, puisque `for … in` l'utilise).
  - 8-8 : la formule du sommet plus un `for`/`if` factices passe.
- [ ] **Image de la boîte aux lettres** : dans la réalité, aux États-Unis,
  c'est l'habitant qui lève le drapeau pour le courrier sortant. Le cours
  reste neutre (« comme dans les dessins animés américains »).

## Chapitre IX — Les dictionnaires (relecture du 2026-09-24)

Appliqués (points 1 à 13) :
- **Pourquoi en tête :** la note de Karim cherchée par indice avec deux
  listes, puis directement avec `carnet["Karim"]`.
- **Le carnet d'adresses,** qui prolonge le classeur du V : des cases
  numérotées d'un côté, des lignes qui commencent par un nom de l'autre.
  Clé, valeur et paire sont définies. L'étiquette sur la couverture est
  distinguée de la clé écrite à l'intérieur.
- **Syntaxe :** les guillemets (NameError sans eux), l'unicité des clés,
  l'ordre d'affichage (ordre de rangement, jamais utilisé pour chercher).
- **Écriture :** `d[k] = v` avec « regarde à gauche du = », et le contraste
  avec l'IndexError d'une liste.
- **Lecture sûre :** carte piège KeyError (étage qui n'existe pas,
  `ages[0]`), `.get` (machine à jus, None, valeur de secours), `in`
  (regarde les clés), `.items()` (deux boîtes par tour, tour par tour).
- **Deux liens maths :** le tableau de valeurs, c'est-à-dire une fonction
  sur un ensemble fini (f[-1] se lit « f de −1 », f(−2) = f(2),
  f[1.5] → KeyError), et le tableau d'effectifs (une rangée de tirelires,
  `.get(n, 0) + 1`, fréquence 0,5).
- **Résumé en 6 points.** Le schéma `dictbox` porte maintenant des libellés
  permanents « clé » et « valeur ».

Exercices : nouvelles données partout, useVars, need, ban et retest.
- 9-2 : `capitales`, avec une lecture au lieu de l'affichage complet, pour
  ne plus dépendre de l'ordre des clés.
- 9-3 : clé tapée au clavier.
- 9-4 : âge tapé au clavier.
- 9-5 : `score["Alice"] = score["Alice"] + pts`.
- 9-6 : prix des fruits.
- 9-7 : stock, avec un seul ordre valide sur 24.
- Nouveaux : 9-8 (tableau d'effectifs, `count` interdit, retest avec une
  valeur absente), quiz 9-9 (ajouter ou remplacer ?) et quiz 9-10 (`in`
  regarde les clés).

Cartes d'erreur ajoutées : KeyError (clé absente / indice numérique),
`.append` ou `.clé` sur un dictionnaire, ValueError « values to unpack »
(`.items()` oublié), `.items` sans parenthèses, et « un dictionnaire » au
lieu de « un dict » dans la carte « pas une fonction ». Restent :

- [ ] **14. Annexes :**
  - aide-mémoire : ajouter `KeyError` (« clé absente du dictionnaire »),
    `"a" in d` (« True si la clé a existe »), `d[x] = d.get(x, 0) + 1`
    (« compte une apparition de x ») ; écrire
    `for cle, valeur in d.items():` au lieu de k, v ;
  - glossaire : « Dictionnaire » → « un carnet d'adresses : chaque ligne
    associe une clé à une valeur ; on cherche par la clé, jamais par
    position » ; nouvelles entrées Clé, Valeur, KeyError.
- [ ] **15. Renvois vers le IX :** aucun autre chapitre n'utilise de
  dictionnaire. Pistes :
  - chapitre X : `try` / `except KeyError`, avec un renvoi à `.get` ;
  - chapitre XI (random) : compter des lancers de dé dans un dictionnaire
    et comparer les fréquences à 1/6 (sortie aléatoire : `random.seed`, ou
    une vérification déterministe comme `sum(effectifs.values())`).
- [ ] **Raccourcis encore acceptés** (jugés acceptables) :
  - 9-4 : `eleve = {"nom": "Alice", "age": int(input(...))}`, le
    dictionnaire écrit d'un coup ;
  - 9-5 : `score = {"Alice": 12 + pts, "Karim": 9}`, le dictionnaire
    reconstruit.

  Dans les deux cas, la saisie est bien utilisée, mais pas l'écriture
  `d[k] = …`.
- [ ] **9-8 :** un dictionnaire écrit en dur (`effectifs = {14: 3, 11: 2, 8: 1}`),
  plus un compteur `for`/`if` pour la fréquence, passe tous les contrôles.
  Il faudrait une vérification du type « commence vide » (un champ `needRe`,
  par exemple). Autres trous mineurs : en 9-2, un dictionnaire sans la France
  passe ; en 9-3, un `if cle == "titre"` qui aiguille vers deux lectures
  écrites en dur passe aussi.
- [x] La carte IndexError dit maintenant « indice » (et non plus
  « position ») ; elle couvre aussi l'écriture (`list assignment index out
  of range`). Fait le 2026-09-24.

Retouches de la relecture de confirmation :
- **Cartes d'erreur :**
  - la carte KeyError sur un nombre envisage les deux cas (clés texte
    confondues avec un indice, ou nombre absent d'un tableau d'effectifs →
    `d.get(n, 0)`) ;
  - elle signale une variable mise entre guillemets (`livre["cle"]`) ;
  - une faute de frappe sur une méthode (`d.item()`) est détectée ;
  - « cannot unpack non-iterable » est couvert ;
  - nouvelle carte pour `notes["Karim"]` sur une liste ;
  - phrase propre au dictionnaire ajoutée en anglais dans la carte « pas une
    fonction ».
- **Cours :**
  - `.get` sort de la carte piège pour un paragraphe à part (clé entre
    parenthèses) ;
  - la ligne `get(n, 0) + 1` est lue de droite à gauche, avec un tour par
    tour détaillé ;
  - la variante `in` est donnée en code ;
  - `.items()` : découpage de la ligne aux deux-points, noms des boîtes au
    choix ;
  - « pages » du classeur (V), NameError (VI), tirelire (IV et VIII) ;
    accolades montrées ;
  - Karim a 17 ans (et non plus 15, qui était aussi sa note) ;
  - EN : « address book » partout.
- **Exercices :** 9-6 passe en difficulté moyenne.

## Chapitre X — Gérer les erreurs (relecture du 2026-09-24)

**Programme officiel :** try/except ne figure pas au programme de Première
spé maths (BO spécial n°1 du 22/01/2019). La partie « Algorithmique et
programmation » se limite aux variables, conditions, boucles, fonctions et
listes. Le même texte exclut aussi les dictionnaires : « on se limite aux
listes sans présenter d'autres types de collections ». Les chapitres IX et X
sont donc marqués « (pour aller plus loin) » dans leur titre, et leur cours
s'ouvre sur une carte « Pour aller plus loin » (nouveau type de bloc `n`,
carte orange) qui cite le programme.

**Moteur d'exécution (point 6, toute l'appli), corrigé le 2026-09-24 :**
- Le coupe-circuit hérite de `BaseException` et s'appuie sur
  `sys.monitoring` (événements JUMP et PY_START) au lieu de `sys.settrace`.
  Il ne se désactive plus quand le code de l'élève le rattrape : `except:`
  nu, `except Exception`, `except BaseException`, `finally: continue`, ne
  gèlent plus l'onglet (testé dans le vrai Pyodide).
- Une RecursionError arrête le programme dès la première occurrence : une
  récursion rattrapée par un except faisait déborder la pile JavaScript et
  tuait Pyodide.
- Réponses simulées épuisées : arrêt immédiat avec la carte « Ton programme
  pose une question de trop », au lieu de renvoyer "" sans fin.
- `except:` sans nom, `except Exception` et `except BaseException` sont
  refusés avant l'exécution (carte « Précise le type d'erreur »).
- Plus rapide que l'ancien moteur : 0,28 s contre 0,5 s pour 300 000 tours
  de boucle.
- Constaté au passage : l'appli charge Pyodide 0.314 (Python 3.14.2), pas la
  0.26.4 qui sert seulement de repli (`loadFallback`).

**Appliqués (points 1 à 13) :**
- **Schéma `tryflow` :** redessiné (Python ESSAIE → aucune erreur / une ligne
  plante → plan B → la suite continue), plus de « undefined », libellés
  permanents.
- **Cours :**
  - le pourquoi, avec la carte rouge `int("abc")` ;
  - le filet du trapéziste (« attraper ») ;
  - le nom après except = le premier mot du message rouge ;
  - le lien avec le chapitre IX (vérifier avant / rattraper après) ;
  - la boucle qui redemande avec le drapeau, expliquée tour par tour ;
  - `pass` ;
  - le piège du filet trop large, montré avec une NameError cachée, et la
    méthode « provoque l'erreur une fois ».
- **Exercices :**
  - 10-1 : les lignes avant / après l'erreur ;
  - 10-2 : KeyError sur le carnet, `in` et `.get` interdits ;
  - 10-3 : ValueError sur une saisie ;
  - 10-4 : deux filets empilés ;
  - 10-5 : compteur avec `pass` ;
  - 10-6 : remise en ordre de la boucle qui redemande (un seul ordre valide
    sur 40 320) ;
  - nouveau 10-7 : redemander tant que ce n'est pas un nombre entre 0 et 20.

  Tous avec need, useVars et retest.
- **Cartes :**
  - ValueError : `int("")`, `int("2.5")`, `float("abc")`, et un renvoi au
    chapitre X ;
  - ZeroDivisionError et KeyError : renvoi à try/except ;
  - try sans except, except décalé, `except valueerror`,
    `except "ValueError"`, deux-points manquants après try/except ;
  - « ton filet attend X, mais l'erreur est Y » ;
  - nouvelle carte RecursionError.

**Restent :**
- [ ] **14. Annexes :**
  - aide-mémoire : ajouter ValueError, ZeroDivisionError, KeyError dans
    « Erreurs fréquentes », ainsi que `pass` et le motif « redemander » dans
    « Gérer les erreurs » ;
  - glossaire : ajouter try / except (« essayer un bloc ; si une erreur
    précise survient, exécuter un bloc de secours au lieu d'arrêter ») ;
  - renvois possibles : piège de Newton (ZeroDivisionError si f'(x) = 0),
    mini-projet (protéger la saisie), chapitre VIII (« répondre faux est
    plus dangereux que planter »).
- [ ] **Limite connue du moteur, déjà présente avec l'ancien :** une boucle
  qui tourne à l'intérieur d'une fonction toute faite de Python ne passe par
  aucun saut du code de l'élève, donc le coupe-circuit ne peut pas
  l'interrompre et l'onglet gèle. Exemples vérifiés : `sum(range(10**11))`,
  `sum(iter(int, 1))`, `10 ** 10 ** 8`. Le premier est plausible en maths
  (sommer un très grand nombre d'entiers). Même chose, en improbable, pour un
  programme qui coupe lui-même la surveillance
  (`sys.monitoring.set_events(4, 0)`) ou un `__del__` qui boucle. La seule
  vraie garantie : exécuter Python dans un Web Worker, que la page peut
  arrêter au bout de 5 s (changement d'architecture : chargement de
  Pyodide dans le Worker, échanges par messages).
- [ ] Une RecursionError rattrapée volontairement arrête quand même le
  programme (choix délibéré : sinon la récursion rattrapée faisait déborder
  la pile JavaScript et tuait Pyodide).
- [ ] 10-5 : `compteur = 3` écrit dans le try, ou un `if v in [...]` avec un
  try factice, passe encore (liste fixe, pas d'essai supplémentaire
  possible). Jugé acceptable.

Retouches après la relecture de confirmation :
- **Méthode du chapitre :**
  - « le premier mot du message rouge » devient « le mot en …Error écrit
    tout en bas de la carte rouge » ; la carte commence par un titre en
    français, donc son premier mot était « Ce ».
- **Cours :**
  - plusieurs except expliqués, avec un exemple ;
  - `while ok == False` expliqué (le while regarde le drapeau avant
    chaque tour) ;
  - piège du filet trop large montré en code ;
  - `pass` introduit avec `except ValueError:` ;
  - trapéziste « qui ne remonte pas finir son numéro ».
- **Exercice 10-7 :** l'indice explique pourquoi 25 n'est pas une erreur
  pour Python, et un essai supplémentaire avec 0 teste la borne.
- **Cartes :**
  - « ton filet attend X » seulement si la ligne fautive est dans un try ;
    pour une NameError dans un try : « ne l'attrape pas, corrige-la » ;
  - `except A or B` → « or ne marche pas après except » ;
  - carte `true` / `false` → majuscule ;
  - suggestions de noms sans les mots des textes et sans les mots-clés
    (plus de « corrige n en un ») ;
  - carte « nom d'erreur mal écrit » seulement juste après except ;
  - carte « except aligné » : mentionne l'absence de try ;
  - carte « question de trop » : ne parle de try que si le code en
    contient ;
  - carte RecursionError : l'appel accidentel d'abord.
- **Moteur :**
  - nettoyage robuste : les sorties sont rétablies d'abord, et une erreur
    de nettoyage ne remonte plus ;
  - l'heure est lue une fois tous les 64 sauts ;
  - un except en tuple sur deux lignes est détecté ;
  - en cas de TIMEOUT, la sortie montre les 20 dernières lignes.

## Chapitre XI — Le hasard et les modules (relecture du 2026-09-24)

**Au programme** de Première spé : partie « Variables aléatoires »,
rubrique « Expérimentations ». Il faut savoir simuler une variable
aléatoire, écrire une fonction qui renvoie la moyenne d'un échantillon,
mesurer l'écart à l'espérance, et calculer la proportion d'échantillons à
≤ 2σ/√n. Monte-Carlo figure en exemple d'algorithme. Le chapitre n'emploie
pas « loi des grands nombres » (Terminale) ; il rappelle « fluctuation »
(Seconde).

Appliqués (points 1 à 16) :
- **Cours** (28 blocs) :
  - au programme ; pourquoi simuler (le gobelet de dés infatigable) ;
  - caisses à outils au garage (`import`, le point se lit « de la caisse ») ;
  - la caisse math : `sqrt` (float), `pi`, `round` ;
  - `randint` (bornes comprises) et son piège face à `range` ;
  - la graine (un livre de nombres : `seed` dit à quelle page commencer)
    et ses deux pièges ;
  - `random.random()` dans [0 ; 1[ (la goutte d'eau) ;
  - compter avec une tirelire ou avec le tableau d'effectifs du IX ;
  - la fréquence du 6 quand n grandit (10 → 10 000) ;
  - l'espérance 3,5 calculée à la main, puis `moyenne_echantillon` ;
  - la proportion à ≤ 2σ/√n (0,96) ;
  - Monte-Carlo pour π (3,1352).
- **Vérification du hasard** (méthode A + C) : la graine est demandée au
  clavier, et le second essai la change, ce qui refuse les réponses en
  dur. Le programme affiche aussi sa propriété (`abs(f - 0.3) < 0.05`,
  `sum(effectifs.values()) == 1000`…), qui doit valoir True. Les propriétés
  ont été testées sur 300 à 2 000 graines, sans aucun échec. Toutes les
  sorties sont identiques en Python 3.12 et 3.14.
- **Exercices :**
  - 11-1 : `sqrt(25) + 1` ;
  - 11-2 : racine d'un nombre tapé ;
  - 11-3 : aire d'un disque, avec `round` ;
  - 11-7 : un seul ordre valide ;
  - 11-6 : l'import placé trop tard ;
  - nouveau 11-8 : quiz sur les bornes de `randint` ;
  - 11-4 : graine tapée ;
  - 11-5 : fréquence de « pierre » ;
  - nouveaux 11-9 à 11-13 : pièce truquée à 0,3 ; somme de deux dés
    (tableau d'effectifs) ; espérance d'un jeu (−0,5 €) ; proportion
    d'échantillons proches (pièce) ; Monte-Carlo, aire sous la parabole
    (1/3).
- **Cartes :**
  - `math` ou `random` sans import (elle disait « écris-le entre
    guillemets ») ;
  - `sqrt` ou `randint` sans le nom de la caisse ;
  - `import Random` ou `maths`, `math.sqr` (suggestion d'orthographe) ;
  - `math.sqrt(-1)` (messages 3.12 et 3.14) ;
  - `randint(6, 1)`, `randint(1)`, `randint(1, 6.5)` ;
  - `from random import *`.

Restent :
- [ ] **17. Annexes et renvois :**
  - aide-mémoire : ajouter une section « Hasard et calculs » (`import`,
    `randint` bornes comprises, `random()` dans [0 ; 1[,
    `random() < p`, `choice`, `seed`, `math.sqrt`, `math.pi`, `round`) ;
    `memoD` dit encore « huit chapitres » ;
  - glossaire : ajouter Module, Simulation, Graine, Échantillon, Espérance ;
  - `math.exp`, `math.cos` et `math.sin` (au programme de Première) ne sont
    pas montrés ;
  - chapitres XIV et XV : comparer la dichotomie ou Newton à
    `math.sqrt(2)`.
- [x] **18. Chapitre XII, exercice 12-6 (corrigé le 2026-09-24, voir la section XII) :** 11 ordres donnent
  « Trop petit ». Certains placent `random.seed(3)` après le tirage :
  ils passent environ 3 fois sur 4, au hasard. Pistes : afficher
  `secret`, ou fusionner les lignes de tirage. À traiter à la relecture du
  XII.
- [ ] Limite de la méthode A : une solution juste qui tire autrement que
  la consigne (par exemple `int(random.random() * 6) + 1` au lieu de
  `randint`) donne d'autres nombres et est refusée. Les consignes précisent
  l'outil à utiliser (« un random.randint(1, 6) par partie »).
- [ ] `random.seed("0")` (graine laissée en texte, `int()` oublié) ne
  provoque aucune erreur mais donne d'autres tirages : l'élève voit
  seulement « Pas encore ». L'indice de 11-4 le signale ; un diagnostic
  dédié serait possible (code contenant `seed(` sans `int(input`).
- [ ] 11-7 (remise en ordre de 3 lignes) reste très simple ; un ordre plus
  riche (import, graine, compteur, boucle) aurait plusieurs ordres valides.
- [ ] Quiz 11-6 : l'option juste cite `NameError: name 'math' is not
  defined`. Python 3.12+ ajoute « Did you forget to import 'math'? » dans
  le traceback, mais l'appli n'affiche que `str(ex)`, sans cette suite.

Retouches après la relecture de confirmation :
- **Cours :**
  - « 6 lancers → presque jamais un 6 » était faux : c'est (5/6)⁵ ≈ 40 % ;
  - « le programme officiel » au lieu de « le programme », ambigu avec le
    programme Python ;
  - `abs` (valeur absolue), `.values()` et `sorted` sont expliqués ;
  - pourquoi la sortie change sans graine, pourquoi « graine », pourquoi
    la graine est tapée au clavier ;
  - distinction boîte / caisse ; exemple de `choice` ;
  - boucles imbriquées expliquées ; marge 0,05 justifiée ;
  - un bloc « Pause » ;
  - échantillon en deux blocs, avec l'espérance en somme pondérée ;
  - σ justifié (V(X) = 91/6 − 49/4 = 35/12, σ/√n, environ 95 %) ;
  - Monte-Carlo détaillé (aires, uniformité, Pythagore, « deux gouttes ») ;
  - la somme des effectifs est affichée comme propriété (`== 600` → True).
- **Exercices :**
  - l'indice de 11-3 renvoyait à « la puissance du chapitre I »,
    inexistante ;
  - 11-12 refusait une solution juste (`useVars` « seuil ») : retiré, et
    la consigne est découpée en 5 étapes ;
  - `abs` est exigé là où la propriété l'utilise : un `print(True)` écrit
    en dur est refusé ;
  - marges élargies (0,12 pour 11-5, 0,06 pour 11-9 et 11-10) : 0 échec
    sur 2 000 graines ;
  - 11-10 vérifie maintenant la fréquence de 7 (la somme des effectifs
    était toujours vraie).
- **Cartes :**
  - `random()` (« on appelle un outil ») ;
  - `random.random < 0.5` ;
  - `math.sqrt("4")` ;
  - `choice([])` ;
  - `randint(1, n)` avec n resté en texte (3.12 et 3.14) ;
  - variable nommée `random` ;
  - `random.choice(choice)` → suggestion `choix` ;
  - la liste des outils « vus dans le cours » est limitée à ceux du cours.

## Chapitre XII — Mini-projet : le nombre mystère (relecture du 2026-09-24)

**Place au programme :** aucun mini-projet n'est exigé. Mais le chapitre
consolide ce qui l'est (variables, conditions, boucles, fonctions) et
applique la « programmation modulaire qui permet de découper une tâche
complexe en tâches plus simples », sur laquelle le programme officiel met
l'accent.

**Moteur (toute l'appli) :** hasard neuf à chaque exécution
(`_pl_random.seed()` au début de `_pl_run`). Avant, le module `random`
gardait son état d'un essai à l'autre dans Pyodide : après un programme
terminé sur `seed(3)`, un code sans graine tirait toujours 19, et un ordre
faux de 12-6 passait à coup sûr. Une graine plantée par l'élève donne
toujours le même tirage. Aucune régression sur les chapitres XI et XII.

Appliqués (points 1 à 11) :
- **12-6 (point 18) :** le secret est tapé par une amie ; 96 ordres
  forment un programme valide sur 362 880, et un seul donne la bonne
  sortie (3.12 et 3.14). L'ancienne version acceptait 11 ordres, dont 7
  seulement par hasard.
- **Cours :**
  - l'algorithme en langage naturel (flèche ←) remplace le code du jeu,
    qui était la solution de 12-7 ;
  - trois pourquoi : `while` plutôt que `for` ; le premier essai avant la
    boucle (le contrôleur à l'entrée) ; redemander à la fin de chaque tour ;
  - le lien avec le drapeau du chapitre X ;
  - le piège du papier plié : un seul secret pour toute la partie, face au
    piège du XI ;
  - le piège `int()` : « la photo de gâteau », `!=` sans fin ;
  - compter et découper ;
  - la stratégie du milieu : 5 essais au pire pour 20 nombres
    (2⁵ − 1 = 31), 7 pour 100, qui annonce la dichotomie du XIV ;
  - « pour jouer vraiment, supprime la graine ».
- **Exercices :**
  - graine tapée au clavier, essais supplémentaires et mots-clés exigés
    partout : les réponses en dur sont refusées ;
  - 12-3 et 12-4 fusionnés, avec les trois branches testées ;
  - quiz 12-5 : « la graine, deux fois » (options en code, plus de texte
    seulement en français) ;
  - 12-7 testé aussi sur une partie gagnée du premier coup ;
  - nouveaux : 12-8 (compteur d'essais, qui commence à 1), 12-9 (la
    fonction `comparer(essai, secret)` avec `return`), quiz 12-10 (la
    stratégie du milieu : 5 essais) ;
  - « trouvé » accentué partout ; `guess` renommé `essai`.
- **Cartes :**
  - « Tu compares du texte à un nombre » ;
  - « La boîte essai doit exister avant la boucle » (elle conseillait des
    guillemets).

Retouches après la relecture de confirmation :
- **Moteur, défaut bloquant introduit par le hasard neuf :** si l'élève
  écrivait `random.seed = 3`, toutes les exécutions suivantes plantaient
  jusqu'au rechargement de la page. Même défaut, plus ancien :
  `random.randint = 8` ou `math.sqrt = 0` faussaient la suite. Les modules
  `random` et `math` sont maintenant remis à neuf avant chaque exécution
  (photo prise au démarrage), dans un `try`. La sortie est plafonnée à
  200 000 caractères.
- **12-6 déplacé après 12-9 :** placé avant 12-7, il donnait les 9 lignes
  du jeu ; c'est maintenant une vérification finale (« tu as écrit le jeu
  toi-même : retrouve-le ! »).
- **Cours :**
  - dictionnaire de traduction (← → `=`, ≠ → `!=`, « Tant que » →
    `while`…) ;
  - pourquoi 1 + 2 + 4 + … (chaque essai double les nouveaux cas ; suite
    géométrique de raison 2) ;
  - « couvrir » au lieu de « départager » ;
  - « tirelire des chapitres IV et VIII » ;
  - « gros classeur » au lieu de « dictionnaire » (deux livres dans le même
    chapitre).
- **Exercices :**
  - 12-7 explique pourquoi il n'y a plus que deux branches dans la boucle ;
  - l'indice de 12-9 ne donne plus la structure (« garde ta boucle,
    remplace le if/else ») ;
  - 12-10 : les « 2,5 candidats » sont expliqués ;
  - 12-8 : aide à l'autocorrection ;
  - 12-2 exige `int` ;
  - des parties à 2 essais sont ajoutées aux retests de 12-7, 12-8 et 12-9
    (elles refusent `nb = 3` écrit en dur).
- **Cartes :**
  - la carte « boîte avant la boucle » convient aussi au drapeau
    (`ok = False`) ;
  - la carte « texte et nombre » donne un exemple générique ;
  - la carte NOINPUT renvoie à `int()` (« le texte "8" n'est jamais égal au
    nombre 8 »).

Restent :
- [ ] Boucle du jeu mise dans une fonction (`def jeu(): while essai != …`)
  sans premier essai : `UnboundLocalError`, et la carte parle d'une boîte
  « du dehors ». Cas rare.
- [ ] 12-7 : trois `if` imbriqués sans boucle, plus un `while False: pass`
  factice pour satisfaire `need`, passent encore (triche délibérée).

## Chapitre XIII — Suites numériques (relecture du 2026-09-24)

**Au cœur du programme** de Première (« Suites numériques, modèles
discrets » ; exemples d'algorithmes : termes, sommes, seuil, factorielle,
Syracuse, Fibonacci). Le chapitre s'adosse au **cahier de maths**
(`cahier-premiere`, chapitre Suites), dont il reprend :
- les casiers numérotés (rang / terme) ;
- f pour la forme explicite, g pour la récurrence ;
- « le premier est gratuit » (n pas, n + 1 termes) ;
- le tableau d'exécution ;
- le contrôleur qui ne vérifie les billets qu'à l'entrée ;
- les exemples n² − 2n, 5 + … + 47 = 390, 2 + 6 + … + 162 = 242, le loyer
  (500 €, +2 %, 700 € → 17), et le piège u₀ = −3, q = 2.

Appliqués (points 1 à 13) :
- **Définition corrigée :** elle réduisait toute suite à la récurrence ;
  elle donne maintenant les deux formes, explicite u<sub>n</sub> = f(n)
  (`def u(n)`) et par récurrence u<sub>n+1</sub> = g(u<sub>n</sub>) (boucle).
- **Boucle qui écrase :** « regarde à gauche du = », une seule boîte,
  `u = g(u)` (la machine ré-alimentée avec son jus).
- **Nature de la suite :** arithmétique / géométrique lues sur la ligne du
  pas, vérifiées par le terme général ; la virgule française (`* 1.05`)
  et deux cartes (`1,05` → SyntaxError, `1,1` → couple de deux nombres).
- **Liste :** quand et pourquoi ; `[u]` pour que `termes[n]` = u<sub>n</sub> ;
  IndexError ; l'écriture du cahier `L.append(... L[-1])`, acceptée en 13-3.
- **Somme :** tirelire, « glisser d'abord, avancer ensuite », 390 et 242.
- **Seuil :**
  - for / while, condition contraire, tableau d'état ;
  - encadrement u₅ = 63 ≤ 100 < u₆ = 127, contrôleur ;
  - carte dépasse / atteint (S = 512 : 10 contre 9), suite décroissante,
    seuil jamais atteint.
- **Sens de variation :** signe de u<sub>n+1</sub> − u<sub>n</sub>, piège
  u₀ = −3, q = 2, « Python conjecture, les maths démontrent ».
- **Limite intuitive** (0,5u + 1 → 2), **factorielle**, **Fibonacci** ;
  renvois vers les chapitres XII, XIV et XV.
- **Exercices** (11) : n ou S tapé, avec essais supplémentaires (les
  réponses en dur et les raccourcis sont refusés).
  - 13-5 : S = 512 sépare « dépasse » de « atteint » ;
  - 13-7 : le loyer du cahier, S = 500 pour trancher entre les deux ;
  - 13-8 : la voiture, suite décroissante, `while u >= S` ;
  - 13-9 : quiz « que représente le 6 ? » ;
  - 13-10 : factorielle ;
  - 13-11 : sens de variation avec un drapeau ;
  - 13-6 : ordre de la liste, un seul valide sur 720.

Restent :
- [ ] **Syracuse** (exemple d'algorithme du programme) : non traité, car il
  faut `//`, jamais enseigné (`u / 2` donne `3.0`). À faire si l'on
  enseigne un jour la division entière.
- [ ] Le quiz 13-9 demande un encadrement (« quel encadrement justifie le
  6 ? »). Comme le quiz 6-1, il apparaît en écart dans le script de
  vérification, qui compare à la sortie : c'est normal.
- [ ] Raccourcis artificiels qui passent encore, parce que `need` ne
  vérifie que la présence du mot :
  - 13-2 : `for u in [5 - 2 * n]` ;
  - 13-4 : la formule 2ⁿ⁺¹ − 1 avec un `for` vide ;
  - 13-5 : `S.bit_length()` avec un `while False` ;
  - 13-7 : un logarithme avec un `while` qui ne tourne jamais.

  Triche délibérée, risque faible.

Retouches après la relecture de confirmation :
- **Cours :**
  - `L.append(3 * L[-1] - 1)` était présenté comme « la même boucle »
    (autre suite, qui donnait presque 13-3) : c'est devenu
    `L.append(2 * L[-1] + 1)` ;
  - `u = 2 * u + 1` n'est ni arithmétique ni géométrique (« seulement +
    r, ou seulement × q ») ;
  - « le drapeau à l'envers » (« à chaque pas ? » : levé au départ,
    baissé une seule fois), le contrôle des sacs ;
  - f / g : un numéro de porte, ou le contenu du casier précédent ;
  - somme : 47 = u₁₄, et `range(n + 1)` pour n + 1 termes ;
  - la virgule : 05, le mot *tuple*, une erreur qui apparaît plus loin ;
  - les pieds de Fibonacci reliés au code ; la factorielle montrée avec un
    `while` (13-10 demande un `for`) ;
  - une pause ;
  - le cahier `while u < 5000` signalé dans la carte « dépasse / atteint » ;
  - les attributions au cahier corrigées (chapitres Suites **et**
    Algorithmique, « le 2 est effacé », valeurs arrondies du cahier,
    formule générale de la somme) ;
  - « (si n ≥ 1) » dans le résumé.
- **Exercices :**
  - 13-9 : options sous forme d'encadrements (plus d'option défendable,
    plus de texte seulement en français) ;
  - 13-11 : règle qui dépend du rang (u → 0,5u + 10 − n) ; les essais avec
    u₀ = 0 et u₀ = 20 refusent le drapeau inversé, le `else` qui réécrit le
    drapeau, et `> 0` ;
  - noms de variables non imposés quand ils ne sont pas annoncés (`terme`,
    `S`, `annees` et `fact` sont acceptés) ;
  - 13-8 : « à écrire * 0.85 » ;
  - 13-6 (ordre, facile) placé avant 13-3.
- **Carte virgule :**
  - placée avant les cartes « addition / multiplication impossible » ;
  - condition resserrée (plus de faux positif sur `a, b = 0, 1`).
- [ ] Renvois réciproques à ajouter dans les autres chapitres : le cours
  du XV (« c'est une suite récurrente, comme au chapitre XIII ») et le
  résumé du XII (somme géométrique).
- [ ] Aide-mémoire et glossaire : ajouter Suite, Rang, Terme, Raison,
  Seuil, Tirelire qui multiplie.

## Cahier de maths (cahier-premiere) — à corriger côté cahier, pas côté Python

- [ ] **« Dépasse » écrit de deux façons dans le cahier :**
  - `while u <= 700` pour « dépasse 700 » (chapitre Suites, l'exemple du
    loyer) ;
  - `while u < 5000` pour « dépasse 5000 » (chapitre Algorithmique et
    Python, l'exemple du capital).

  « Dépasse » veut dire strictement plus grand : il faut `while u <= S`.
  `while u < S` correspond à « atteint ou dépasse ». Les deux ne donnent la
  même réponse que si aucun terme ne tombe pile sur S. Python-Learn
  (chapitre XIII) enseigne la règle et donne un contre-exemple
  (u<sub>n</sub> = 2<sup>n</sup>, S = 512 : 10 contre 9). À harmoniser dans
  le cahier.
- [ ] Vocabulaire à rapprocher, sans contradiction : le cahier dit
  « meuble à casiers » et « tableau d'exécution », Python-Learn dit
  « classeur » et « tableau d'état ». Le chapitre XIII fait le pont.

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
