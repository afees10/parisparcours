# ParcoursGen • Paris

**Générateur intelligent d'itinéraires à Paris** pour les étudiants de l'ISAE-Supmeca.

Sélectionne les activités de la semaine → l'algorithme construit un parcours **logique** (géographie + temps + transports) sans ping-pong à travers Paris.

## Fonctionnalités clés

- Algorithme de clustering géographique + nearest-neighbor optimisé
- Estimation réaliste des temps de trajet (marche + métro)
- Carte interactive avec le tracé du parcours (Leaflet)
- Plusieurs styles : Équilibré, Compact, Détendu, Culture
- Export texte prêt à copier dans ton planning
- Thème sombre premium ISAE-Supmeca (#0B0F1C + orange #FF5C00)

## Lancer en local

```bash
# Rien à installer
double-clic sur index.html
```

## Déploiement Vercel (recommandé)

1. Importe le dossier `ParcoursGen` sur GitHub
2. Nouveau projet Vercel → Framework "Other"
3. Build & Install commands **vides**
4. Output Directory = `.`
5. Deploy

## Améliorations futures possibles

- Chargement réel des données "Que faire à Paris ?" via Open Data
- Ajout d'activités custom par l'utilisateur
- Export PDF / iCal
- Optimisation plus avancée (algorithme génétique ou OR-Tools)

Projet étudiant — ISAE-Supmeca 2026
