# Formation GitHub 3
## Utilisation de GitHub avec Git (méthode clonage)

### Objectifs
- Cloner un dépôt GitHub sur sa machine locale.
- Travailler en local et synchroniser avec GitHub.

### Étapes
1. Copier l’URL du dépôt (`HTTPS` ou `SSH`).
2. Dans le terminal :
   ```bash
   git clone https://github.com/utilisateur/nom-depot.git
   ```
3. Se déplacer dans le projet cloné :
   ```bash
   cd nom-depot
   ```
4. Ajouter un fichier, puis valider les changements :
   ```bash
   git add fichier.txt
   git commit -m "Ajout du fichier"
   ```
5. Envoyer les changements vers GitHub :
   ```bash
   git push origin main
   ```

### Résultat attendu
- Un dépôt cloné en local.
- Synchronisation correcte entre GitHub et la machine.
