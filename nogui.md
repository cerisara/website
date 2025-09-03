Misc terminal tools:

- curl -s "https://aleyan.com/projects/ascii-side-of-the-moon?date=2025-09-03"
- curl https://wttr.in/nancy
- charm.sh
- mutt + offlineimap + notmuch
- khalendar + vdirsyncer
- vim + git
- password-store + gpg2
- lynx

### 100% terminal

La souris, c'est l'enfer pour les vrais geeks: il faut déplacer le bras pour la chercher,
déplacer la main tout en visant avec l'oeil un petit coin de l'écran, et cliquer...
Quelle perte de temps, alors que tout peut être fait en général en tapant sur 2 touches du
clavier, sans bouger les mains, en les laissant tout le temps à la bonne position.
Après tout, on a un cerveau qui nous a permis d'apprendre une voire plusieurs langues d'une
complexité extrême, alors est-ce si difficile de retenir quelques combinaisons de touche qui
nous permettent de perdre dix fois moins de temps ?

Bref, l'idéal du geek est de tout faire au clavier, très vite, dans un terminal.
Alors c'est vrai que les outils suivants ont vraiment un look très "old-school", tout noir et vert,
mais s'ils ont survécu aussi longtemps et sont toujours utilisés, c'est pour une bonne raison !

- **emails** : **mutt** est très très bien, on gère ses emails très rapidement dans le terminal,
  et lorsqu'un email arrive en HTML (quelle idée ! mais bon, y'en a qui trouvent ça "joli"...),
  il est facile de configurer une touche pour l'ouvrir illico dans un firefox. Et pour faire des
  recherches plus rapidement dans nos dizaines de milliers de mails passés, rien de mieux que
  **offlineimap**: j'ai longtemps utilisé mutt en connection directe avec Zimbra,
  mais Zimbra envoie parfois des headers erronés; je suis donc passé à offlineimap + mutt, ca marche bien avec Zimbra.
  Par contre, offlineimap/mutt marchent très mal avec GMAIL: j'utilise donc pour GMAIL spécifiquement
  [lieer+notmuch](https://lieer.gaute.vetsj.com) qui est conçu spécifiquement pour GMAIL: il marche très bien.
- **éditeur**: OK, y'a pas photo: **VIM**, what else ? Ah j'entends quelque chose au fond, quoi ? "Et Max" ?
  hummm... connais pas !
- **gestionnaire de mots de passe**: bon celui-là est très très geek, et pas facile à installer, mais tout
  dans le terminal, ultra-rapide, private-secure, synchronisé dans git,
  dispo sous android et linux: **pass** (password-store) combiné avec **gpg** et bien sûr **git** pour centraliser les
  fichiers de mot de passe.
- **gestionnaire d'articles**: pour ceux qui lisent beaucoup d'articles en PDF sur le web (il serait grand temps
  d'éliminer le PDF pour le remplacer par du markdown+epub, mais bon, c'est un autre débat): **papis**
  est très bien, tout terminal, rapide, synchro avec **git**.
- **spreadsheet**: SVP, arrêtez ces usines à gaz excel, libreoffice et la clique ! Utilisez **sc-im** dans
  le terminal, c'est mille fois plus rapide; bien sûr, il n'y a pas toutes les fonctionnalités "avancées" que
  l'on peut trouver dans les autres, mais on en a très rarement besoin; bien sûr, il faut apprendre de nouveaux
  raccourcis claviers, mais une fois qu'on connaît **VIM**, ca y ressemble beaucoup, et c'est synchro avec **git**
  bien sûr.
- **office**: Tant qu'on est dans ces suites, pour les présentations, **Reveal.js** est génial, bourré de
  fonctionnalités réseaux (synchro des slides en HTML, annotations diffusées, etc.); Et pour les docs, utilisez
  **Markdown** pour publier sur le web et écrire rapidement, et **Latex** lorsqu'on veut fignoler l'édition;
  le tout compilé avec **pandoc** qui passe d'un format à l'autre sans soucis.
- **navigateur internet**: **lynx** pour aller vite, mais c'est vrai que il y a beaucoup de pages qui ne passent
  plus bien dans lynx; dans ce cas, il faut faire un compromis et utiliser une interface graphique, mais contrôlée
  au clavier: **qutebrowser**.
- **agenda**: J'ai utilisé **calcurse** pendant plusieurs années, mais n'étant pas compatible avec calDAV, il ne
  permet pas de voir les agenda sur android. Je suis donc passé (fin 2024) à **khal** et **vdirsyncer** pour mes PC linux,
  et **ETAR** et **DAVx5** sur android (tout est sur FDroid et Google-free). Bien sur, il faut avoir un site de confiance
  pour hoster le serveur calDAV, ou le self-hoster soi-meme. Mon agenda pro est hébergé sur Zimbra, et mon agenda perso
  est sur **framagenda**. 
- **réseaux sociaux**: fuyez les grands réseaux sociaux; les geeks sont encore sur **Usenet** (eh oui, ca ne sert pas que
  à pirater, on peut aussi y discuter !), à lire avec **slrn** par exemple. Ou alors, il y a **Mastodon**, mais pas très adapté au terminal; sinon, le vénérable IRC, ou pas de réseaux sociaux du tout, c'est encore mieux.

J'en ai sûrement oublié, mais l'anneau pour les lier tous, c'est bien sûr **git** !

