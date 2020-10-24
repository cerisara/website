## Plaidoyer pour une éducation sans vidéo

Aujourd'hui, nous associons implicitement "conférence en ligne" ou "cours à distance"
à des solutions d'échanges basées sur des flux vidéo.
Or, la vidéo est sans doute la solution technique la plus mauvaise pour cela,
en particulier pour les cours en ligne.
Ses principaux défauts ?

- C'est la modalité d'échange la plus **polluante**: à l'heure où nous devons drastiquement réduire notre
consommation d'énergie pour donner une chance de survie aux générations futures, et lorsque l'on peut
avantageusement remplacer le gaspillage énergétique des flux video par des solutions beaucoup plus sobre
en électricité et meilleures en terme de fonctionalités, pourquoi se priver ?
- C'est la modalité la plus **liberticide**: comme c'est une modalité extrêmement gourmante en ressources
(quantité de données, de stockage, bande passante, puissance de calcul), seules des grandes entreprises privées
leader sur le marché ont les moyens d'assurer une qualité satisfaisante, car la technologie nécessaire coûte cher.
Ces entreprises, qui font payer ces services à faible prix, font du chiffre d'affaire en monnayant nos données
personnelles, et contribuent ainsi à encore réduire nos libertés individuelles, du moins ce qu'il en reste.
- C'est la solution la plus **inégalitaire**, qui fracture les étudiants en deux groupes séparés:
les privilégiés, majoritaires, qui possèdent une connection fibre chez eux, et les plus pauvres qui ne possèdent
qu'une connection mobile très limitée (par ex. 50MB chez Free) ou payent selon leur consommation.
Quelques Universités offrent parfois des clefs 4G à certains étudiants, mais c'est loin d'être généralisé, et
cela représente un coût important qui sera forcément assumé par quelqu'un à un moment donné, alors que
d'autres solutions, beaucoup moins gourmandes en bande passante, existent et peuvent résorber en grande partie
cette fracture.
- Enfin, la video est une mauvaise solution pour l'éducation, qui n'offre **aucune interactivité**, aucun dynamisme
dans des échanges unidirectionnels, et qui résulte souvent en une piètre qualité, par exemple lorsque l'on filme
un prof écrivant au tableau, ou lorsque la connection lag pour une raison ou une autre.

Or, il existe d'autres solutions à tous ces problèmes, mais ils ne sont que peu utilisés,
principalement pour des raisons d'habitude, de méconnaissance, et de confort car elles recquièrent effectivement
un effort pour changer de façon de rédiger ses supports de cours.
La base de ces solutions consiste en effet à rédiger ses supports non plus avec powerpoint, mais dans un simple
format textuel, qui est d'ailleurs le même que celui utilisé dans les Wiki; il est d'ailleurs très simple et
permet de créer des transparents beaucoup plus rapidement qu'avec powerpoint, mais en offrant moins de possibilités
visuelles. Les slides résultant sont tout aussi beaux, mais plus simples, plus épurés, avec un focus sur le contenu
plutôt que la forme. Il est possible par ailleurs d'ajouter des effets visuels assez bluffant, car inhabituels et
très différents de ceux auxquels nous avons l'habitude avec les suites office. Mais ces effets sont encore assez
complexes à mettre en oeuvre (ce sont en fait toutes les animations javascript).
Les slides résultant sont alors de simples pages web, que tous les étudiants peuvent consulter dans tout
navigateur, même sur leur smartphone.

Mais cela va bien au-delà, car il est possible, et même très facile, d'inclure de très nombreuses fonctionalités
qui peuvent rendre ce format de diffusion très riche en fonction des situations. Par exemple:

- La qualité des transparents est parfaite quelle que soit la connection internet, car il ne s'agit en fait que
d'une page web améliorée, directement stockée en local sur le terminal de l'étudiant;
- Pendant un cours, tous les slides des étudiants peuvent être synchronisés avec un browser "maître": ainsi, les
étudiants peuvent revenir en arrière sur leur écran, mais dès que le "maître" avance à un endroit de la présentation,
tous les clients s'y rendent automatiquement. En terme de qualité sur le terminal, et d'interactivité avec le
support de cours, cette méthode permet déjà un gain énorme par rapport à une retransmission vidéo ou un partage d'écran.
- Pendant un cours, le prof peut dessiner, avec sa souris ou mieux un stylet, sur les slides, et ses dessins seront
immédiatement retransmis sur les slides des étudiants.
- De même, des animations, des courbes qui se dessinent, peuvent être contrôlées par le "maître" et être reproduites
sur les "clients".
- S'il y a besoin de montrer un terminal, par exemple lors d'un cours de programmation, il est possible d'inclure
dans les slides clients un "pseudo-terminal" qui retransmettra en direct le terminal du prof.
- Il suffit d'appuyer sur une touche pour enregistrer un commentaire audio par slide, et ainsi faire du cours
un MOOC consultable à tout moment.

Et de nombreux autres plugins ne cessent d'être développés et enrichissent de mille façon possible cette nouvelle
manière de concevoir les cours.
Pour plus d'infos techniques, allez voir reveal.js et ses nombreux plugins, notamment multiplex, chalkboard, audioslides, etc.

Il faudrait simplifier l'utilisation de ces méthodes afin de les démocratiser au-delà de la sphère des informaticiens,
et je réfléchis pour cela à étendre la plateforme du fediverse OLKi afin qu'elle permette à des enseignants
de tester ces méthodes avec zéro code, sans serveurs et zéro installation.
Si vous êtes intéressés, merci de me contacter !

