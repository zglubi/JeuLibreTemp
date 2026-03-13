Game Design Document — Grid Fight Tactics

1. Présentation générale
1.1 Pitch

Grid Fight Tactics est un jeu de stratégie tactique compétitive en 1v1, combinant planification au tour par tour et action en temps réel.
Chaque joueur contrôle un Commandant et trois unités spécialisées sur une grille.
L’objectif : éliminer le Commandant adverse.

Le jeu repose sur une alternance entre :

    Phase de préparation : programmation d’actions offensives.

    Phase de combat : exécution automatique des attaques + déplacements en temps réel du défenseur.

Le résultat est un duel nerveux, lisible, stratégique et riche en mind games.

2. Gameplay Core

2.1 Objectif

Vaincre le Commandant ennemi en réduisant ses PV à 0.

2.2 Conditions de victoire / défaite

    Victoire : le Commandant adverse meurt.

    Défaite : votre Commandant meurt.

    Les unités ordinaires peuvent mourir et être ressuscitées.

3. Plateau de jeu

3.1 Vue et structure

    Grille vue du dessus en 3D tactique.

    Deux zones de départ opposées en diagonale.

    Cases permettant :

        déplacements

        attaques directionnelles

        ciblage précis

3.2 Placement initial

    Chaque joueur place ses 3 unités dans sa zone.

    Placement alterné pour créer du mind game dès le début.

4. Unités

4.1 Composition d’équipe

Avant la partie :

    Choisir 3 unités dans un roster.

    Chaque unité possède :

        statistiques (PV, vitesse, portée…)

        attaques directionnelles

        attaques ciblées

        capacités spéciales

4.2 Commandant

    Unité centrale.

    Faible mobilité mais capacités puissantes.

    Sa mort = fin de partie.

4.3 Mort et résurrection

    Une unité morte peut être ramenée à la vie en dépensant de l’énergie.

    Le joueur choisit où la faire réapparaître (dans une zone définie).

5. Ressource : Énergie

5.1 Fonctionnement

    Chaque tour : 10 points d’énergie.

    Dépenses possibles :

        activer une unité

        lancer une attaque

        utiliser une capacité

        ressusciter une unité

5.2 Philosophie

L’énergie impose des choix tactiques :

    attaquer plus fort ?

    ressusciter une unité clé ?

    économiser pour un tour explosif ?

6. Structure d’un tour

6.1 Alternance des rôles

Chaque tour alterne :

    un attaquant

    un défenseur

6.2 Phase 1 — Préparation (Attaquant)

L’attaquant :

    choisit quelles unités activer

    dépense son énergie

    programme des actions :

        attaque directionnelle

        attaque ciblée

        capacité spéciale

Le défenseur est passif durant cette phase.

6.3 Phase 2 — Combat (10 secondes)

    Les actions programmées se déclenchent automatiquement.

    Attaques avec startup, durée, cooldown.

    Certaines attaques peuvent persister ou se répéter.

Pendant ce temps, le défenseur :

    déplace ses unités en temps réel (drag & drop)

    esquive

    se repositionne

    respecte une limite de déplacement par unité

7. Ce qui rend le jeu unique

7.1 Hybridation stratégique

    Planification façon échecs / tactique.

    Exécution façon action / esquive.

7.2 Mind games

    L’attaquant doit anticiper les mouvements du défenseur.

    Le défenseur doit lire les intentions de l’attaquant.

7.3 Accessibilité

    Règles simples.

    Profondeur émergente.

7.4 Format compétitif

    Parties rapides.

    Idéal pour le PvP en ligne.

8. User Stories

8.1 Lancer une partie

    Lancer une partie sur une grille pour vaincre le Commandant adverse.
    Complexité : 3

10. User Stories — Composition d’équipe

    Sélectionner une unité dans le roster. (1)

    Retirer une unité sélectionnée. (1)

    Confirmer une équipe de 3 unités. (1)

11. User Stories — Placement initial

    Voir la grille. (1)

    Voir la zone de placement. (1)

    Sélectionner une unité non placée. (1)

    Placer une unité sur une case valide. (1)

    Modifier le placement. (1)

