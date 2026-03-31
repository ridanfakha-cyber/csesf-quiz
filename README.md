# CSESF – Quiz Soft Skills 🏆

Outil de sélection de candidats pour le stage **Chargé(e) de communication & événementiel** du CSESF (Seine-Saint-Denis).

## 🚀 Déploiement

Ce projet est un **fichier HTML unique** (`index.html`) — aucune installation, aucune dépendance, aucun serveur requis.

### Option 1 — GitHub Pages (recommandé)
1. Push `index.html` sur la branche `main`
2. Aller dans **Settings → Pages**
3. Source : `main` / `/ (root)`
4. Le site sera accessible sur `https://TON-PSEUDO.github.io/csesf-quiz/`

### Option 2 — Fichier local
Ouvrir `index.html` directement dans un navigateur. Fonctionne sans connexion internet.

---

## 🔐 Code admin

```
CSESF2026
```

> À changer dans le fichier `index.html` à la ligne : `const ADMIN_CODE = 'CSESF2026';`

---

## 📋 Fonctionnalités

### Côté candidat
- Quiz de 10 questions – scénarios réalistes
- 5 soft skills évalués : Créativité, Initiative, Communication, Adaptabilité, Esprit d'équipe
- Page de confirmation sans scores visibles

### Côté admin (code requis)
- **Dashboard** avec statistiques globales
- **Fiche détaillée** par candidat : scores, réponses, analyses, verdict
- **Filtres** : Recommandé / À explorer / Insuffisant
- **Export CSV** (compatible Excel)
- **Backup JSON** + import pour transférer les données entre appareils
- **Suppression** individuelle ou totale

---

## 💾 Stockage des données

Les données sont stockées dans le **localStorage** du navigateur — elles persistent entre les sessions sur le même appareil/navigateur.

> ⚠️ Les données sont liées au navigateur utilisé. Utiliser **Backup JSON** pour sauvegarder et transférer.

---

## 🛠 Modifier le quiz

Tout est dans `index.html` :
- **Questions** → tableau `QUESTIONS` (ligne ~530)
- **Code admin** → constante `ADMIN_CODE` (ligne ~490)
- **Seuils de verdict** → fonction `saveAndConfirm()` (`>= 80` = Recommandé, `>= 60` = À explorer)

---

*CSESF – Association pour le sport inclusif en Seine-Saint-Denis*
