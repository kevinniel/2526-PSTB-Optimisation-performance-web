# TP — Audit d’optimisation de la performance web

## Durée

2 jours

## Travail attendu

Vous devez réaliser l’audit complet d’un site web de votre choix.

Le site peut être :

* un site vitrine
* un site e-commerce
* un blog
* un site institutionnel
* une application web publique

Le site choisi doit contenir au minimum :

* plusieurs pages
* des images
* du CSS
* du JavaScript
* un contenu visible exploitable

---

# Objectif du TP

L’objectif est d’analyser les performances d’un site web existant, d’identifier ses problèmes principaux et de proposer des optimisations concrètes.

Vous devez être capables de :

* mesurer les performances d’un site
* comprendre les causes des lenteurs
* analyser les fichiers chargés par la page
* repérer les problèmes SEO de base
* repérer les problèmes d’accessibilité
* évaluer l’impact environnemental
* proposer des corrections priorisées

---

# Outils à utiliser

Vous devez utiliser au minimum :

* DevTools — onglet Network
* Lighthouse
* WAVE
* Website Carbon Calculator ou EcoIndex
* Analyse manuelle du code rendu dans la page
* Analyse des balises SEO
* Analyse des images et fichiers chargés

Vous pouvez utiliser d’autres outils si vous les jugez utiles.

---


## 1. Choix du site

Choisissez un site web à auditer.

Indiquez dans votre rapport :

* nom du site
* URL
* type de site
* objectif supposé du site
* public cible supposé
* raison du choix

---

## 2. Audit Lighthouse

Lancez un audit Lighthouse sur la page d’accueil.

Vous devez relever :

* score Performance
* score Accessibilité
* score Bonnes pratiques
* score SEO
* Core Web Vitals disponibles
* principaux problèmes détectés
* captures d’écran des résultats

Vous devez expliquer les problèmes importants avec vos mots.

---

## 3. Analyse Network

Avec l’onglet Network des DevTools, analysez le chargement de la page.

Vous devez relever :

* nombre total de requêtes
* poids total chargé
* temps de chargement principal
* fichiers les plus lourds
* images les plus lourdes
* fichiers JavaScript importants
* fichiers CSS importants
* requêtes inutiles ou suspectes
* éventuels appels externes

Vous devez produire un tableau de synthèse.

Exemple :

| Élément        | Observation | Impact          | Correction possible   |
| -------------- | ----------- | --------------- | --------------------- |
| Image hero     | 2,4 Mo      | Chargement lent | Compresser / WebP     |
| script.js      | 800 Ko      | JS lourd        | Minifier / découper   |
| police externe | 4 requêtes  | Latence         | Réduire les variantes |

---

## 4. Analyse du rendu et du code

Analysez la page affichée et le code HTML rendu.

Vous devez vérifier :

* structure HTML
* présence d’un seul `<h1>`
* cohérence des titres `<h2>`, `<h3>`
* présence de balises inutiles ou excessives
* quantité de code HTML
* chargement du JavaScript
* présence de `async` ou `defer`
* éventuels scripts bloquants
* présence de CSS inutilisé ou très lourd

---

## 5. Analyse SEO

Analysez les éléments SEO de base.

Vous devez vérifier :

* balise `<title>`
* meta description
* balises Open Graph
* structure des titres
* textes alternatifs sur les images
* URL lisibles
* présence éventuelle de données structurées / schema.org
* cohérence globale du contenu

Vous devez indiquer ce qui est correct et ce qui doit être amélioré.

---

## 6. Analyse accessibilité

Avec WAVE et une analyse manuelle, vérifiez :

* contrastes
* textes alternatifs
* labels de formulaires
* structure des titres
* navigation clavier si possible
* erreurs détectées par WAVE
* alertes importantes
* éléments non accessibles

Vous devez expliquer les problèmes principaux.

---

## 7. Analyse environnementale

Utilisez Website Carbon Calculator ou EcoIndex.

Vous devez relever :

* résultat obtenu
* poids de la page
* estimation d’impact environnemental si disponible
* causes probables d’un mauvais score
* optimisations possibles

---

# Jour 2 — Synthèse, recommandations et restitution

## 8. Synthèse des problèmes

Regroupez les problèmes identifiés par catégorie :

* Performance
* Images
* JavaScript
* CSS
* Serveur / hébergement
* SEO
* Accessibilité
* Impact environnemental
* UX/UI

Pour chaque problème, indiquez :

* description du problème
* preuve ou capture
* impact
* niveau de priorité
* correction proposée

Priorités à utiliser :

* Critique
* Important
* Moyen
* Faible

---

## 9. Plan d’optimisation

Vous devez proposer un plan d’action concret.

Votre plan doit contenir au minimum 10 recommandations.

Pour chaque recommandation, indiquez :

