# ⚙️ Mise en place de l’environnement technique

Cette séance commune explique comment préparer son ordinateur pour travailler avec **Java, JavaScript (Node.js), Kotlin, Python et PHP**.  
L’objectif est de vérifier si chaque langage est déjà installé, puis de l’installer si nécessaire.  

---

## 1. Java

### Vérifier si Java est installé
Dans le terminal :  
```bash
java -version  
javac -version
```

Exemple de réponse attendue :  
```
java version "21.0.2" 2024-01-16  
javac 21.0.8
```

### Télécharger et installer Java
- Site officiel : [https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/)  
- Installer le **JDK** (Java Development Kit).  
- Pendant l’installation, accepter les options par défaut.  

---
### Extention vscode recommandée
pack Extension Pack for Java (éditeur : Microsoft)

---
### Vérifier l’interpréteur java :  
Tu as déjà installé le JDK 21, VS Code détecte automatiquement javac et java via le PATH (vérifier par les tets version dans le terminal) :

## 2. JavaScript (Node.js)

### Vérifier si Node.js est installé
```bash
node -v
```

Exemple attendu :  
```
v20.11.0
```

### Télécharger et installer Node.js
- Site officiel : [https://nodejs.org/](https://nodejs.org/)  
- Télécharger la version **LTS (Long Term Support)**.  
- Installer en suivant les options par défaut.  

### Extention vscode recommandée : Code Runner (de Jun Han)
Il est installé par défaut dans les dernière version vscode. C'est un bouton "play" qui permet exécuter directement le code sans passer par la phase de saisie de la commande d'exécution.  

---

## 3. Kotlin

### Vérifier si Kotlin est installé
```bash
kotlin -version
```

Exemple attendu :  
```
Kotlin version 1.9.22
```

### Télécharger et installer Kotlin
#### méthode 1 (pour les étudiants plus avancés) : l'IDE IntelliJ IDEA
- Kotlin fonctionne avec le **JDK** déjà installé.  
- Outil recommandé : **SDKMAN!** (Linux/macOS) ou IntelliJ IDEA (Windows/macOS/Linux).  
- Télécharger IntelliJ IDEA Community :  
  [https://www.jetbrains.com/idea/download](https://www.jetbrains.com/idea/download)  

---
Dans les options d'installatation, cocher :  
✔️ Create Desktop Shortcut → oui  
✔️ Add "bin" folder to the PATH → oui  
✔️ Add "Open Folder as Project" → optionnel  
✔️ Associations → .java, .kt, .kts

#### méthode 2  pour utiliser kotlin dans vscode (débutant) 

1 - Télécharge Kotlin Compiler (ZIP) ici :
👉 https://github.com/JetBrains/kotlin/releases

(fichier : kotlin-compiler-1.x.x.zip)

2 - Dézippe dans C:\kotlin par exemple

3 - Ajoute au PATH Windows :

C:\kotlin\bin

4- Faire le test dans vscode  
kotlin -version  
ou  
kotlinc -version

2 - Installer les extensions VS Code

- Kotlin (fwcd)

- Code Runner (optionnel) → exécuter facilement des snippets

#### Résumé

JavaScript en navigateur se fait avec des balise <script> dans un fichier HTML.

JavaScript dans VS Code se fait via Node.js et s'exécute avec la commande "node fichier.js"

Avec l'extension Code Runner (pour tous les langages) l'exécution  se fait en 1 clic : on clique droit dans le fichier ouvert et on sélectionne "Run Code"

## 4. Python

### Vérifier si Python est installé
```bash
python --version
```
ou sur certains systèmes :  
```bash
python3 --version
```

Exemple attendu :  
```
Python 3.12.2
```

### Télécharger et installer Python

#### 1 - Installer 
- Site officiel : [https://www.python.org/downloads/](https://www.python.org/downloads/)  
- Pendant l’installation sous Windows, **cocher la case "Add Python to PATH"**.  

sinon :  
Si python --version ne marche pas et tu veux qu’il marche :  
ajoute dans le path :  C:\Users\<TON_USER>\AppData\Local\Programs\Python\Python313\

C:\Users\<TON_USER>\AppData\Local\Programs\Python\Python313\Scripts\  
Ce dossier contient les utilitaires installés avec pip et autres packages.
Exemples :  
pip.exe (gestionnaire de paquets Python)  
jupyter.exe (si tu installes Jupyter)  
flask.exe, django-admin.exe, etc.

Donc, si tu veux utiliser pip install et lancer directement les programmes qu’il installe, ce dossier "Scripts" doit aussi être dans le PATH.

OK, ferme/réouvre le terminal, puis on test:

python --version

where python

Remplace Python313 si ton dossier s’appelle autrement.  
Contient les utilitaires installés avec pip et autres packages.
Exemples :

pip.exe (gestionnaire de paquets Python)

jupyter.exe (si tu installes Jupyter)

flask.exe, django-admin.exe, etc.

#### 2 - Installer l’extension "Python" dans le VS Code

Ouvre VS Code

Va dans l’onglet Extensions (icône carrée à gauche ou Ctrl+Shift+X)

Cherche Python (éditeur : Microsoft)

Clique sur Installer

Cette extension te permet d’exécuter ton code Python directement dans VS Code.

#### 2 - Sélectionner l’interpréteur Python

Ctrl+Shift+P → tape Python: Select Interpreter

Choisis le path de ton installation Python

Si tu as plusieurs Python (par ex. Anaconda + Python officiel), c'est là qu'il faut choisir celui que tu veux utiliser

---

## 5. PHP

### Vérifier si PHP est installé
```bash
php -v
```

Exemple attendu :  
```
PHP 8.3.4 (cli) (built: Mar 5 2024)
```

### Télécharger et installer PHP
- Site officiel : [https://www.php.net/downloads](https://www.php.net/downloads)  
- Sous Windows, il est conseillé d’installer **XAMPP** (qui inclut PHP, Apache, MariaDB) :  
  [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html)  

Si on a déjà Laragon installé sur la machine, PHP est déjà installé. Ce n'est pas la peinne de l'installer une deuxième fois.
- Soit on fait les tets dans Laragon (c'est plus compliqué à notre stade), 
- soit on fait les tets dans vscode (c'est plus pratique), à ce moment-là on utilise le php de Laragon en ajoutant dans le PATH le dossier correspondant : C:\laragon\bin\php\php-8.x.x-Win32-vs16-x64 (remplace 8.x.x par ta version exacte que tu peux voir dans C:\laragon\bin\php\).
---

### extension vscode recommandée  
PHP Intelephense (éditeur : Ben Mewburn)  
👉 Fournit : autocomplétion, erreurs, analyse du code.

### Vérifier l’interpréteur PHP  
si c'est Laragon alors vérifie le PATH (ex. C:\laragon\bin\php\php-8.2.x-Win32-vs16-x64)

## 🎯 Conclusion

À la fin de cette séance, chaque élève doit :  
- Pouvoir exécuter une commande `--version` pour **Java, Node.js, Kotlin, Python et PHP**.  
- Avoir les outils installés et configurés sur son ordinateur.  
- Être prêt à passer à la création et l’exécution de premiers programmes dans chaque langage.  
