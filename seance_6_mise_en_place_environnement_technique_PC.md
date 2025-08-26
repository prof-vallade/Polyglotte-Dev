# ⚙️ Mise en place de l’environnement technique

Cette séance commune explique comment préparer son ordinateur pour travailler avec **Java, JavaScript (Node.js), Kotlin, Python et PHP**.  
L’objectif est de vérifier si chaque langage est déjà installé, puis de l’installer si nécessaire.  

---

## 1. Java

### Vérifier si Java est installé
Dans le terminal :  
```bash
java -version
```

Exemple de réponse attendue :  
```
java version "21.0.2" 2024-01-16
```

### Télécharger et installer Java
- Site officiel : [https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/)  
- Installer le **JDK** (Java Development Kit).  
- Pendant l’installation, accepter les options par défaut.  

---

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
- Kotlin fonctionne avec le **JDK** déjà installé.  
- Outil recommandé : **SDKMAN!** (Linux/macOS) ou IntelliJ IDEA (Windows/macOS/Linux).  
- Télécharger IntelliJ IDEA Community :  
  [https://www.jetbrains.com/idea/download](https://www.jetbrains.com/idea/download)  

---

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
- Site officiel : [https://www.python.org/downloads/](https://www.python.org/downloads/)  
- Pendant l’installation sous Windows, **cocher la case "Add Python to PATH"**.  

sinon :
Si python --version ne marche pas et tu veux qu’il marche :
Ouvre Variables d’environnement
Panneau de configuration → Système → Paramètres système avancés → Variables d’environnement…
Dans Path (compte utilisateur), ajoute :
C:\Users\<TON_USER>\AppData\Local\Programs\Python\Python313\
C:\Users\<TON_USER>\AppData\Local\Programs\Python\Python313\Scripts\
OK, ferme/réouvre le terminal, puis :

python --version
where python

Remplace Python313 si ton dossier s’appelle autrement.
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

## 🎯 Conclusion

À la fin de cette séance, chaque élève doit :  
- Pouvoir exécuter une commande `--version` pour **Java, Node.js, Kotlin, Python et PHP**.  
- Avoir les outils installés et configurés sur son ordinateur.  
- Être prêt à passer à la création et l’exécution de premiers programmes dans chaque langage.  
