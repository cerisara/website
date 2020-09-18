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

