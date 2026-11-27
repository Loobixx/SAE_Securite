# SAE 4A Cybersécurité - Projet Valdoré Services

Bienvenue sur le dépôt du projet de conception et déploiement du système d'information de l'entreprise fictive **Valdoré Services**.

## L'équipe et Répartition des Rôles

*   **Yoann** : Chef de projet et Suivi client (Missions M9 et M1)
    *   Tient à jour le dépôt Git, le tableau de suivi (Kanban/GLPI) et rédige ce fichier README.
    *   Prépare le point d'avancement avec le client lors de chaque séance encadrée.
    *   En charge de l'executive summary en anglais pour la soutenance.
*   **Jules** : Architecte Déploiement et Documentation (Missions M2, M3 et M10)
    *   Coordonne la recherche documentaire et les matrices de choix techniques.
    *   Centralise le plan de déploiement, le versionnage des configurations et la rédaction du cahier de recette.
*   **Anis** : Responsable Sécurité et Audit (Mission M8)
    *   Pilote l'analyse de risques (méthode EBIOS) et lance les audits (Nmap, OpenVAS, PingCastle, Lynis).
    *   Coordonne la correction des vulnérabilités critiques et s'assure que les restaurations de sauvegardes sont fonctionnelles.
*   **Charles** : Analyste Performances et Exploitation (Missions M4, M5, M7)
    *   Définit les métriques, configure la supervision et mène les tests de charge (iperf3).
    *   Analyse les flux avec Wireshark, structure le cahier d'exploitation et trace les interventions.

## Liens Utiles

*   **Dépôt GitHub** : [https://github.com/Loobixx/SAE_Securite](https://github.com/Loobixx/SAE_Securite)
*   **Espace Google Drive** : [Dossier Partagé](https://drive.google.com/drive/folders/1um1-TCe8P5_s9aoBMx7HtW8-D7GZRoB7?usp=sharing)

---

## Suivi de projet

### Séance du 12 Novembre 2026

**Travail réalisé :**
- Lecture du cahier des charges et répartition des rôles/missions.
- Initialisation des outils de collaboration (dépôt Git et dossier partagé Google Drive).

- Point technique avec la DSI pour identifier le matériel disponible pour la maquette.

- Création du fichier de suivi des exigences (Google Sheet) dans le Drive.

- Élaboration d'une première d'architecture réseau pour une futur proposition.

---

### Séance du 26 Novembre 2026

**Travail réalisé :**
* **R1 — Plan d'adressage et découpage VLAN (Équipe) :** Définition des plages IP privées (RFC 1918) et découpage en VLAN (Postes, Serveurs internes, DMZ, Administration) dimensionnés pour au moins 120 équipements.
* **T1 — Matrices de choix techniques (Jules) :** Finalisation des cinq matrices de choix (Mission M3) en respectant la contrainte matérielle de 24 Go de RAM au total.
* **T4 — Référentiels de sécurité (Jules & Anis) :** Recensement des guides ANSSI et benchmarks CIS dans le dossier documentaire (Mission M2).
* **T2 — Documentation d'architecture (Yoann) :** Réalisation du schéma d'architecture logique et définition de l'ordre de déploiement des services (Mission M10).
* **Q5 — Politique de mots de passe & analyse de risques (Anis) :** Rédaction des règles de complexité et de renouvellement selon les recommandations ANSSI, et recensement des biens essentiels et menaces pour la méthode EBIOS (Mission M8).
* **R4 — Pare-feu OPNsense (Yoann / Charles) :** Création de la machine virtuelle OPNsense et amorce de la configuration des quatre interfaces réseau et des zones associées (en cours).
* **S1 — Annuaire Active Directory (Yoann / Charles) :** Début d'installation de la machine virtuelle Windows Server pour l'annuaire (en cours).
* **S5 — Serveurs Linux (Jules / Charles) :** Début d'installation de la première machine virtuelle Debian (en cours).

---

### Séance du 27 Novembre 2026

**Travail réalisé :**
* **Suivi client & point d'avancement (Yoann / Équipe — Mission M9) :** Présentation de l'état d'avancement de l'architecture et des premiers livrables à M. Fenêtre (rôle client).
* **Cohérence documentaire (Équipe — Missions M2, M3, M10) :** Revue croisée et harmonisation de l'ensemble des livrables (schéma d'architecture, plan d'adressage, matrices de choix et dossier documentaire) pour garantir leur cohérence globale.
* **Suivi des exigences (Yoann — Mission M9) :** Mise à jour du tableau de suivi des exigences sur le Google Drive en fonction de l'avancement.
* **R4, S1, S5 — Préparation des machines virtuelles (Équipe) :** Poursuite de l'installation et de la configuration des VM (pare-feu OPNsense, contrôleur de domaine Windows Server et serveurs Debian).
