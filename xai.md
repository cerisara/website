### Les arbres de décision ne sont pas explicables

Imaginez la tâche suivante: on veut savoir si un bâteau flottera ou coulera.
On entraîne un classifieur, par exemple un arbre de décision, en lui donnant en entrée
la masse et le volume du bâteau. Supposons aussi que la véritable grandeur physique
qui permette de décider si un bâteau coule ou pas est la masse volumique (ce n'est pas
vrai bien sûr, mais supposons que ce soit le cas). Dans ce cas, l'arbre de décision
entraîné sera très profond, car il découpera l'espace de recherche selon 2 axes qui ne
correspondent pas à la vértiable grandeur physique discriminante:

- Si la masse > 10T et le volume < 10m3, alors il coule
- Si la masse > 12T et le volume < 12m3, alors il coule
- Si la masse > 14T et le volume < 14m3, alors il coule
- etc.

Ce résultat ne nous permet pas d'interpréter correctement le classifieur: en terme
d'explicabilité, nous voudrions comprendre que c'est la masse volumique qui importe !

Par contre, si nous remplaçons l'arbre de décision par un réseau de neurones,
la dernière couche du réseau calculera effectivement la masse volumique. Donc, en ce sens,
le réseau de neurones est plus explicable que l'arbre de décision.
Par contre, il ne nous dira pas explicitement, en langage naturel, qu'il calcule la masse volumique,
et pour être totalement explicable, il faudrait construire une technique qui découvre que
la valeur calculée sur la dernière couche est une grandeur connue, et qu'il s'agit de la masse volumique.
La notion d'interprétation revient alors à associer les théories et connaissance que nous connaissons
avec cette fameuse "dernière couche" du réseau. Une telle interprétation est ainsi limitée par nos connaissances.

Une autre remarque importante en lien avec cet exemple est que l'approche classique d'explicabilité
des réseaux de neurones qui étudie l'importance des observations en entrée, par exemple via les
*integrated gradients*, n'est pas pertinente ici, et je pense qu'il vaut mieux s'intéresser aux dernières
couches du réseau, celles qui calculent les informations de haut niveau.

