Les maths sont calculés par mes soins et je dois admettre que Black Desert ne communique pas spécialement les formulations mathématiques, donc l'application est sujet à erreurs/changement si les développeurs changent la façon de causer des dommages IG.
Je voudrai tout de même notifier que sur une logique purement mathématiques, le but ici est de comprendre le "POURCENTAGE" affiché de votre compétence.

Sur la plus part des MMORPG vous voyez directement vos flats en points et non en pourcentages comme sur BDO ou encore SoulWorker.

Ici le but recherché a été de trouver la formulation mathématiques pour convertir ces pourcentages en points afin d'afficher la valeur de ces dits "pourcentages".

Logiquement sur une logique brute, vous aurez donc purement votre flat value.


Formulation mathématiques:
   Dégâts Totaux = ((AP de base * %Comp / 100 * Attaques multiples) + (Multiplicateur secondaire * AP de base * Nombre Max Y hits)) * Buff\n
   Dégâts Finaux = (Dégâts Totaux - DP Mob) / Réduction


Par la suite nous prendrons le résultat de cette formule pour venir soustraire d'abord la valeur en points réductions puis, je divise celà par 1.3 par exemple pour 30% de réductions et vous obtenez la valeur brute de votre sort.

Détail:

Etape 1:
Skill% / 100

Etape 2:
AP TOTAL * (Skill% /100)

Etape 3:
Si ton sort est un sort à Tiks, le résultat d'avant est multiplié par le nombre de tiks.
Résultat de AP TOTAL * (Skill% /100) * xN DMG (Nombre de Tiks)

Etape 4:

Si ton tiks peut générer d'autres tiks il sont alors inclu mais pas multipliés

Donc le calculateur reprends ton dégâts de base;

AP TOTAL * (Skill% /100)
et il le multiplie par le Y Max Hit (Les tiks que vont générer les autres Tiks)

Donc:
Résultat de AP TOTAL * (Skill% /100) * Max Y Hit (Tiks supplémentaires)

Etape 5:

Le calculateur additionne la value du Max Y Hit à la valeur final de ton dégât de base * ton xN DMG
Il ne la MULTIPLIE DONC PAS, sinon ce serait bien entendu trop fort si les tiks se multipliaient par eux mêmes :P

Etape 6:
Si tu as un buff multiplicateur par exemple un 1,5x DMG, le calculateur se charge de faire le total de tout ce que j'ai énoncé avant * ton multiplicateur.

Tu peux te servir de celà pour n'importe quel multiplicateur à condition de comprendre le multiplicateur que tu veux user.
Globalement, si c'est du backstab tu peux ajouter 1,5x par exemple !

Ensuite sur BDO tu as une valeur de réduction de base en point par rapport aux DP, donc on les soustrais simplement au résultat final, puis viennent les multiplicateur en pourcentages de réductions qui peuvent aller de 1% à 30%.

Donc là, le multiplicateur divise par exemple par 1.3 pour (30% de réductions) le chiffre total pour te donner la réelle valeur BRUTE de ton sort !

Ninee9, un joueur qui tâche de conserver son amour des MMORPG.
