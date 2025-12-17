# Système Intelligent de Gestion des Absences : Cas de l'ENS Marrakech (absENS)

<p align="center">
  <img src="/web/gestion-abs/images/emsi1.png" alt="Logo emsi" width="180">
</p>

## 📌 Résumé du Projet

Ce projet de stage a consisté en la conception et la mise en œuvre d'une solution numérique intelligente, nommée **absENS**, destinée à automatiser la gestion des absences au sein de l’ENS Marrakech.  
Le système regroupe une application web, une application mobile Android et un dispositif embarqué Raspberry Pi.

---

## 🏫 Contexte

Le projet a été réalisé au sein du Département d’Informatique de l’ENS Marrakech, dans le cadre d’un stage académique visant à moderniser la gestion traditionnelle des présences (papier, Excel).

---

## ❗ Problématique

Les méthodes actuelles sont :

- Non automatisées  
- Sujettes aux erreurs  
- Non accessibles en temps réel  
- Difficiles à maintenir

👉 Objectif : créer une **solution sécurisée, rapide, intelligente**, basée sur QR Codes + Vision par ordinateur.

---

## 🎯 Objectifs du Projet

### ✔️ Objectifs Fonctionnels
- Lecture de QR code unique
- Gestion par rôles (Étudiant, Enseignant, Admin)
- Consultation des absences & statistiques
- Justification par l'administration
- Fenêtre temporelle d’accès : *15 min avant → 5 min après*

### ✔️ Objectifs Techniques
- Laravel, MySQL, API REST (Sanctum)
- Android (Java)
- Raspberry Pi + caméra
- Vision par ordinateur avec OpenCV
- Temps de réponse < 2 secondes

---

## 🛠️ Technologies Utilisées

### Backend
- PHP / Laravel  
- MySQL  
- API REST (Sanctum)  
- DomPDF, Simple-Qrcode  
- Spatie Laravel Permission

### Frontend
- HTML/CSS/JS  
- Bootstrap  
- FullCalendar  
- Chart.js  
- Android (Java)

### Outils
- VS Code  
- GitHub  
- Docker  
- StarUML  
- Notion  
- Déploiement : Sevalla

---

# 🖼️ Diagrammes UML

## 🎭 Diagramme de Cas d'Utilisation (Use Case)

<p align="center">
  <img src="/web/gestion-abs/images/usecase1.png" alt="Diagramme de cas d'utilisation absENS" width="700">
  <img src="/web/gestion-abs/images/usecase2.png" alt="Diagramme de cas d'utilisation absENS" width="700">
</p>

---

## 🧩 Diagramme de Classes

<p align="center">
  <img src="/web/gestion-abs/images/calss.png" alt="Diagramme de classes absENS" width="800">
</p>

---

# 🧱 Architecture Globale du Système

<p align="center">
  <img src="/web/gestion-abs/images/image.jpg" alt="Architecture générale du système absENS" width="900">
</p>

---

# 🔌 Composante Matérielle

<p align="center">
  <img src="/web/gestion-abs/images/schema.png" alt="Module Raspberry Pi absENS" width="550">
  <img src="/web/gestion-abs/images/sh6.jpg" alt="Raspberry Pi absENS" width="550">
  <img src="/web/gestion-abs/images/systemesAbs.jpeg" alt="Module Raspberry Pi absENS" width="550">
</p>

---
# Des Captures d’Écran
<p align="center"> Captures d’Écran de l'Authontification</p>

<p align="center">
  <img src="/web/gestion-abs/images/auth.jpg" alt="" width="550">
  <img src="/web/gestion-abs/images/au3.png" alt="" width="550">
</p>

<p align="center"> Captures d’Écran de l'espace administration</p>

<p align="center">
  <img src="/web/gestion-abs/images/a1.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a18.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a20.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a22.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a6.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a14.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a12aaa.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a26.png" alt="" width="550">
  <img src="/web/gestion-abs/images/a35.png" alt="" width="550">
</p>

<p align="center"> Captures d’Écran de l'espace l'étudiant</p>

<p align="center">
  <img src="/web/gestion-abs/images/e1.png" alt="" width="550">
  <img src="/web/gestion-abs/images/e4.png" alt="" width="550">
  <img src="/web/gestion-abs/images/emailAbs.png" alt="" width="550">
  <img src="/web/gestion-abs/images/e5.png" alt="" width="550">
  <img src="/web/gestion-abs/images/e6.png" alt="" width="550">
</p>

---

# 📷 Fonctionnement Global du Système

1. L’étudiant scanne son QR code → Raspberry Pi envoie la présence à l’API.  
2. La caméra de salle analyse les présences réelles via OpenCV.  
3. L’enseignant valide la séance via web/mobile.  
4. L’administration consulte les statistiques globales.

---


## 👨‍🏫 Références académiques

- **Réalisé par** : AIT ICHOU Rafik  
- **Encadré par** : Pr. NAIT MALEK Youssef - ENS Marrakech
- **Établissements** : ENS

---

## 📬 Contact

Pour toute question, vous pouvez me contacter :

**Email** : rafikaitichou@gmail.com  

---

##

Projet réalisé dans le cadre d’un stage au  
**Département d’Informatique – ENS Marrakech**.
<p align="center">
  <img src="/web/gestion-abs/images/ens.png" alt="Logo ENS Marrakech" width="180">
</p>

---

