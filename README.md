# Philipp Ray Diffusion — Site Vitrine

Page vitrine one-page pour **Philipp Ray Diffusion**, hébergée sur GitHub Pages.

## 🌐 Live

https://philippraydiffusion.github.io/beyondcommunication/

---

## 📁 Structure

```
beyondcommunication/
├── index.html   # Page vitrine complète (HTML + CSS + JS)
├── .env         # Token GitHub local (jamais commité)
├── .gitignore
└── README.md
```

---

## 🚀 Pousser une mise à jour

```powershell
$env:TOKEN = (Get-Content .env | Select-String "GITHUB_TOKEN").ToString().Split("=")[1]
git remote set-url origin "https://PhilippRayDiffusion:$env:TOKEN@github.com/PhilippRayDiffusion/beyondcommunication.git"
git add .
git commit -m "Update"
git push origin main
git remote set-url origin https://github.com/PhilippRayDiffusion/beyondcommunication.git
```

---

## 🔑 Credentials

Le fichier `.env` (local uniquement) contient :

```
GITHUB_TOKEN=ghp_...
GITHUB_USER=PhilippRayDiffusion
GITHUB_REPO=beyondcommunication
```

> Ne jamais commiter le fichier `.env`.
