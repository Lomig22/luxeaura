# 🏆 LUXURA MONTE-CARLO

Site web premium haut de gamme pour une marque de luxe monégasque.

![Version](https://img.shields.io/badge/version-1.0.0-gold)
![License](https://img.shields.io/badge/license-MIT-blue)

## 📋 À Propos

**Luxura Monte-Carlo** est un site web vitrine premium conçu pour incarner l'excellence, le raffinement et l'art de vivre méditerranéen. Inspiré par l'esthétique des plus grandes maisons de luxe, ce site offre une expérience utilisateur fluide, élégante et orientée conversion.

### ✨ Caractéristiques Principales

- ✅ **Design Premium** : Interface épurée et sophistiquée
- ✅ **Responsive Mobile-First** : Optimisé pour tous les appareils
- ✅ **Animations Fluides** : Transitions et effets subtils (AOS, parallax)
- ✅ **Performance Optimisée** : Chargement rapide et images optimisées
- ✅ **SEO Ready** : Structure sémantique et meta tags optimisés
- ✅ **Boutique Élégante** : Système de filtres et présentation produits premium
- ✅ **Formulaires Fonctionnels** : Validation et notifications
- ✅ **Navigation Intuitive** : Menu sticky et smooth scroll

---

## 🎨 Design & Direction Artistique

### Palette de Couleurs

```css
Or Principal:   #C9A961  /* Primary Gold */
Or Foncé:       #B08D4F  /* Dark Gold */
Or Clair:       #E5D4A8  /* Light Gold */
Noir:           #0A0A0A  /* Black */
Anthracite:     #1A1A1A  /* Charcoal */
Gris Foncé:     #2A2A2A  /* Dark Gray */
Gris Moyen:     #666666  /* Medium Gray */
Gris Clair:     #CCCCCC  /* Light Gray */
Blanc:          #FFFFFF  /* White */
Ivoire:         #F8F6F3  /* Ivory */
```

### Typographie

- **Titres** : Playfair Display (Serif) - Élégant et haut de gamme
- **Corps de texte** : Inter (Sans-serif) - Moderne et lisible

### Style Visuel

- Minimal & premium
- Grandes images haute résolution
- Transitions fluides (cubic-bezier)
- Espacements généreux
- Grilles modernes (CSS Grid)

---

## 📁 Structure du Projet

```
luxeaura-main/
│
├── index.html              # Page d'accueil
├── boutique.html           # Page boutique avec filtres
├── about.html              # Page à propos / histoire
├── contact.html            # Page contact avec formulaire
│
├── css/
│   └── style.css          # Styles CSS complets (1000+ lignes)
│
├── js/
│   └── main.js            # JavaScript interactif
│
└── README.md              # Documentation
```

---

## 🚀 Installation & Utilisation

### Installation

1. **Cloner ou télécharger le projet**
```bash
cd luxeaura-main
```

2. **Ouvrir le site**
   - Ouvrez `index.html` dans votre navigateur
   - Ou utilisez un serveur local :

```bash
# Avec Python
python -m http.server 8000

# Avec Node.js (http-server)
npx http-server -p 8000

# Avec PHP
php -S localhost:8000
```

3. **Accéder au site**
```
http://localhost:8000
```

### Aucune Dépendance Locale Requise

Le site utilise des CDN pour :
- **Google Fonts** (Playfair Display, Inter)
- **Font Awesome** 6.4.0 (Icônes)
- **AOS** 2.3.1 (Animations au scroll)

Pas besoin de `npm install` ou `composer install` !

---

## 📄 Pages du Site

### 1. **Page d'Accueil** (`index.html`)

**Sections incluses :**
- ✨ Hero Section avec vidéo/image immersive
- 💎 Section Promesse (3 piliers : Artisanat, Expérience, Services VIP)
- 🛍️ Aperçu Produits (grille de 4 collections)
- 🌟 Section Expérience (split layout avec image)
- 📧 Newsletter (inscription)

**Objectif :** Capter l'attention et inspirer l'émotion

---

### 2. **Page Boutique** (`boutique.html`)

**Fonctionnalités :**
- 🔍 Système de filtrage par catégorie (Horlogerie, Accessoires, Joaillerie, Lifestyle)
- 🎨 Grille de produits responsive (8 produits exemple)
- 🔎 Zoom sur image au survol
- 💼 Badges (Nouveau, Exclusif)
- 🛒 Bouton "Ajouter au panier"
- 📄 Pagination
- 🎁 Bannière Services (livraison, garantie, etc.)

**Objectif :** Présenter les produits avec élégance et faciliter l'achat

---

### 3. **Page À Propos** (`about.html`)

**Sections incluses :**
- 📖 Histoire de la marque
- 💡 Valeurs (Excellence, Exclusivité, Élégance, Service)
- 💬 Citation inspirante du fondateur
- 🛠️ Savoir-faire d'exception
- 📅 Timeline (1987-2026)
- 📞 CTA vers boutique et contact

**Objectif :** Raconter une histoire émotionnelle et crédible

---

### 4. **Page Contact** (`contact.html`)

**Fonctionnalités :**
- 📝 Formulaire contact premium (validation front-end)
- 📍 Informations de contact (adresse, téléphone, email, horaires)
- 🗺️ Carte Google Maps intégrée
- 👑 Encart Service VIP
- ❓ FAQ Accordéon (4 questions)

**Objectif :** Faciliter la prise de contact et répondre aux questions

---

## ⚙️ Fonctionnalités JavaScript

Le fichier `js/main.js` inclut :

### Navigation
- ✅ Navbar sticky avec effet de scroll
- ✅ Menu mobile responsive (hamburger)
- ✅ Smooth scroll vers les ancres

### Animations
- ✅ Intégration AOS (Animate On Scroll)
- ✅ Effets de transition fluides
- ✅ Animations au hover

### Boutique
- ✅ Système de filtrage produits (JavaScript)
- ✅ Tri dynamique
- ✅ Zoom d'images (modal)

### Formulaires
- ✅ Validation email
- ✅ Gestion de soumission
- ✅ Notifications toast élégantes
- ✅ Protection contre les soumissions vides

### FAQ
- ✅ Accordéon interactif
- ✅ Animation d'ouverture/fermeture

### Panier (Exemple)
- ✅ Fonction `addToCart()`
- ✅ Stockage localStorage
- ✅ Mise à jour du badge

---

## 🎯 SEO & Performance

### SEO
- ✅ Meta descriptions optimisées
- ✅ Structure HTML sémantique (header, nav, main, section, footer)
- ✅ Titres hiérarchiques (H1, H2, H3...)
- ✅ Alt text sur toutes les images
- ✅ Schema markup ready

### Performance
- ✅ Images optimisées (Unsplash haute qualité)
- ✅ Lazy loading (optionnel)
- ✅ CSS minifiable
- ✅ JavaScript optimisé (debounce, throttle)

### Accessibilité
- ✅ Contraste suffisant (WCAG AA)
- ✅ Navigation au clavier
- ✅ ARIA labels (ready)
- ✅ Taille de police lisible

---

## 📱 Responsive Design

Le site s'adapte parfaitement à tous les écrans :

### Breakpoints
```css
Desktop:   1400px+  (layout large)
Laptop:    1024px   (adaptation grilles)
Tablet:    768px    (colonnes réduites)
Mobile:    < 768px  (menu hamburger, stack vertical)
```

### Mobile-First
- Menu hamburger élégant
- Grilles adaptées (1 colonne)
- Espacements réduits
- Boutons tactiles optimisés
- Images responsives

---

## 🎨 Personnalisation

### Modifier les Couleurs

Éditez les variables CSS dans `css/style.css` :

```css
:root {
    --primary-gold: #C9A961;
    --dark-gold: #B08D4F;
    /* ... autres couleurs */
}
```

### Changer les Polices

Remplacez les imports Google Fonts dans les fichiers HTML :

```html
<link href="https://fonts.googleapis.com/css2?family=VotrePolice..." rel="stylesheet">
```

Et modifiez les variables CSS :

```css
:root {
    --font-serif: 'VotrePoliceSerif', serif;
    --font-sans: 'VotrePolice', sans-serif;
}
```

### Modifier les Images

Remplacez les URLs Unsplash par vos propres images :

```html
<!-- Avant -->
<img src="https://images.unsplash.com/photo-xyz..." alt="...">

<!-- Après -->
<img src="images/mon-image.jpg" alt="...">
```

### Ajuster les Animations

Modifiez les durées et delays AOS dans `js/main.js` :

```javascript
AOS.init({
    duration: 1000,  // Durée en ms
    once: true,      // Animation une seule fois
    offset: 100      // Offset de déclenchement
});
```

---

## 🛠️ Intégration Backend

Le site est actuellement en **front-end pur**. Pour intégrer un backend :

### Formulaires
Remplacez les fonctions JavaScript par des appels API :

```javascript
// Dans js/main.js - fonction handleContactSubmit()
fetch('/api/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
})
.then(response => response.json())
.then(data => showNotification('Message envoyé !', 'success'));
```

### Boutique E-commerce
Intégrez avec :
- **Shopify API**
- **WooCommerce REST API**
- **Stripe** pour les paiements
- Votre propre API

### CMS
Intégrez avec :
- **WordPress** (thème custom)
- **Strapi** (headless CMS)
- **Contentful**
- **Sanity**

---

## 📊 Analytics & Tracking

### Google Analytics
Ajoutez avant `</head>` :

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Facebook Pixel
```html
<!-- Facebook Pixel -->
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
  n.queue=[];t=b.createElement(e);t.async=!0;
  t.src=v;s=b.getElementsByTagName(e)[0];
  s.parentNode.insertBefore(t,s)}(window, document,'script',
  'https://connect.facebook.net/en_US/fbevents.js');
  fbq('init', 'YOUR_PIXEL_ID');
  fbq('track', 'PageView');
</script>
```

---

## 🚀 Déploiement

### Hébergement Recommandé

**Gratuit :**
- 🌐 **Netlify** (recommandé) - Drag & drop
- 🌐 **Vercel** - Intégration Git
- 🌐 **GitHub Pages** - Pour projets publics
- 🌐 **Cloudflare Pages**

**Payant :**
- 💎 **OVH** - Hébergement français
- 💎 **Hostinger** - Abordable
- 💎 **SiteGround** - Performance
- 💎 **WP Engine** - Si WordPress

### Déploiement Netlify (1 minute)

1. Créez un compte sur [netlify.com](https://netlify.com)
2. Glissez-déposez le dossier `luxeaura-main/`
3. Votre site est en ligne ! 🎉

### Déploiement via Git

```bash
# Initialiser Git
git init
git add .
git commit -m "Initial commit - Luxura Monte-Carlo"

# Pousser sur GitHub
git remote add origin https://github.com/username/luxura-mc.git
git push -u origin main

# Connecter à Netlify/Vercel via l'interface
```

### Domaine Personnalisé

Une fois déployé, configurez votre domaine :
- `www.luxura-montecarlo.com`
- Certificat SSL automatique (gratuit)

---

## 📝 Copywriting & Textes

### Headlines Suggérés
- *"Luxe incarné. Expérience unique."*
- *"L'excellence à chaque instant."*
- *"Produits exclusifs pour une vie raffinée."*

### CTAs Performants
- **Découvrir** (soft)
- **Explorer la collection** (engagement)
- **Nous contacter** (direct)
- **Prendre rendez-vous VIP** (exclusif)

### Ton Rédactionnel
- ✅ Élégant mais accessible
- ✅ Court et impactant
- ✅ Évocateur d'émotion
- ✅ Pas de jargon complexe

---

## 🎁 Bonus Inclus

### Icônes
- ✅ Font Awesome 6.4.0 (2000+ icônes)

### Animations
- ✅ AOS (Animate On Scroll) intégré
- ✅ Effets de parallax (optionnel)
- ✅ Transitions CSS fluides

### Composants Réutilisables
- ✅ Cartes produits
- ✅ Boutons (primary, secondary, outline)
- ✅ Formulaires stylisés
- ✅ Notifications toast
- ✅ Modals (prêts à l'emploi)

---

## 🐛 Troubleshooting

### Le menu mobile ne s'ouvre pas
✅ Vérifiez que `js/main.js` est bien chargé
✅ Ouvrez la console (F12) pour voir les erreurs

### Les animations ne fonctionnent pas
✅ Vérifiez que le CDN AOS est chargé
✅ Vérifiez la connexion internet (CDN externe)

### Les images ne s'affichent pas
✅ Connexion internet requise (images Unsplash)
✅ Remplacez par vos propres images locales

### Le formulaire ne s'envoie pas
✅ C'est normal, il faut connecter un backend
✅ Utilisez Formspree, EmailJS ou votre API

---

## 📞 Support & Contact

Pour toute question ou demande de personnalisation :

📧 Email : votre-email@agency.com  
🌐 Site : www.votre-agency.com  
📱 Tél : +33 X XX XX XX XX

---

## 📜 Licence

MIT License - Libre d'utilisation pour projets personnels et commerciaux.

---

## 🙏 Crédits

**Développement** : DEV Agency  
**Design** : Inspiré par les plus grandes maisons de luxe  
**Images** : Unsplash (libre de droits)  
**Icônes** : Font Awesome  
**Animations** : AOS Library  

---

## 🔮 Évolutions Futures

### Phase 2 (Optionnelle)
- [ ] Intégration e-commerce complète (Stripe)
- [ ] Système de compte client
- [ ] Wishlist / Favoris
- [ ] Comparateur de produits
- [ ] Chat en direct (VIP support)
- [ ] Blog / Actualités
- [ ] Multilingue (FR/EN)
- [ ] PWA (Progressive Web App)

---

## ⭐ Remerciements

Merci d'avoir choisi ce template premium. Si vous l'appréciez, n'hésitez pas à :
- ⭐ Mettre une étoile sur GitHub
- 📢 Partager avec vos collègues
- 💬 Laisser un avis

---

**Fait avec 💛 et ☕ en 2026**

```
╔══════════════════════════════════════╗
║   LUXURA MONTE-CARLO                 ║
║   Premium Website Template           ║
║   Version 1.0.0                      ║
╚══════════════════════════════════════╝
```
