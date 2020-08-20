## Site personnel

Ce site est en construction permanente.
L'objectif de ce site est de diffuser des blogs (plutôt sérieux), des tutos, du code, etc.

Pour le moment, vous pouvez:

- **Nouveau**: Un [premier cours en ligne sur le deep learning](https://olki.loria.fr/mooc/mooc1) en français, 100% gratuit et sans traqueurs  !
- lire un [premier blog (en anglais) sur le deep learning](https://blog.cerisara.fr).
- me contacter sur Mastodon: @cerisara@mastodon.etalab.gouv.fr
- voir [mon CV](https://members.loria.fr/CCerisara/resume)

Mon objectif: un deep learning éthique et accessible...

Mes différentes identités numériques:

- [sur github](https://github.com/cerisara); mais je suis aussi sur gitlab.com, bitbucket, framagit, et gitlab.inria.fr
- [sur stackoverflow](https://stackoverflow.com/users/2637126/xtof54)
- [sur iNaturalist](https://www.inaturalist.org/people/christophecerisara)
- [sur Mastodon](https://mastodon.etalab.gouv.fr/@cerisara)
- [sur Google scholar](https://scholar.google.com/citations?user=dB1-aHwAAAAJ&hl=fr&oi=ao)
- et de nombreuses autres...

-------------

## Tuto: accéder à des livres numériques sous Ubuntu 20

De plus en plus de bibliothèques proposent de télécharger et de lire des livres numériques
sur liseuse, et utilisent le logiciel Adobe Digital Editions (ADE) pour gérer les emprunts et les DRM des livres.
Quand on est sous linux, ce n'est malheureusement pas si simple.
Voici un petit tuto qui vous permet de récupérer les livres sous Ubuntu 20, et de les lire sur une Kindle,
en enlevant (temporairement, juste le temps de l'emprunt !) le DRM.

- installez la version 4.22 de Calibre sous Ubuntu (qui fonctionne avec python 2.7 !) comme ceci:

```
sudo -v && wget -nv -O- https://download.calibre-ebook.com/linux-installer.sh | sudo sh /dev/stdin
```

- Installez ensuite dans calibre la derniere version du plugin DeDRM
- En partant d'une installe de Ubuntu 20 "propre", installez wine en le configurant pour du win32, puis ADE:

```
sudo apt install wine
export WINEARCH="win32"
export WINEPREFIX=~/.wineadobe
wineboot -u
winetricks dotnet40
wine ADE_4.5_Installer.exe 
```

- Il faut enfin faire la connection entre calibre/DeDRM (qui tourne sous linux) et ADE (qui tourne sous Wine) en installant
python 2.7 sous Wine (à télécharger ici: http://www.voidspace.org.uk/python/modules.shtml#pycrypto et https://www.python.org/download/releases/2.7/)

```
msiexec /i ~/Downloads/python-2.7.18.msi
wine ~/Downloads/pycrypto-2.6.win32-py2.7.exe
```

- puis en configurant le plugin DeDRM en lui indiquant simplement le WINEPREFIX = ~/.wineadobe
- Lors de l'import d'un livre, le plugin peut ne toujours pas fonctionner, car il cherche python.exe dans C:windows/system32 alors que l'install précédente l'a mise dans C:Python2.7 . Dans ce cas, copier/coller l'executable python.exe au bon endroit.

