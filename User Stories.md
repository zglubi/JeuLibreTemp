# User Stories — Grid Fight Tactics

## Epic — Jouer une partie tactique en duel

En tant que **joueur**,  
je veux **affronter un adversaire dans un duel tactique sur une grille**,  
afin de **vaincre son Commandant en combinant stratégie et esquive en temps réel**.

---

# 1. Composition d’équipe

## User Story

En tant que **joueur**,  
je veux **choisir 3 unités dans un roster avant la partie**,  
afin de **créer une stratégie et des synergies adaptées à mon style de jeu**.

### Critères d’acceptation

- Le joueur peut sélectionner **exactement 3 unités** dans un roster.
- Chaque unité possède **des capacités et statistiques uniques**.
- La sélection doit être **validée avant le début de la partie**.
- Les deux joueurs composent leur équipe **indépendamment**.

---

# 2. Placement initial des unités

## User Story

En tant que **joueur**,  
je veux **placer mes unités sur la grille avant le début de la partie**,  
afin de **préparer une stratégie de départ et anticiper l’adversaire**.

### Critères d’acceptation

- Les joueurs placent leurs unités **à tour de rôle**.
- Le **Commandant est placé automatiquement dans un coin du plateau**.
- Les zones de placement sont **limitées à la zone de départ du joueur**.
- Une fois toutes les unités placées, **la partie commence**.

---

# 3. Gestion de l’énergie

## User Story

En tant que **joueur**,  
je veux **disposer d’une ressource d’énergie à dépenser chaque tour**,  
afin de **choisir quelles actions effectuer et prioriser mes unités**.

### Critères d’acceptation

- Chaque joueur reçoit **10 points d’énergie au début du tour**.
- L’énergie peut être utilisée pour :
  - activer des **attaques**
  - utiliser des **capacités**
  - **ressusciter une unité**
- Le joueur ne peut **pas dépasser son énergie disponible**.

---

# 4. Phase de préparation (attaquant)

## User Story

En tant que **joueur attaquant**,  
je veux **programmer les actions de mes unités avant le combat**,  
afin de **planifier une stratégie offensive contre l’adversaire**.

### Critères d’acceptation

- Le joueur peut **activer des unités en dépensant de l’énergie**.
- Chaque unité activée peut :
  - attaquer dans une **direction**
  - cibler une **case**
  - utiliser une **capacité spéciale**
- Toutes les actions sont **verrouillées avant la phase de combat**.
- Le défenseur **ne peut pas agir pendant cette phase**.

---

# 5. Phase de combat (défenseur)

## User Story

En tant que **joueur défenseur**,  
je veux **contrôler mes unités en temps réel pendant la phase de combat**,  
afin de **esquiver les attaques et limiter les dégâts**.

### Critères d’acceptation

- La phase de combat dure **10 secondes**.
- Les attaques programmées par l’attaquant **se déclenchent automatiquement**.
- Le défenseur peut **déplacer ses unités sur la grille par drag & drop**.
- Les unités ont une **limite de déplacement basée sur leurs statistiques**.

---

# 6. Alternance des rôles

## User Story

En tant que **joueur**,  
je veux **alterner entre les rôles d’attaquant et de défenseur**,  
afin que **les deux joueurs aient les mêmes opportunités stratégiques**.

### Critères d’acceptation

- À chaque tour, les rôles **attaquant/défenseur s’inversent**.
- Chaque joueur a l’opportunité **d’attaquer et de défendre régulièrement**.

---

# 7. Mort des unités

## User Story

En tant que **joueur**,  
je veux **que les unités puissent être éliminées pendant le combat**,  
afin que **les décisions tactiques aient un impact réel sur la partie**.

### Critères d’acceptation

- Les unités possèdent des **points de vie**.
- Lorsqu’ils atteignent **0**, l’unité est **éliminée du plateau**.

---

# 8. Résurrection d’unités

## User Story

En tant que **joueur**,  
je veux **pouvoir ramener une unité éliminée à la vie**,  
afin de **récupérer une pièce stratégique au prix de l’énergie**.

### Critères d’acceptation

- Une unité morte peut être **ressuscitée en dépensant de l’énergie**.
- L’unité réapparaît **dans la zone de départ du joueur**.
- La résurrection empêche d’utiliser **cette énergie pour d’autres actions**.

---

# 9. Condition de victoire

## User Story

En tant que **joueur**,  
je veux **gagner en éliminant le Commandant adverse**,  
afin que **la partie ait un objectif clair et stratégique**.

### Critères d’acceptation

- Le Commandant possède des **points de vie**.
- Lorsque ses PV atteignent **0**, la partie **se termine immédiatement**.
- Le joueur adverse est **déclaré vainqueur**.

---

# 10. Expérience de duel rapide

## User Story

En tant que **joueur compétitif**,  
je veux **des parties rapides et intenses**,  
afin de **pouvoir enchaîner les matchs et améliorer ma stratégie**.

### Critères d’acceptation

- Une partie dure **quelques minutes**.
- Le rythme alterne **planification stratégique et action rapide**.
- Les règles restent **simples mais offrent une profondeur tactique élevée**.