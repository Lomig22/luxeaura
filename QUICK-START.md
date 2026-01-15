# ⚡ DÉMARRAGE RAPIDE - LUXURA MONTE-CARLO

Guide ultra-rapide pour lancer votre site en 5 minutes ! ⏱️

---

## 🚀 OPTION 1 : Ouvrir Directement (Le Plus Simple)

### Étape 1 : Ouvrir le fichier
```
Double-cliquez sur : index.html
```

✅ **C'est tout !** Votre site s'ouvre dans votre navigateur par défaut.

---

## 🌐 OPTION 2 : Avec un Serveur Local (Recommandé)

### Pourquoi un serveur local ?
- ✅ URLs plus propres
- ✅ Meilleure simulation de production
- ✅ Évite les problèmes CORS

### A. Avec Python (Déjà installé sur Mac/Linux)

```bash
# Ouvrir le Terminal
cd "/Users/admin/DEV AGENCY/DEV/luxeaura-main"

# Lancer le serveur
python3 -m http.server 8000

# Ou avec Python 2
python -m SimpleHTTPServer 8000
```

**Ouvrir** : http://localhost:8000

---

### B. Avec Node.js (http-server)

```bash
# Installer http-server (une seule fois)
npm install -g http-server

# Dans le dossier du projet
cd "/Users/admin/DEV AGENCY/DEV/luxeaura-main"

# Lancer
http-server -p 8000

# Ou avec npx (sans installation)
npx http-server -p 8000
```

**Ouvrir** : http://localhost:8000

---

### C. Avec PHP (Déjà installé sur Mac)

```bash
cd "/Users/admin/DEV AGENCY/DEV/luxeaura-main"
php -S localhost:8000
```

**Ouvrir** : http://localhost:8000

---

### D. Avec Visual Studio Code (Live Server)

1. Ouvrir le projet dans VS Code
2. Installer l'extension "Live Server"
3. Clic droit sur `index.html` → "Open with Live Server"

✅ Le site s'ouvre automatiquement avec rechargement automatique !

---

## 📱 TESTER EN RESPONSIVE

### Raccourcis Navigateur

**Chrome / Edge / Brave** :
```
Cmd + Option + I (Mac)
Ctrl + Shift + I (Windows)

Puis cliquer sur l'icône 📱 (Toggle device toolbar)
```

**Firefox** :
```
Cmd + Option + M (Mac)
Ctrl + Shift + M (Windows)
```

**Safari** :
```
Développement → Entrer en mode Responsive Design
```

### Tailles à Tester

- 📱 **iPhone 12/13/14** : 390x844px
- 📱 **iPhone 14 Pro Max** : 430x932px
- 📱 **Samsung Galaxy S21** : 360x800px
- 📲 **iPad** : 768x1024px
- 📲 **iPad Pro** : 1024x1366px
- 💻 **Laptop** : 1366x768px
- 🖥️ **Desktop** : 1920x1080px

---

## ✏️ PERSONNALISATION RAPIDE

### Changer le Nom de la Marque

**Rechercher** : `LUXURA`  
**Remplacer par** : `VOTRE MARQUE`

**Fichiers concernés** :
- `index.html`
- `boutique.html`
- `about.html`
- `contact.html`
- `css/style.css`

---

### Changer les Couleurs

**Fichier** : `css/style.css`  
**Ligne** : ~17-27

```css
:root {
    --primary-gold: #VOTRE_COULEUR;  /* Changez ici */
    --dark-gold: #VOTRE_COULEUR_FONCEE;
    /* ... */
}
```

**Couleurs suggérées** :

**Or/Gold** (actuel) :
- `#C9A961` (or classique)

**Alternatives luxe** :
- `#8B7355` (bronze)
- `#B87333` (cuivre)
- `#CD7F32` (bronze antique)
- `#E5C287` (champagne)
- `#4A4A4A` (gris anthracite)
- `#2C2C2C` (noir premium)

---

### Changer les Images

**Rechercher** : `images.unsplash.com`