12. User Stories — Gestion de l’énergie

    Voir l’énergie disponible. (1)

    Dépenser de l’énergie pour activer des actions. (1)

13. User Stories — Phase de préparation

    Sélectionner une unité active. (1)

    Programmer une attaque directionnelle. (2)

    Programmer une attaque ciblée. (2)

    Utiliser une capacité. (2)

    Confirmer les actions. (1)

14. User Stories — Phase de combat

    Voir les attaques se déclencher. (2)

15. User Stories — Déplacement en défense

    Sélectionner une unité. (1)

    Déplacer une unité. (2)

    Repositionner plusieurs unités. (2)

16. User Stories — Mort et résurrection

    Voir les PV diminuer. (1)

    Voir une unité mourir. (1)

    Choisir une unité morte. (1)

    Ressusciter une unité. (2)

17. User Stories — Victoire

    Attaquer le Commandant. (1)

    Gagner la partie lorsque le Commandant meurt. (1)

18. Vision long terme

    Développer un jeu compétitif moderne, lisible et profond.

    Mélanger réflexion, anticipation, exécution, lecture de l’adversaire.

    Proposer un format idéal pour :

        l’e-sport

        les duels rapides

        les joueurs tactiques cherchant un gameplay innovant

19. Sprint Planning (3 semaines)

Ce planning vise à livrer une boucle de gameplay complète en trois sprints courts et ciblés. Chaque sprint produit un livrable jouable, permettant d’itérer rapidement.
Sprint 1 — Setup de la partie & Placement

Durée : 1 semaine
Objectif : permettre au joueur de lancer une partie et de placer ses unités.
Contenu du sprint
User Stories incluses

    Lancer une partie (3)

    Sélectionner une unité (1)

    Retirer une unité (1)

    Confirmer mon équipe (1)

    Voir la grille (1)

    Voir ma zone de placement (1)

    Sélectionner une unité à placer (1)

    Placer une unité (1)

    Modifier le placement (1)

Total complexité: 11 points

Livrable:

À la fin du sprint, le joueur peut :

    lancer une partie

    composer une équipe de 3 unités

    visualiser la grille

    placer ses unités dans sa zone de départ

Le setup complet de la bataille est fonctionnel.

Sprint 2 — Programmation des actions

Durée : 1 semaine

Objectif : permettre au joueur d’utiliser l’énergie et de programmer ses actions offensives.

Contenu du sprint:

User Stories incluses

    Voir mon énergie (1)

    Dépenser de l’énergie (1)

    Sélectionner une unité active (1)

    Programmer une attaque directionnelle (2)

    Programmer une attaque ciblée (2)

    Utiliser une capacité (2)

    Confirmer mes actions (1)

Total complexité: 10 points

Livrable:

À la fin du sprint, le joueur peut :

    gérer son énergie

    sélectionner des unités actives

    programmer des attaques directionnelles, ciblées ou des capacités

    valider ses actions

Les actions sont prêtes à être exécutées dans la phase suivante.

Sprint 3 — Combat & Fin de partie

Durée : 1 semaine

Objectif : exécuter les actions, gérer les déplacements défensifs, les dégâts et la victoire.

Contenu du sprint

User Stories incluses

    Voir les attaques se déclencher (2)

    Sélectionner une unité en défense (1)

    Déplacer une unité (2)

    Repositionner plusieurs unités (2)

    Voir une unité subir des dégâts (1)

    Voir une unité mourir (1)

    Choisir une unité morte (1)

    Ressusciter une unité (2)

    Attaquer le Commandant (1)

    Gagner la partie (1)

Total complexité: 14 points

Livrable:

À la fin du sprint, le jeu permet :

    l’exécution automatique des attaques

    les déplacements défensifs en temps réel

    la gestion des dégâts et de la mort

    la résurrection d’unités

    la victoire lorsque le Commandant ennemi meurt

La boucle de gameplay complète est jouable.

Résumé des sprints:

Sprint 1: Setup + placement (11)

Sprint 2: Programmation des actions (10)

Sprint 3: Combat + victoire (14)

État final après 3 semaines

Un prototype jouable incluant la boucle complète :

Composition d’équipe → Placement → Programmation → Combat → Victoire


