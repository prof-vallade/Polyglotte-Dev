# Formation GitHub 4
## Utilisation de GitHub avec Git (méthode remote)

### Objectifs
- Créer un dépôt en local et le lier à GitHub.
- Pousser un projet existant vers GitHub.

### Étapes
1. Créer un dépôt Git en local :
   ```bash
   git init
   ```
2. Ajouter des fichiers :
   ```bash
   git add .
   git commit -m "Initial commit"
   ```
3. Créer un dépôt vide sur GitHub.
4. Lier le dépôt local au dépôt GitHub :
   ```bash
   git remote add origin https://github.com/utilisateur/nom-depot.git
   ```
5. Envoyer le projet :
   ```bash
   git push -u origin main
   ```

### Résultat attendu
- Un dépôt local existant est désormais hébergé sur GitHub.
- Le dépôt est synchronisé.
