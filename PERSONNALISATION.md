# 🎨 GUIDE DE PERSONNALISATION - LUXURA MONTE-CARLO

Guide complet pour adapter le site à votre marque en quelques minutes.

---

## 🏷️ 1. CHANGER LE NOM DE LA MARQUE

### A. Rechercher & Remplacer

**Texte à chercher** : `LUXURA`  
**Remplacer par** : `VOTRE MARQUE`

**Fichiers concernés** :
- ✅ `index.html`
- ✅ `boutique.html`
- ✅ `about.html`
- ✅ `contact.html`
- ✅ `README.md`

### B. Parties spécifiques

**"Monte-Carlo"** → Remplacer par votre ville/région :
```html
<!-- Avant -->
<span class="monte-carlo">Monte-Carlo</span>

<!-- Après -->
<span class="monte-carlo">Paris</span>
<!-- ou -->
<span class="monte-carlo">Geneva</span>
```

---

## 🎨 2. CHANGER LES COULEURS

### Option A : Personnalisation Rapide

**Fichier** : `css/style.css`  
**Lignes** : 17-27

```css
:root {
    /* Changez UNIQUEMENT cette ligne pour tout transformer */
    --primary-gold: #VOTRE_COULEUR;  /* ← ICI */
    --dark-gold: #VOTRE_COULEUR_FONCEE;
    --light-gold: #VOTRE_COULEUR_CLAIRE;
    
    /* Le reste peut rester identique */
    --black: #0A0A0A;
    --charcoal: #1A1A1A;
    --white: #FFFFFF;
    --ivory: #F8F6F3;
}
```

---

### Option B : Palettes Prédéfinies

#### 🥇 OR CLASSIQUE (Actuel)
```css
:root {
    --primary-gold: #C9A961;
    --dark-gold: #B08D4F;
    --light-gold: #E5D4A8;
}
```

#### 🥉 BRONZE ÉLÉGANT
```css
:root {
    --primary-gold: #8B7355;
    --dark-gold: #6B5643;
    --light-gold: #A8927B;
}
```

#### 💎 BLEU ROYAL
```css
:root {
    --primary-gold: #2C5F8D;
    --dark-gold: #1A4060;
    --light-gold: #4A7FA7;
}
```

#### 🌿 VERT ÉMERAUDE
```css
:root {
    --primary-gold: #2E7C67;
    --dark-gold: #1F5548;
    --light-gold: #45A88F;
}
```

#### 🍷 BORDEAUX PREMIUM
```css
:root {
    --primary-gold: #8B2F39;
    --dark-gold: #6B1F29;
    --light-gold: #AB4F59;
}
```

#### 🌑 NOIR PREMIUM (Ultra minimaliste)
```css
:root {
    --primary-gold: #2C2C2C;
    --dark-gold: #1A1A1A;
    --light-gold: #4A4A4A;
}
```

#### 🥈 ARGENT MODERNE
```css
:root {
    --primary-gold: #8E8E93;
    --dark-gold: #636366;
    --light-gold: #AEAEB2;
}
```

---

### Option C : Palette Personnalisée Complète

Pour un contrôle total, éditez toutes les couleurs :

```css
:root {
    /* Couleur primaire (CTAs, accents) */
    --primary-gold: #VOTRE_PRIMAIRE;
    --dark-gold: #VOTRE_PRIMAIRE_FONCEE;
    --light-gold: #VOTRE_PRIMAIRE_CLAIRE;
    
    /* Couleurs de fond */
    --black: #000000;
    --charcoal: #1A1A1A;
    --dark-gray: #2A2A2A;
    --ivory: #F8F6F3;
    --white: #FFFFFF;
    
    /* Couleurs texte */
    --medium-gray: #666666;
    --light-gray: #CCCCCC;
}
```

---

## 🖼️ 3. REMPLACER LES IMAGES

### A. Structure recommandée

Créez un dossier `/images/` :

