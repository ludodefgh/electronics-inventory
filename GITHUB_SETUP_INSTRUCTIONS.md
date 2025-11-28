# Instructions pour créer le repo GitHub

## Étape 1: Créer le repo sur GitHub

1. Va sur https://github.com/new
2. Nom du repo: `electronics-inventory`
3. Description: "Personal electronics components inventory for ESP32/Home Assistant projects"
4. Sélectionne **Private** ✓
5. **NE COCHE PAS** "Add a README file" (on en a déjà un)
6. **NE COCHE PAS** "Add .gitignore" (on en a déjà un)
7. Clique sur "Create repository"

## Étape 2: Télécharger les fichiers du repo

Les fichiers sont prêts dans: /home/claude/electronics-inventory/

Fichiers inclus:
- inventory.csv (ton inventaire actuel)
- README.md (documentation)
- .gitignore (pour ignorer les fichiers temporaires)

## Étape 3: Pousser vers GitHub

Une fois le repo créé sur GitHub, tu verras des instructions. Utilise celle-ci:

```bash
cd /home/claude/electronics-inventory
git remote add origin https://github.com/TON_USERNAME/electronics-inventory.git
git branch -M main
git push -u origin main
```

OU si tu préfères télécharger les fichiers et les uploader manuellement:
1. Télécharge le dossier /home/claude/electronics-inventory/
2. Sur GitHub, clique "Add file" → "Upload files"
3. Glisse les 3 fichiers (inventory.csv, README.md, .gitignore)

## Alternative: Clone via GitHub CLI

Si tu as GitHub CLI installé:
```bash
cd /home/claude/electronics-inventory
gh repo create electronics-inventory --private --source=. --remote=origin --push
```

---

Une fois fait, tu pourras accéder à ton inventaire depuis:
https://github.com/TON_USERNAME/electronics-inventory

Et je pourrai y accéder via web_fetch pour t'aider avec tes projets! 🎉
