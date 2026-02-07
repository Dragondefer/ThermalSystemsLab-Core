# Phase 1 — Température et environnement

## 1. Objectif de la phase
Établir une simulation de base où la météo (jours, nuits, saisons) influence la température de l'environnement sur une base de temps modulaire. Cette phase vise à recréer les variations naturelles de température en fonction de l'environnement et du temps.

## 2. Périmètre
### Inclus
- Simulation du temps (jours, nuits, saisons)
- Simulation de la température extérieure en fonction du temps

### Exclu
- Simulation de la météo (pluie, vent, etc.)
- Simulation de l'intérieur des bâtiments

## 3. Hypothèses
- La température extérieure est influencée uniquement par le temps (pas de sources de chaleur ou de refroidissement externes)
- La température évolue de manière plus ou moins prévisible et cyclique
- La simulation du temps est linéaire et contrôlable (pas de sauts temporels ou d'accélérations imprévues)

## 4. Description du système
Vue fonctionnelle du système introduit dans cette phase.
Aucun détail d’implémentation.
- Un module de temps qui simule les jours, nuits et saisons
- Un module de météo qui génère une température extérieure en fonction du temps simulé et des paramètres saisonniers
- Un système de contrôle pour faire avancer le temps de manière régulière et prévisible

## 5. Interfaces
### Entrées
- Temps simulé : unité de temps (secondes, minutes, heures), contrôle de l'avancement du temps
- Paramètres saisonniers : paramètres définissant les caractéristiques de chaque saison (température moyenne, amplitude des variations, etc.)

### Sorties
- Température extérieure : unité de température (°C), valeur évoluant en fonction du temps et des paramètres saisonniers

## 6. Scénarios étudiés
- Simulation d'une journée complète (24 heures) pour observer les variations de température entre le jour et la nuit
- Simulation d'une année complète pour observer les variations de température entre les saisons
- Simulation avec différents paramètres saisonniers pour observer l'impact sur la température extérieure

## 7. Résultats attendus
Comportements attendus, qualitativement et quantitativement.
- La température extérieure doit suivre un cycle jour/nuit avec des variations prévisibleses
- La température extérieure doit suivre un cycle saisonnier avec des variations prévisibles
- Les résultats doivent être reproductibles et paramétrables en fonction des paramètres saisonniers

## 8. Limites connues
Ce que le modèle ne capture pas volontairement.
- Les variations météorologiques imprévues (pluie, vent, etc.)
- Les interactions avec d'autres systèmes (intérieur des bâtiments, sources de chaleur, etc.)

## 9. Pistes d’évolution
Ouvertures pour les phases futures.
- Introduction de la météo (pluie, vent, etc.) et de ses effets sur la température extérieure mais aussi sur les systèmes intérieurs (neige ajoute une couche d'isolation, pluie refroidit l'environnement et accélère le transfert de chaleur avec un effet de refroidissement, etc.)