```
luxeaura-main/
├── images/
│   ├── hero.jpg (1920x1080px)
│   ├── products/
│   │   ├── product-1.jpg (800x1000px)
│   │   ├── product-2.jpg
│   │   └── ...
│   ├── about/
│   │   ├── story.jpg
│   │   └── craftsmanship.jpg
│   └── logo.svg
```

### B. Remplacer les URLs

**Exemple Hero Section** :

```html
<!-- AVANT (Unsplash) -->
<div class="hero-image" style="background-image: url('https://images.unsplash.com/photo-xyz...');"></div>

<!-- APRÈS (Local) -->
<div class="hero-image" style="background-image: url('images/hero.jpg');"></div>
```

**Exemple Produit** :

```html
<!-- AVANT -->
<img src="https://images.unsplash.com/photo-xyz..." alt="Montre">

<!-- APRÈS -->
<img src="images/products/montre-excellence.jpg" alt="Montre Excellence">
```

### C. Optimiser les images

**Outils recommandés** :
- [TinyPNG](https://tinypng.com) - Compression sans perte
- [Squoosh](https://squoosh.app) - Compression avancée
- [ImageOptim](https://imageoptim.com/mac) - Mac only

**Formats recommandés** :
- **JPG** : Photos produits, lifestyle (qualité 80-85%)
- **PNG** : Logos, icônes avec transparence
- **WebP** : Format moderne (50% plus léger)
- **SVG** : Logo vectoriel (scalable)

**Poids maximum** :
- Hero : < 800Ko
- Produits : < 200Ko
- Thumbnails : < 100Ko

---

## ✏️ 4. CHANGER LA TYPOGRAPHIE

### A. Google Fonts (Recommandé)

**Étape 1** : Choisissez vos polices sur [fonts.google.com](https://fonts.google.com)

**Étape 2** : Remplacez le lien dans **TOUS** les fichiers HTML :

```html
<!-- AVANT (dans <head>) -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

<!-- APRÈS (exemple avec Cormorant & Montserrat) -->
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600;700&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
```

**Étape 3** : Modifiez `css/style.css` (ligne ~23) :

```css
:root {
    /* AVANT */
    --font-serif: 'Playfair Display', serif;
    --font-sans: 'Inter', sans-serif;
    
    /* APRÈS */
    --font-serif: 'Cormorant Garamond', serif;
    --font-sans: 'Montserrat', sans-serif;
}
```

### B. Combinaisons recommandées

#### 🎩 Élégant Classique (Actuel)
```css
--font-serif: 'Playfair Display', serif;  /* Titres */
--font-sans: 'Inter', sans-serif;         /* Texte */
```

#### 👔 Moderne Sophistiqué
```css
--font-serif: 'Cormorant Garamond', serif;
--font-sans: 'Montserrat', sans-serif;
```

#### 💼 Corporate Luxe
```css
--font-serif: 'Libre Baskerville', serif;
--font-sans: 'Raleway', sans-serif;
```

#### 🏛️ Classique Intemporel
```css
--font-serif: 'Merriweather', serif;
--font-sans: 'Open Sans', sans-serif;
```

#### ✨ Ultra Premium
```css
--font-serif: 'Cinzel', serif;
--font-sans: 'Lato', sans-serif;
```

#### 🎨 Créatif Moderne
```css
--font-serif: 'Spectral', serif;
--font-sans: 'Work Sans', sans-serif;
```

---

## 📝 5. MODIFIER LES TEXTES

### A. Headlines (Titres principaux)

**Fichier** : `index.html`

```html
<!-- Hero Title -->
<h1 class="hero-title">
    Luxe. Élégance.<br>Expérience Monte-Carlo.
</h1>

<!-- Personnaliser -->
<h1 class="hero-title">
    Votre Titre<br>Sur Mesure.
</h1>
```

**Exemples alternatifs** :
- *"Excellence. Innovation. Passion."*
- *"L'Art du Raffinement Absolu"*
- *"Créations d'Exception Depuis 1987"*
- *"Où le Luxe Rencontre l'Émotion"*

### B. Sous-titres

```html
<!-- Hero Subtitle -->
<p class="hero-subtitle">
    Découvrez l'univers Luxura : raffinement, savoir-faire et exclusivité.
</p>

<!-- Personnaliser -->
<p class="hero-subtitle">
    Votre message personnalisé ici.
</p>
```

### C. CTAs (Call-to-Actions)

**Fichier** : Tous les `.html`

```html
<!-- Boutons principaux -->
<a href="#" class="btn btn-primary">Découvrir</a>
<a href="#" class="btn btn-secondary">Explorer</a>

<!-- Alternatives -->
<a href="#" class="btn btn-primary">Voir la collection</a>
<a href="#" class="btn btn-primary">Prendre rendez-vous</a>
<a href="#" class="btn btn-primary">Nous contacter</a>
```

---

## 🏢 6. METTRE À JOUR LES INFORMATIONS DE CONTACT

### A. Coordonnées

**Fichier** : Tous les `.html` (footer + contact.html)

```html
<!-- AVANT -->
<li><i class="fas fa-map-marker-alt"></i> Monte-Carlo, Monaco</li>
<li><i class="fas fa-phone"></i> +377 XX XX XX XX</li>
<li><i class="fas fa-envelope"></i> contact@luxura-mc.com</li>

<!-- APRÈS -->
<li><i class="fas fa-map-marker-alt"></i> 123 Avenue des Champs-Élysées, 75008 Paris</li>
<li><i class="fas fa-phone"></i> +33 1 XX XX XX XX</li>
<li><i class="fas fa-envelope"></i> contact@votremarque.com</li>
```

### B. Horaires

**Fichier** : `contact.html`

```html
<!-- À personnaliser -->
<p>Lundi - Samedi : 10h - 19h</p>
<p>Dimanche : Sur rendez-vous</p>

<!-- Exemples -->
<p>Lundi - Vendredi : 9h - 18h</p>
<p>Samedi : 10h - 17h</p>
<p>Dimanche : Fermé</p>
```

---

## 🌐 7. CONFIGURER LES RÉSEAUX SOCIAUX

**Fichier** : Tous les `.html` (footer)

```html
<!-- AVANT (liens placeholder) -->
<a href="#"><i class="fab fa-instagram"></i></a>
<a href="#"><i class="fab fa-facebook-f"></i></a>
<a href="#"><i class="fab fa-pinterest-p"></i></a>
<a href="#"><i class="fab fa-linkedin-in"></i></a>

<!-- APRÈS (vrais liens) -->
<a href="https://instagram.com/votre_compte" target="_blank"><i class="fab fa-instagram"></i></a>
<a href="https://facebook.com/votre_page" target="_blank"><i class="fab fa-facebook-f"></i></a>
<a href="https://pinterest.com/votre_profil" target="_blank"><i class="fab fa-pinterest-p"></i></a>
<a href="https://linkedin.com/company/votre_entreprise" target="_blank"><i class="fab fa-linkedin-in"></i></a>
```

**N'oubliez pas** `target="_blank"` pour ouvrir dans un nouvel onglet !

---

## 🎯 8. AJOUTER VOTRE LOGO

### A. Préparer le logo

**Format recommandé** : SVG (vectoriel, scalable)  
**Alternative** : PNG transparent (2x resolution)

**Dimensions** :
- **Header** : 200x60px (ratio 3:1)
- **Footer** : 150x50px

### B. Remplacer le texte par une image

**Fichier** : Tous les `.html`

```html
<!-- AVANT (texte) -->
<div class="logo">
    <a href="index.html">LUXURA <span class="monte-carlo">Monte-Carlo</span></a>
</div>

<!-- APRÈS (image) -->
<div class="logo">
    <a href="index.html">
        <img src="images/logo.svg" alt="Votre Marque" style="height: 50px;">
    </a>
</div>
```

### C. Ajuster les styles (optionnel)

**Fichier** : `css/style.css`

```css
/* Si vous utilisez une image logo */
.logo img {
    height: 50px;
    width: auto;
    transition: var(--transition-smooth);
}

.navbar.scrolled .logo img {
    height: 40px; /* Plus petit au scroll */
}
```

---

## 🖌️ 9. PERSONNALISER LES ANIMATIONS

### A. Vitesse des animations

**Fichier** : `js/main.js` (ligne ~43)

```javascript
// AVANT
AOS.init({
    duration: 1000,  // 1 seconde
    once: true,
    offset: 100
});

// APRÈS (plus rapide)
AOS.init({
    duration: 600,   // 0.6 seconde
    once: true,
    offset: 100
});

// APRÈS (plus lent/dramatique)
AOS.init({
    duration: 1500,  // 1.5 secondes
    once: true,
    offset: 100
});
```

### B. Répéter les animations (ou pas)

```javascript
// Animation UNE FOIS (recommandé)
once: true

// Animation À CHAQUE SCROLL (peut être lourd)
once: false
```

### C. Désactiver complètement les animations

**Option 1** : Commenter l'initialisation

```javascript
// AOS.init({ ... });
```

**Option 2** : Retirer AOS des HTML

```html
<!-- Supprimer cette ligne de tous les .html -->
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>

<!-- Et supprimer tous les attributs data-aos -->
<div data-aos="fade-up">  <!-- ← Supprimer data-aos -->
```

---

## 🎨 10. STYLES AVANCÉS

### A. Changer le style des boutons

**Fichier** : `css/style.css` (lignes ~403-442)

**Bouton principal arrondi** :

```css
.btn-primary {
    background: var(--primary-gold);
    color: var(--white);
    border-radius: 50px;  /* ← Ajouter */
}
```

**Bouton avec ombre forte** :

```css
.btn-primary {
    background: var(--primary-gold);
    color: var(--white);
    box-shadow: 0 10px 30px rgba(201, 169, 97, 0.4);  /* ← Ajouter */
}
```

**Bouton avec gradient** :

```css
.btn-primary {
    background: linear-gradient(135deg, var(--primary-gold), var(--dark-gold));
    color: var(--white);
}
```

### B. Modifier l'espacement général

**Fichier** : `css/style.css` (ligne ~24)

```css
:root {
    /* AVANT */
    --section-padding: 100px;
    
    /* APRÈS (plus compact) */
    --section-padding: 60px;
    
    /* APRÈS (plus aéré) */
    --section-padding: 150px;
}
```

### C. Changer la largeur du container

**Fichier** : `css/style.css` (ligne ~84)

```css
.container {
    /* AVANT */
    max-width: 1400px;
    
    /* APRÈS (plus étroit) */
    max-width: 1200px;
    
    /* APRÈS (plus large) */
    max-width: 1600px;
}
```

---

## 🛠️ 11. PERSONNALISATIONS RAPIDES BONUS

### A. Ajouter un favicon

**1. Créer un favicon** : [favicon.io](https://favicon.io)

**2. Ajouter dans `<head>` de tous les HTML** :

```html
<link rel="icon" type="image/png" sizes="32x32" href="images/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="images/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="images/apple-touch-icon.png">
```

### B. Changer le copyright

**Fichier** : Tous les `.html` (footer)

```html
<!-- AVANT -->
<p>&copy; 2026 Luxura Monte-Carlo. Tous droits réservés.</p>

<!-- APRÈS -->
<p>&copy; 2026 Votre Marque. Tous droits réservés.</p>
```

### C. Personnaliser le message console

**Fichier** : `js/main.js` (fin du fichier)

```javascript
// AVANT
console.log('%cLUXURA MONTE-CARLO', 'font-size: 24px; font-weight: bold; color: #C9A961;');
console.log('%cWebsite by Premium Dev Agency', 'font-size: 12px; color: #666;');

// APRÈS
console.log('%cVOTRE MARQUE', 'font-size: 24px; font-weight: bold; color: #C9A961;');
console.log('%cDéveloppé avec ❤️ par Votre Agence', 'font-size: 12px; color: #666;');
```

---

## 📋 CHECKLIST PERSONNALISATION

Avant de déployer, vérifiez :

### Identité visuelle
- [ ] Nom de marque remplacé partout
- [ ] Logo ajouté (header + footer + favicon)
- [ ] Couleurs personnalisées (palette cohérente)
- [ ] Polices changées (si souhaité)

### Contenu
- [ ] Tous les textes adaptés à votre marque
- [ ] Images remplacées ou optimisées
- [ ] CTAs personnalisés
- [ ] Produits/services mis à jour

### Contact
- [ ] Adresse postale correcte
- [ ] Numéro de téléphone à jour
- [ ] Email professionnel configuré
- [ ] Liens réseaux sociaux valides
- [ ] Horaires d'ouverture corrects

### Technique
- [ ] Google Analytics ID ajouté
- [ ] Formulaire connecté (Formspree/EmailJS)
- [ ] Favicon généré et ajouté
- [ ] Meta descriptions personnalisées
- [ ] Copyright à jour

---

## 💡 CONSEILS PRO

### 1. Cohérence visuelle
✅ Restez cohérent dans vos choix (couleurs, polices, espacements)  
✅ Maximum 2 polices (1 serif + 1 sans-serif)  
✅ Maximum 3 couleurs principales

### 2. Performance
✅ Optimisez TOUTES les images avant upload  
✅ Utilisez des formats modernes (WebP)  
✅ Activez la compression serveur (Gzip)

### 3. Accessibilité
✅ Vérifiez le contraste texte/fond ([WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/))  
✅ Testez la navigation au clavier (Tab)  
✅ Ajoutez des alt text descriptifs

### 4. Mobile First
✅ Testez sur **plusieurs tailles** d'écran  
✅ Vérifiez la lisibilité des textes  
✅ Assurez-vous que les boutons sont tactiles (min 44x44px)

---

## 🆘 DÉPANNAGE

### "Ma couleur ne s'applique pas"
✅ Vérifiez que vous modifiez bien `css/style.css`  
✅ Videz le cache navigateur (Ctrl+Shift+R / Cmd+Shift+R)  
✅ Cherchez si la couleur est en dur ailleurs dans le CSS

### "Ma police ne charge pas"
✅ Vérifiez le lien Google Fonts dans TOUS les HTML  
✅ Vérifiez l'orthographe exacte dans `--font-serif` / `--font-sans`  
✅ Testez avec une connexion internet active (CDN externe)

### "Mon logo est trop grand/petit"
✅ Ajustez `height` dans le style inline : `style="height: XXpx;"`  
✅ Ou créez une règle CSS spécifique (voir section 8.C)

---

## 🎓 RESSOURCES UTILES

### Design
- [Coolors.co](https://coolors.co) - Générateur de palettes
- [Adobe Color](https://color.adobe.com) - Roue chromatique
- [Paletton](https://paletton.com) - Harmonies de couleurs

### Typographie
- [Google Fonts](https://fonts.google.com) - Polices gratuites
- [FontPair](https://fontpair.co) - Associations de polices
- [Type Scale](https://type-scale.com) - Hiérarchie typographique

### Images
- [Unsplash](https://unsplash.com) - Photos gratuites HD
- [Pexels](https://pexels.com) - Photos + vidéos
- [TinyPNG](https://tinypng.com) - Compression

---

**🎨 Personnalisation terminée !**

N'hésitez pas à expérimenter et faire plusieurs tests avant le déploiement final.

**Astuce** : Dupliquez le dossier pour garder une version originale de sauvegarde !

---

**Version** : 1.0  
**Dernière MAJ** : Janvier 2026
