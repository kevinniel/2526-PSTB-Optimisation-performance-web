# Cours Optimisation de la Performance Web

## Importance 
- Crédibilité du site
- Si la page est trop longue à charger, les gens partent
- Si business de vente en ligne : attention si les gens partent on perd le business.

### Les éléments d'importance
- UX/UI est favorisé par l'optimisation des performances
- SEO : implicitement amélioré si le site est plus rapide
- COÛTS : plus le site est optimisé, moins il coûte cher à maintenir et à héberger  

## Les éléments du chargement d'une page web

Sur lesquels peut-on agir ?

- ❌ DNS
- ✅ Requête HTTP(s)
- ✅ Réponse serveur
- ✅ Parsing HTML
- ✅ Chargement des fichiers (CSS, JS, IMG, etc...)
- ✅ Construction du DOM
- ✅ Rendu (visuel)
- ✅ Exécution du JS
- ✅ Interactions utilisateurs


## Hébergement
1. Hébergement classique (ex: https://www.hostinger.com/fr/tarifs)
    - ➕ : pas cher, simple et rapide pour un wordpress ou un site static
    - ➖ : bande passante limitée (souvent), peu d'espace de stockage, vous n'êtes pas libre des technologies
2. VPS ou serveur dédié : 
    - ➕ : vous avez le contrôle total sur la machine
    - ➖ : un peu plus cher, temps d'administration
3. Cloud
    - ➕ : S'adapte aux besoins, Vous payez à la consommation
    - ➖ : Un peu galère au début de s'y retrouver dans les offres.

## Technologies utilisées
- Toutes les technologies sont **BIEN**.
- Choisissez les technologies en fonction des besoins du projet.
- HTTP2 au lieu de HTTP

## Code

- Réduire la quantité de code "rendu" (renvoyé par le serveur pour affichage) pour alléger le poids des téléchargements de fichiers externes.
- Optimisation des performances du code côté back (algorithmique)
- Requêtes en base de données
- ASYNC / DEFER : qui permettent de gérer des fichiers JS en asynchrone (en terme de chargement)

## SEO (Référencement)
- Balises de référencement (meta, OpenGraph, sémantique HTML, etc...)
- Microdatas : données qui permettent d'apporter des éléments de précision sur une partie du contenu d'une page
- Vitesse de chargement de la page : optimisation de la taille des fichiers (images, CSS, JS, Code, etc...)
- Accessibilité !

## Outils
- Onglet "Network" du Dev Tools (inspecteur d'éléments)
- Google LightHouse (= la bible de l'optimisation)
- Extension WAVE (analyse l'accessibilité d'un site internet) (Vous avez aussi les normes mondiales (WCAG) et européennes (RGAA) qui sont adaptées des mondiales).
- Outils de calcul d'empreinte environnemental d'un site internet
- EcoIndex : idem ligne du dessus !

## Sources

- `https://www.awwwards.com/`
- `https://ogp.me/`: Open Graph Protocol - permet de préciser des informations sur la page web pour les moteurs de recherche.
- `https://developers.google.com/search/docs/crawling-indexing/special-tags?hl=fr` : balises meta SEO expliquées par Google
- `https://schema.org/docs/full.html` : Microdatas
- `https://developer.chrome.com/docs/lighthouse/overview?hl=fr` : Lighthouse
- `https://wave.webaim.org/extension/` : Wave pluging
- `https://www.websitecarbon.com/` : Website Carbon Calculator
- `https://chromewebstore.google.com/detail/ecoindexfr/apeadjelacokohnkfclnhjlihklpclmp?hl=fr` : EcoIndex




