# 🚀 Guide de déploiement sur Vercel - ParcoursParis

Ce guide t'explique comment mettre **ParcoursParis** en ligne gratuitement sur Vercel en moins de 5 minutes.

---

## Option 1 : La plus simple (recommandée pour la présentation)

### Méthode Drag & Drop (sans Git)

1. Va sur : [https://vercel.com](https://vercel.com)
2. Connecte-toi avec ton compte **GitHub** (ou crée un compte gratuitement)
3. Une fois connecté, clique sur le bouton **"Add New Project"**
4. Dans la section **"Import Third-Party Git Repository"**, descends et clique sur **"Import Git Repository"** → puis choisis **"Continue with GitHub"** si demandé.
5. **Méthode ultra-simple (sans repo) :**
   - Va directement ici : [https://vercel.com/new](https://vercel.com/new)
   - Clique sur **"Browse"** ou glisse-dépose le dossier entier `ParcoursParis`
   - Vercel va détecter automatiquement `index.html`
   - Clique sur **Deploy**

Tu auras une URL du type : `https://parcours-paris-xxx.vercel.app`

---

## Option 2 : Méthode propre (recommandée à long terme)

### Avec GitHub + Vercel

**Étape 1 : Installer Git (si pas déjà fait)**

1. Télécharge Git ici : https://git-scm.com/download/win
2. Installe-le avec les options par défaut.
3. Redémarre ton terminal PowerShell après l'installation.

**Étape 2 : Créer un repository GitHub**

1. Va sur [https://github.com](https://github.com) et connecte-toi.
2. Clique sur le bouton vert **"New"** (ou **"New repository"**).
3. Nomme-le : `parcours-paris` (ou ce que tu veux).
4. Laisse les options par défaut (Public ou Private selon ton choix).
5. Clique sur **"Create repository"**.

**Étape 3 : Initialiser Git localement**

Ouvre PowerShell et exécute les commandes suivantes :

```powershell
cd "$env:USERPROFILE\Projets\ParcoursParis"

git init
git add .
git commit -m "Initial commit - ParcoursParis ISAE-Supmeca"
```

**Étape 4 : Lier à GitHub**

Sur la page de ton nouveau repo GitHub, copie les commandes indiquées dans la section **"...or push an existing repository from the command line"**.

Exemple :

```powershell
git remote add origin https://github.com/TON_PSEUDO/parcours-paris.git
git branch -M main
git push -u origin main
```

**Étape 5 : Déployer sur Vercel**

1. Retourne sur [https://vercel.com](https://vercel.com)
2. Clique sur **"Add New Project"**
3. Tu devrais voir ton repo `parcours-paris` apparaître.
4. Clique sur **Import**.
5. Vercel va détecter automatiquement que c'est un site statique.
6. Clique sur **Deploy**.

---

## Après le déploiement

- Vercel te donne une URL propre.
- Tu peux la personnaliser dans les settings du projet (ex: `parcours-paris-isae.vercel.app`).
- Chaque fois que tu pushes sur GitHub, Vercel redéploie automatiquement.

---

## Conseils pour ta présentation

1. **Change le nom du projet** dans Vercel (Settings → General → Project Name) pour avoir une URL plus belle.
2. Ajoute éventuellement un petit footer avec le lien du repo GitHub pour montrer que c'est un vrai projet versionné.
3. Teste bien le site sur mobile avant la présentation.

---

## Besoin d'aide ?

Si tu bloques à une étape, envoie-moi un message avec l'erreur que tu vois.

Bonne présentation ! 🎓
