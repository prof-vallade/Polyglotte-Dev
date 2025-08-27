# 👋 Afficher « Bonjour c'est &lt;Langage&gt; » et exécuter dans VS Code (5 langages)

Ce mémo montre **le code minimal** et **comment l’exécuter dans VS Code** pour : Java, JavaScript (Node.js), Kotlin, Python et PHP.  
Deux méthodes d’exécution sont proposées : **Terminal** et **Code Runner** (optionnel).

> 💡 Prérequis rapides :  
> - **Java** : JDK installé (`java -version`, `javac -version`)  
> - **JavaScript** : Node.js installé (`node -v`)  
> - **Kotlin** : soit IntelliJ IDEA, soit le compilateur CLI `kotlinc` ajouté au PATH  
> - **Python** : `python --version` (ou `py --version`)  
> - **PHP** : `php -v` (PHP CLI, via installation seule ou via Laragon et PATH configuré)

---

## 1) Java

### Code — `Bonjour.java`
```java
public class Bonjour {
    public static void main(String[] args) {
        System.out.println("Bonjour c'est Java");
    }
}
```

### Exécuter dans le **Terminal VS Code**
```bash
javac Bonjour.java
java Bonjour
```

### (Optionnel) Exécuter avec **Code Runner**
- Clic droit → **Run Code**  
- Ou `Ctrl+Alt+N`  
> ⚠️ Pour des projets Java multi-fichiers, préférez IntelliJ IDEA.

---

## 2) JavaScript (Node.js)

### Code — `bonjour.js`
```javascript
console.log("Bonjour c'est JavaScript");
```

### Exécuter dans le **Terminal VS Code**
```bash
node bonjour.js
```

### (Optionnel) **Code Runner**
- Clic droit → **Run Code** (ou `Ctrl+Alt+N`).

---

## 3) Kotlin

### Option A — **IntelliJ IDEA** (recommandé pour débuter)
- Nouveau projet **Kotlin/JVM** → crée `Main.kt` avec :  
```kotlin
fun main() {
    println("Bonjour c'est Kotlin")
}
```
- Clique sur **▶ Run**.

### Option B — **Terminal VS Code** avec le compilateur CLI
> Nécessite `kotlinc` dans le PATH (`kotlinc -version`).

#### Code — `Bonjour.kt`
```kotlin
fun main() {
    println("Bonjour c'est Kotlin")
}
```

#### Compiler & exécuter
```bash
kotlinc Bonjour.kt -include-runtime -d Bonjour.jar
java -jar Bonjour.jar
```

#### (Optionnel) **Code Runner**
- Clic droit → **Run Code** (si `kotlinc` est installé et détecté).

---

## 4) Python

### Code — `bonjour.py`
```python
print("Bonjour c'est Python")
```

### Exécuter dans le **Terminal VS Code**
```bash
python bonjour.py
# ou sur certains systèmes :
py bonjour.py
```

### (Optionnel) **Code Runner**
- Clic droit → **Run Code** (ou `Ctrl+Alt+N`).

---

## 5) PHP

### Code — `bonjour.php`
```php
<?php
echo "Bonjour c'est PHP";
?>
```

### Exécuter dans le **Terminal VS Code**
```bash
php bonjour.php
```

### (Optionnel) **Code Runner**
- Clic droit → **Run Code** (ou `Ctrl+Alt+N`).

---

## ⚙️ Astuces VS Code

- **Sélectionner l’interpréteur Python** : `Ctrl+Shift+P` → *Python: Select Interpreter* → choisir la bonne version.  
- **Activer le bouton Stop de Code Runner** : dans `settings.json`  
```json
{
  "code-runner.runInTerminal": true,
  "code-runner.showStopIconInEditor": true
}
```

- **Forcer l’exécution de Code Runner dans un nouveau terminal** (pour éviter de “bloquer” le terminal) :  
  Paramètres → `Code Runner: Run In New Terminal` → ✅

---

## ✅ Récapitulatif des commandes (Terminal)

| Langage     | Commande d’exécution                                       |
|-------------|-------------------------------------------------------------|
| **Java**    | `javac Bonjour.java && java Bonjour`                        |
| **JS**      | `node bonjour.js`                                          |
| **Kotlin**  | `kotlinc Bonjour.kt -include-runtime -d Bonjour.jar` puis `java -jar Bonjour.jar` |
| **Python**  | `python bonjour.py` (ou `py bonjour.py`)                    |
| **PHP**     | `php bonjour.php`                                          |

Bon code à tous 👩‍💻👨‍💻 !
