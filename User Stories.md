# User Stories — Grid Fight Tactics (décomposition minimale)

---

# Lancer une partie tactique

En tant que **joueur**  
je veux **lancer une partie sur une grille**  
afin de **vaincre le Commandant adverse**.

Complexité : 3

---

# Composition d’équipe

## Sélection d'une unité

En tant que **joueur**  
je veux **sélectionner une unité dans le roster**  
afin de **l'ajouter à mon équipe**

Complexité : 1

---

## Désélection d'une unité

En tant que **joueur**  
je veux **retirer une unité sélectionnée**  
afin de **modifier mon équipe**

Complexité : 1

---

## Limitation du nombre d’unités

En tant que **système**  
je veux **limiter l’équipe à 3 unités**  
afin de **respecter les règles du jeu**

Complexité : 1

---

## Validation de la composition

En tant que **joueur**  
je veux **confirmer mon équipe**  
afin de **commencer la phase suivante**

Complexité : 1

---

# Placement initial

## Afficher la grille

En tant que **joueur**  
je veux **voir la grille de jeu**  
afin de **placer mes unités**

Complexité : 1

---

## Afficher la zone de placement

En tant que **joueur**  
je veux **voir ma zone de départ**  
afin de **placer mes unités uniquement dans cette zone**

Complexité : 1

---

## Sélectionner une unité à placer

En tant que **joueur**  
je veux **sélectionner une unité non placée**  
afin de **la positionner sur la grille**

Complexité : 1

---

## Placer une unité sur une case

En tant que **joueur**  
je veux **placer une unité sur une case valide**  
afin de **définir sa position de départ**

Complexité : 1

---

## Déplacer une unité placée

En tant que **joueur**  
je veux **changer la position d'une unité placée**  
afin de **ajuster ma stratégie**

Complexité : 1

---

## Placement automatique du Commandant

En tant que **système**  
je veux **placer automatiquement le Commandant dans un coin**  
afin de **respecter les règles de départ**

Complexité : 1

---

## Alternance de placement

En tant que **système**  
je veux **alterner le placement entre les joueurs**  
afin de **équilibrer la phase de départ**

Complexité : 2

---

# Gestion de l’énergie

## Afficher l’énergie

En tant que **joueur**  
je veux **voir mon énergie disponible**  
afin de **planifier mes actions**

Complexité : 1

---

## Donner l’énergie au début du tour

En tant que **système**  
je veux **donner 10 énergie au début du tour**  
afin de **permettre au joueur d’agir**

Complexité : 1

---

## Consommer de l’énergie

En tant que **système**  
je veux **réduire l’énergie lors d’une action**  
afin de **appliquer le coût des actions**

Complexité : 1

---

## Bloquer une action sans énergie

En tant que **système**  
je veux **empêcher une action si l’énergie est insuffisante**  
afin de **respecter les règles**

Complexité : 1

---

# Phase de préparation

## Sélectionner une unité active

En tant que **joueur attaquant**  
je veux **choisir une unité active**  
afin de **lui assigner une action**

Complexité : 1

---

## Programmer une attaque directionnelle

En tant que **joueur attaquant**  
je veux **choisir une direction d’attaque**  
afin de **définir la zone touchée**

Complexité : 2

---

## Programmer une attaque ciblée

En tant que **joueur attaquant**  
je veux **choisir une case cible**  
afin de **déterminer l’endroit de l’attaque**

Complexité : 2

---

## Programmer une capacité

En tant que **joueur attaquant**  
je veux **activer une capacité d’unité**  
afin de **produire un effet spécial**

Complexité : 2

---

## Verrouiller les actions

En tant que **système**  
je veux **verrouiller les actions programmées**  
afin de **lancer la phase de combat**

Complexité : 1

---

# Phase de combat

## Démarrer le timer de combat

En tant que **système**  
je veux **lancer un timer de 10 secondes**  
afin de **limiter la phase de combat**

Complexité : 1

---

## Exécuter les attaques programmées

En tant que **système**  
je veux **déclencher les attaques programmées**  
afin de **appliquer les actions du joueur attaquant**

Complexité : 2

---

## Appliquer les dégâts

En tant que **système**  
je veux **réduire les PV d'une unité touchée**  
afin de **représenter les dégâts**

Complexité : 1

---

# Déplacement du défenseur

## Sélectionner une unité

En tant que **joueur défenseur**  
je veux **sélectionner une unité**  
afin de **la déplacer**

Complexité : 1

---

## Déplacer une unité

En tant que **joueur défenseur**  
je veux **glisser une unité vers une autre case**  
afin de **changer sa position**

Complexité : 2

---

## Limiter le déplacement

En tant que **système**  
je veux **limiter la distance de déplacement d’une unité**  
afin de **respecter ses statistiques**

Complexité : 2

---

# Mort d’unité

## Réduire les PV

En tant que **système**  
je veux **réduire les points de vie d'une unité**  
afin de **suivre les dégâts**

Complexité : 1

---

## Éliminer une unité

En tant que **système**  
je veux **retirer une unité du plateau lorsque ses PV atteignent 0**  
afin de **représenter sa mort**

Complexité : 1

---

# Résurrection

## Sélectionner une unité morte

En tant que **joueur**  
je veux **choisir une unité éliminée**  
afin de **la ressusciter**

Complexité : 1

---

## Payer le coût de résurrection

En tant que **système**  
je veux **consommer de l’énergie pour la résurrection**  
afin de **appliquer le coût**

Complexité : 1

---

## Faire réapparaître l’unité

En tant que **système**  
je veux **faire apparaître l’unité dans la zone de départ**  
afin de **la remettre en jeu**

Complexité : 2

---

# Victoire

## Réduire les PV du Commandant

En tant que **joueur**  
je veux **attaquer le Commandant ennemi**  
afin de **le vaincre**

Complexité : 1

---

## Déclencher la fin de partie

En tant que **système**  
je veux **terminer la partie lorsque le Commandant meurt**  
afin de **déterminer le vainqueur**

Complexité : 1