| Priorité | Problème | Correction | Impact attendu | Difficulté |
| -------- | -------- | ---------- | -------------- | ---------- |

Exemple :

| Priorité  | Problème            | Correction                          | Impact attendu         | Difficulté |
| --------- | ------------------- | ----------------------------------- | ---------------------- | ---------- |
| Critique  | Images trop lourdes | Convertir en WebP et redimensionner | Chargement plus rapide | Facile     |
| Important | JS bloquant         | Ajouter defer sur certains scripts  | Meilleur rendu initial | Moyen      |

---

## 10. Avant / après théorique

Vous ne modifiez pas forcément le site.

Mais vous devez estimer ce qui pourrait être amélioré après correction :

* score Performance actuel
* score Performance visé
* poids actuel de la page
* poids visé
* nombre actuel de requêtes
* nombre visé
* principaux gains attendus

Les estimations doivent être réalistes et justifiées.

---

# Livrables attendus

Vous devez rendre :

## 1. Rapport d’audit au format PDF

Le rapport doit contenir :

* présentation du site audité
* captures des outils utilisés
* résultats Lighthouse
* analyse Network
* analyse SEO
* analyse accessibilité
* analyse environnementale
* synthèse des problèmes
* plan d’optimisation priorisé
* conclusion claire

# Contraintes

Votre rapport doit être clair, structuré et professionnel.

Vous devez éviter :

* les captures sans explication
* les copier-coller bruts de Lighthouse
* les recommandations vagues
* les phrases du type “il faut optimiser le site” sans précision
* les analyses non justifiées

Chaque problème important doit être accompagné d’une preuve ou d’une observation précise.

---

# Barème d’évaluation — 20 points

## 1. Choix et présentation du site — 2 points

| Critère                                 | Points |
| --------------------------------------- | -----: |
| Site pertinent et exploitable           |      1 |
| Présentation claire du contexte du site |      1 |

---

## 2. Audit Lighthouse — 3 points

| Critère                                     | Points |
| ------------------------------------------- | -----: |
| Scores correctement relevés                 |      1 |
| Problèmes principaux identifiés             |      1 |
| Explications compréhensibles et pertinentes |      1 |

---

## 3. Analyse Network — 3 points

| Critère                                           | Points |
| ------------------------------------------------- | -----: |
| Nombre de requêtes, poids et temps relevés        |      1 |
| Fichiers lourds ou problématiques identifiés      |      1 |
| Analyse correcte de l’impact sur les performances |      1 |

---

## 4. Analyse SEO — 2 points

| Critère                              | Points |
| ------------------------------------ | -----: |
| Vérification des balises principales |      1 |
| Recommandations SEO pertinentes      |      1 |

---

## 5. Analyse accessibilité — 2 points

| Critère                                          | Points |
| ------------------------------------------------ | -----: |
| Utilisation correcte de WAVE ou outil équivalent |      1 |
| Problèmes d’accessibilité expliqués              |      1 |

---

## 6. Analyse environnementale — 1,5 point

| Critère                                   | Points |
| ----------------------------------------- | -----: |
| Mesure réalisée avec un outil adapté      |    0,5 |
| Résultat expliqué                         |    0,5 |
| Optimisations environnementales proposées |    0,5 |

---

## 7. Plan d’optimisation — 3 points

| Critère                      | Points |
| ---------------------------- | -----: |
| Recommandations concrètes    |      1 |
| Priorisation claire          |      1 |
| Impact et difficulté estimés |      1 |

---

## 8. Qualité du rapport — 2 points

| Critère                                     | Points |
| ------------------------------------------- | -----: |
| Rapport structuré et lisible                |      1 |
| Captures, tableaux et preuves bien intégrés |      1 |

---

# Bonus — jusqu’à +2 points

Des points bonus peuvent être accordés si vous réalisez :

* un mini avant/après sur une copie locale d’une page
* une analyse mobile et desktop séparée
* une analyse de plusieurs pages du même site
* une estimation chiffrée des gains possibles
* une recommandation technique avancée : cache, CDN, lazy loading, SSR, compression Brotli/Gzip, optimisation serveur

---

# Rendu attendu

À rendre :

* rapport PDF
* éventuellement fichiers complémentaires

Nom des fichiers :

`NOM_Prenom_Audit_Performance_Web.pdf`

A envoyer par mail à `k.niel.pro@gmail.com` avant lundi 15 Juin 2026 à 17h45 (heure de réception du mail !) avec en objet de mail : "PSTB_NOM_Prenom_TP_DevWeb"

---

# Conseil final

Votre objectif n’est pas seulement de dire que le site est lent.

Votre objectif est de prouver pourquoi il est lent, d’expliquer l’impact, puis de proposer les corrections les plus efficaces en priorité.