**Option 1 - Garder Unsplash** :
1. Aller sur [unsplash.com](https://unsplash.com)
2. Chercher : `luxury watch`, `monaco`, `jewelry`, etc.
3. Copier l'URL de l'image
4. Remplacer dans le HTML

**Option 2 - Vos propres images** :
1. Créer un dossier `/images/`
2. Ajouter vos photos
3. Remplacer les URLs :

```html
<!-- Avant -->
<img src="https://images.unsplash.com/photo-xyz..." alt="...">

<!-- Après -->
<img src="images/ma-photo.jpg" alt="...">
```

---

### Modifier les Textes

**Fichiers HTML** : Remplacez directement le texte entre les balises

```html
<!-- Exemple -->
<h1>Luxe. Élégance. Expérience Monte-Carlo.</h1>
<!-- Devient -->
<h1>Votre Titre Personnalisé</h1>
```

💡 **Astuce** : Utilisez le fichier `CONTENT-GUIDE.md` pour des suggestions de textes.

---

## 🔗 LIENS À CONFIGURER

### Réseaux Sociaux (Footer)

**Fichier** : Tous les `.html`  
**Section** : Footer

```html
<!-- Ligne ~XXX -->
<a href="#"><i class="fab fa-instagram"></i></a>
<!-- Remplacer par -->
<a href="https://instagram.com/votre_compte"><i class="fab fa-instagram"></i></a>
```

À faire pour :
- Instagram
- Facebook
- Pinterest
- LinkedIn

---

### Informations de Contact

**Rechercher et remplacer** :

```html
<!-- Adresse -->
Place du Casino, 98000 Monte-Carlo
→ Votre adresse réelle

<!-- Téléphone -->
+377 XX XX XX XX
→ Votre numéro

<!-- Email -->
contact@luxura-mc.com
→ votre-email@domaine.com
```

---

## 📧 CONNECTER LES FORMULAIRES

### Option A : Formspree (Gratuit & Simple)

1. Créer un compte sur [formspree.io](https://formspree.io)
2. Créer un nouveau formulaire
3. Copier l'URL du endpoint
4. Modifier `contact.html` :

```html
<form action="https://formspree.io/f/VOTRE_ID" method="POST">
```

---

### Option B : EmailJS (Frontend Only)

1. Créer un compte sur [emailjs.com](https://emailjs.com)
2. Configurer un service email
3. Suivre leur guide d'intégration
4. Modifier `js/main.js` (fonction `handleContactSubmit`)

---

### Option C : Votre Backend

Modifier `js/main.js` ligne ~170 :

```javascript
fetch('https://votre-api.com/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
})
```

---

## 🚀 DÉPLOIEMENT EN LIGNE

### 1️⃣ NETLIFY (Le Plus Simple)

**Durée** : 2 minutes ⏱️

1. Aller sur [netlify.com](https://netlify.com)
2. Créer un compte (gratuit)
3. **Glisser-déposer** le dossier `luxeaura-main/`
4. ✅ **Site en ligne !**

**URL gratuite** : `votre-site.netlify.app`

**Domaine personnalisé** : Configurable dans les settings

---

### 2️⃣ VERCEL

```bash
# Installer Vercel CLI
npm install -g vercel

# Dans le dossier du projet
cd "/Users/admin/DEV AGENCY/DEV/luxeaura-main"

# Déployer
vercel

# Suivre les instructions
```

---

### 3️⃣ GITHUB PAGES

```bash
# Initialiser Git
git init
git add .
git commit -m "Initial commit"

# Créer un repo sur GitHub
# Puis :
git remote add origin https://github.com/USERNAME/luxura-mc.git
git push -u origin main

# Activer GitHub Pages dans Settings
```

**URL** : `username.github.io/luxura-mc`

---

### 4️⃣ FTP (Hébergement Traditionnel)

**Logiciel FTP recommandé** :
- **FileZilla** (gratuit, multi-plateforme)
- **Cyberduck** (gratuit, Mac)
- **Transmit** (payant, Mac, puissant)

**Étapes** :
1. Obtenir identifiants FTP de votre hébergeur
2. Se connecter avec le logiciel FTP
3. Uploader tous les fichiers dans `/public_html/` ou `/www/`
4. Vérifier sur votre domaine

---

## 🎨 AJOUTER GOOGLE FONTS PERSONNALISÉES

**Fichier** : Tous les `.html`  
**Section** : `<head>`

```html
<!-- Remplacer -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display..." rel="stylesheet">

<!-- Par vos polices (exemple avec Cormorant & Montserrat) -->
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600;700&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
```

Puis dans `css/style.css` :

```css
:root {
    --font-serif: 'Cormorant Garamond', serif;
    --font-sans: 'Montserrat', sans-serif;
}
```

---

## 📊 AJOUTER GOOGLE ANALYTICS

**Fichier** : Tous les `.html`  
**Position** : Avant `</head>`

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

**Obtenir l'ID** :
1. Créer un compte [analytics.google.com](https://analytics.google.com)
2. Créer une propriété
3. Copier l'ID de mesure (G-XXXXXXXXXX)

---

## ✅ CHECKLIST AVANT MISE EN LIGNE

### Contenu
- [ ] Nom de marque personnalisé
- [ ] Textes relus (pas de "Lorem ipsum")
- [ ] Coordonnées de contact à jour
- [ ] Prix cohérents
- [ ] Liens réseaux sociaux configurés

### Technique
- [ ] Formulaires connectés (Formspree, EmailJS, etc.)
- [ ] Google Analytics ajouté
- [ ] Favicon personnalisé (icône navigateur)
- [ ] Meta descriptions modifiées (SEO)
- [ ] Images optimisées (< 500Ko chacune)

### Design
- [ ] Couleurs personnalisées (si souhaité)
- [ ] Logo ajouté
- [ ] Images remplacées (si Unsplash non souhaité)
- [ ] Polices personnalisées (optionnel)

### Test
- [ ] Testé sur Chrome
- [ ] Testé sur Safari
- [ ] Testé sur Firefox
- [ ] Testé sur mobile (iPhone)
- [ ] Testé sur mobile (Android)
- [ ] Testé sur tablette
- [ ] Tous les liens fonctionnent
- [ ] Formulaires s'envoient

---

## 🆘 PROBLÈMES FRÉQUENTS

### ❌ Les icônes ne s'affichent pas
**Solution** : Vérifier la connexion internet (Font Awesome via CDN)

### ❌ Les animations ne fonctionnent pas
**Solution** : Vérifier que AOS est chargé (CDN) et `js/main.js` aussi

### ❌ Le menu mobile ne s'ouvre pas
**Solution** : Ouvrir la console (F12), vérifier les erreurs JavaScript

### ❌ Le formulaire ne s'envoie pas
**Solution** : Normal, connecter à Formspree ou EmailJS (voir section Formulaires)

### ❌ Les images sont lentes à charger
**Solution** : 
1. Télécharger les images d'Unsplash
2. Les optimiser avec [tinypng.com](https://tinypng.com)
3. Les héberger localement (`/images/`)

---

## 📞 SUPPORT

**Problème technique ?**
- 📖 Consultez le `README.md` (documentation complète)
- 📝 Consultez le `CONTENT-GUIDE.md` (suggestions contenu)
- 💬 Ouvrez une issue sur GitHub (si applicable)

---

## 🎓 RESSOURCES UTILES

### Apprendre
- [MDN Web Docs](https://developer.mozilla.org) - Documentation HTML/CSS/JS
- [W3Schools](https://w3schools.com) - Tutoriels débutants
- [CSS-Tricks](https://css-tricks.com) - Astuces CSS

### Outils
- [Unsplash](https://unsplash.com) - Photos gratuites haute qualité
- [Font Awesome](https://fontawesome.com) - Icônes
- [Google Fonts](https://fonts.google.com) - Polices gratuites
- [TinyPNG](https://tinypng.com) - Compression images
- [Can I Use](https://caniuse.com) - Compatibilité navigateurs

### Inspiration
- [Awwwards](https://awwwards.com) - Sites primés
- [Dribbble](https://dribbble.com) - Designs
- [Behance](https://behance.net) - Portfolios créatifs

---

## ✨ PROCHAINES ÉTAPES

**Niveau 1 - Essentiel** ✅
- [x] Personnaliser les textes
- [x] Ajouter vos images
- [x] Configurer les contacts
- [x] Connecter les formulaires
- [x] Déployer en ligne

**Niveau 2 - Amélioration** 🚀
- [ ] Ajouter Google Analytics
- [ ] Optimiser les images
- [ ] Configurer un domaine personnalisé
- [ ] Ajouter plus de produits
- [ ] Créer du contenu (blog)

**Niveau 3 - Avancé** 💎
- [ ] Intégrer un vrai e-commerce (Shopify, WooCommerce)
- [ ] Ajouter un système de paiement (Stripe)
- [ ] Créer un espace client
- [ ] Multilingue (FR/EN)
- [ ] PWA (Progressive Web App)

---

## 🎉 FÉLICITATIONS !

Vous avez maintenant un site web premium fonctionnel !

**Partagez votre création** :
- 📸 Screenshot sur Instagram
- 💼 Ajoutez à votre portfolio
- 🌟 Montrez à vos clients

---

**Besoin d'aide ?** Relisez ce guide ou consultez le README.md complet.

**Bonne chance avec votre projet ! 🚀✨**

---

**Version** : 1.0  
**Dernière mise à jour** : Janvier 2026  
**Durée de lecture** : 10 minutes ⏱️
