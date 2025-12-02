Voici les autres sections du fichier `README.md` enrichies avec le contenu fourni :

``` markdown
# Système Intelligent de Gestion des Absences : Cas de l'ENS Marrakech (absENS)

## Résumé du Projet

Ce projet de stage a consisté en la conception et la mise en œuvre d'une solution numérique complète et intelligente, baptisée **absENS**, visant à moderniser et à automatiser la gestion des absences au sein des établissements d'enseignement supérieur, avec l'École Normale Supérieure de Marrakech (ENS Marrakech) comme cas d'étude.

Le système repose sur l'intégration de trois composantes principales : une application web, une application mobile (Android) et un dispositif électronique embarqué basé sur Raspberry Pi, assurant une double vérification de la présence par scan de QR code et vision par ordinateur.

## Contexte

Le projet de stage s'intitule « Conception et mise en œuvre d'un système intelligent de gestion des absences: Cas de l'ENS Marrakech ». Il a été réalisé au sein du Département d'Informatique de l'École Normale Supérieure (ENS) de l'Université Cadi Ayyad. Il s'inscrit dans le cadre d'un stage de perfectionnement académique ayant pour objectif de répondre à la problématique courante dans l'enseignement supérieur qu'est la gestion manuelle des présences, souvent inefficace, sujette à des erreurs et chronophage.

Le département d'informatique de l'ENS Marrakech est l'un des pôles les plus dynamiques de l'établissement. L'environnement de travail a permis de développer une solution technologique intégrant des aspects logiciels (application web et mobile) et matériels (Raspberry Pi, caméras, QR codes). L'encadrement a été assuré par un enseignant-chercheur du département.

## Problématique

La gestion traditionnelle des présences (listes papier ou fichiers Excel) présente de multiples limites, notamment l'absence d'automatisation, le manque d'ergonomie, la difficulté d'accès aux données en temps réel et les faibles performances face à un nombre croissant d'utilisateurs. De plus, les plateformes de gestion existantes sont souvent coûteuses, difficiles à maintenir ou inadaptées aux besoins locaux. Elles manquent également d'intégration matérielle, comme des lecteurs de QR codes connectés ou des systèmes de vérification en salle.

La problématique principale est de concevoir un système plus léger, sécurisé, accessible et personnalisable, permettant de coupler la détection physique des présences avec un traitement logiciel sécurisé. Le système devait être basé sur la lecture d'un code QR unique attribué à chaque étudiant, contenant son identifiant national (CNE).

## Objectifs du Projet

Les objectifs du projet se répartissent sur trois plans :

1.  **Objectifs Fonctionnels**:
    *   Assurer l'enregistrement automatique des présences via un QR code unique par étudiant.
    *   Gérer les utilisateurs selon leurs rôles (étudiant, enseignant, administrateur).
    *   Permettre la consultation des absences par les enseignants et la génération de statistiques par les administrateurs.
    *   Réserver la justification des absences exclusivement aux administrateurs.
    *   Permettre aux étudiants de marquer leur présence uniquement dans une fenêtre temporelle spécifique (entre 15 minutes avant et 5 minutes après le début de la séance).

2.  **Objectifs Techniques**:
    *   Développer une application web basée sur **Laravel** et **Bootstrap**.
    *   Développer une application mobile **Android** destinée à la fois aux enseignants et aux étudiants.
    *   Utiliser un **Raspberry Pi** pour le scan de QR codes à l'entrée.
    *   Utiliser une caméra fixe dans la salle pour la vérification par **vision par ordinateur**.
    *   Stocker les données dans une base de données **MySQL** centralisée.
    *   Garantir une compatibilité multiplateforme (Windows, Linux, macOS).
    *   Viser un temps de réponse inférieur à deux secondes après la lecture du QR code.

3.  **Contraintes**:
    *   Réalisation sur une période de six mois.
    *   Privilégier des solutions **open-source** et du matériel à coût réduit.
    *   Le travail est encadré par un superviseur, avec le respect rigoureux du cahier des charges initial.

## Technologies utilisées

Le projet a mobilisé une diversité de technologies logicielles et matérielles :

### Composante Logicielle
*   **Backend (Application Web & API)**:
    *   **PHP** et **Laravel** (basé sur l'architecture MVC).
    *   Base de données relationnelle **MySQL**.
    *   **API REST** sécurisée par **Laravel Sanctum** pour l'authentification par tokens.
    *   Gestion des rôles et permissions via le package **Spatie Laravel Permission**.
    *   Génération de documents **PDF** pour les rapports via **Laravel DomPDF**.
    *   Génération des **QR Codes** via le package **Laravel QR Code** (simple-qrcode).

*   **Frontend (Interfaces Utilisateur)**:
    *   **Application Web** (Administrateur/Professeur/Étudiant) : Développée en **HTML/CSS/JavaScript** avec le framework **Bootstrap** pour le design responsive.
    *   **Bibliothèques JavaScript** : **FullCalendar** pour l'affichage interactif des emplois du temps et **Chart.js** pour la représentation graphique des statistiques.
    *   **Application Mobile Android** (Professeur/Étudiant) : Développée en **Java**.

### Outils de Développement et Gestion de Projet
*   **IDE Principal** : **Visual Studio Code** (VS Code).
*   **Versionnement** : **GitHub** (via Git) pour la gestion du code source.
*   **Conteneurisation** : **Docker** pour la portabilité et la cohérence de l'environnement de développement.
*   **Modélisation** : **StarUML** pour les diagrammes UML (cas d'utilisation, séquence, classe).
*   **Gestion de projet** : **Notion** (tableaux Kanban et planification).
*   **Déploiement** : Plateforme **Sevalla** pour le déploiement et le test en ligne de l'application.

### Composante Matérielle et Embarquée
*   **Micro-ordinateur** : **Raspberry Pi** (cœur du système embarqué).
*   **Système de Scannage (Entrée de Salle)** : Utilisation d'une caméra connectée au Raspberry Pi pour lire le **QR Code** unique de l'étudiant (contenant son CNE).
*   **Vérification de Présence** : Utilisation d'une caméra murale et de la **vision par ordinateur** via la bibliothèque **OpenCV** en **Python** pour détecter et compter le nombre réel d'étudiants présents.
*   **Prototypage Matériel** : Utilisation de la carte **Arduino Uno** pour les premiers tests.
*   **Périphériques embarqués** : Capteur de proximité, flash LED puissant, ventilateur et LED RGB pour le feedback visuel.

```
