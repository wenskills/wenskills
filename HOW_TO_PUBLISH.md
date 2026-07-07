# Publier le README WenSkills sur GitHub

## 1. Vérifier ton username GitHub

Le README de profil ne fonctionne que si le repo porte exactement le même nom que ton compte.

Exemples :

- username GitHub : `wenskills` → repo à créer : `wenskills`
- username GitHub : `wendyrasam` → repo à créer : `wendyrasam`

L’URL finale doit ressembler à :

```txt
https://github.com/TON_USERNAME/TON_USERNAME
```

## 2. Créer le repo spécial sur GitHub

1. Va sur GitHub.
2. Clique sur **New repository**.
3. Dans **Repository name**, mets exactement ton username.
4. Mets le repo en **Public**.
5. Ne coche rien si tu veux pousser ce dossier directement depuis le terminal.
6. Clique sur **Create repository**.

## 3. Pousser ce dossier depuis le terminal

Place-toi dans le dossier extrait :

```bash
cd wenskills-profile
```

Puis lance :

```bash
git init
git add .
git commit -m "Create WenSkills profile README"
git branch -M main
git remote add origin https://github.com/TON_USERNAME/TON_USERNAME.git
git push -u origin main
```

Remplace bien `TON_USERNAME` par ton vrai username GitHub.

Exemple si ton username est `wenskills` :

```bash
git remote add origin https://github.com/wenskills/wenskills.git
git push -u origin main
```

## 4. Si tu as déjà créé le repo avec un README vide

Utilise plutôt cette méthode :

```bash
git clone https://github.com/TON_USERNAME/TON_USERNAME.git
cp -r wenskills-profile/* TON_USERNAME/
cd TON_USERNAME
git add .
git commit -m "Update profile README"
git push
```

## 5. Modifier les liens à compléter

Dans `README.md`, remplace :

- `portfolio-à compléter`
- `linkedin-à compléter`
- `email-à compléter`

Tu peux aussi remplacer les images de projets dans `assets/` par de vraies captures plus tard, en gardant les mêmes noms :

```txt
clutchr-cover.png
atlas-cover.png
baileo-cover.png
sidequest-cover.png
```

## 6. Bio GitHub à mettre

Dans ton profil GitHub > Edit profile > Bio :

```txt
Développeuse full-stack orientée produit — interfaces soignées, backends solides, IA utile & webdesign qui a du goût.
```

Version plus courte :

```txt
Full-stack developer · produit, webdesign, architecture & IA utile.
```

## 7. Repos à épingler

Ordre conseillé :

1. Clutchr
2. ATlaS
3. Baileo
4. SideQuest
5. Catalogue de formations / migration Symfony, seulement si montrable
6. Alerte AMU, seulement si montrable sans souci de confidentialité
