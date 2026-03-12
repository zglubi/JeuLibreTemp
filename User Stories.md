# User Stories — Grid Fight Tactics

## Duel tactique sur grille

**Complexité : 3**

En tant que **joueur**,  
je veux **jouer un duel tactique sur une grille**,  
afin de **détruire le Commandant adverse**.

### Actions principales

- sélectionner une équipe
- placer mes unités
- planifier mes attaques
- déplacer mes unités pour esquiver
- gérer mon énergie
- éliminer les unités ennemies
- cibler le Commandant adverse

---

# 1. Composition d’équipe

**Complexité : 1**

## User Story

En tant que **joueur**,  
je veux **sélectionner 3 unités dans un roster**.

### Actions

- ouvrir l’écran de sélection
- parcourir la liste des unités
- sélectionner une unité
- désélectionner une unité
- confirmer la composition

### Règles

- maximum **3 unités**
- minimum **3 unités**
- chaque unité possède :
  - statistiques
  - capacités

---

# 2. Placement initial

**Complexité : 2**

## User Story

En tant que **joueur**,  
je veux **placer mes unités sur la grille** avant le début du combat.

### Actions

- sélectionner une unité
- choisir une case dans la zone de départ
- placer l’unité sur la case
- déplacer une unité déjà placée
- confirmer le placement

### Règles

- placement **alterné entre joueurs**
- placement limité à **la zone de départ**
- le **Commandant est placé automatiquement**

---

# 3. Gestion de l’énergie

**Complexité : 1**

## User Story

En tant que **joueur**,  
je veux **dépenser de l’énergie pour mes actions**.

### Actions

- consulter mon énergie
- activer une unité
- utiliser une capacité
- lancer une attaque
- ressusciter une unité

### Règles

- **10 énergie par tour**
- impossible de dépasser l’énergie disponible

---

# 4. Phase de préparation (attaquant)

**Complexité : 2**

## User Story

En tant que **joueur attaquant**,  
je veux **programmer les actions de mes unités**.

### Actions

- sélectionner une unité
- activer l’unité (coût énergie)
- choisir une action
- définir une direction d’attaque
- cibler une case
- utiliser une capacité
- confirmer les actions

### Règles

- actions **verrouillées avant combat**
- défenseur **ne peut pas agir**

---

# 5. Phase de combat (défenseur)

**Complexité : 3**

## User Story

En tant que **joueur défenseur**,  
je veux **déplacer mes unités pendant le combat** pour esquiver.

### Actions

- sélectionner une unité
- drag l’unité sur la grille
- déplacer l’unité vers une case
- repositionner plusieurs unités
- éviter les zones d’attaque

### Règles

- durée **10 secondes**
- attaques **automatiques**
- déplacement limité par :
  - vitesse
  - distance maximale

---

# 6. Alternance des rôles

**Complexité : 1**

## User Story

En tant que **joueur**,  
je veux **alterner attaquant et défenseur**.

### Actions

- jouer un tour en attaque
- jouer un tour en défense

### Règles

- inversion des rôles à chaque tour

---

# 7. Mort des unités

**Complexité : 1**

## User Story

En tant que **joueur**,  
je veux **que les unités puissent mourir**.

### Actions

- subir des dégâts
- atteindre 0 PV
- retirer l’unité du plateau

### Règles

- une unité morte **ne peut plus agir**

---

# 8. Résurrection

**Complexité : 2**

## User Story

En tant que **joueur**,  
je veux **ressusciter une unité éliminée**.

### Actions

- ouvrir la liste des unités mortes
- sélectionner une unité
- payer le coût en énergie
- faire apparaître l’unité

### Règles

- apparition dans **zone de départ**
- coût en énergie obligatoire

---

# 9. Condition de victoire

**Complexité : 1**

## User Story

En tant que **joueur**,  
je veux **gagner en détruisant le Commandant ennemi**.

### Actions

- attaquer le Commandant
- réduire ses PV à 0

### Résultat

- fin immédiate de la partie
- victoire du joueur

---

# 10. Expérience de duel rapide

**Complexité : 2**

## User Story

En tant que **joueur compétitif**,  
je veux **des parties rapides et lisibles**.

### Objectifs

- parties de **quelques minutes**
- alternance :
  - stratégie
  - action
- règles simples
- profondeur tactique
