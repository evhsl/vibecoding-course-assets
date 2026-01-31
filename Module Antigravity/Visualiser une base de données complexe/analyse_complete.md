# Visualisation d'une base de données complexe avec Antigravity

Ce document retrace le processus de création d'une application d'exploration de données (HATVP) étape par étape, illustré par les captures d'écran du module.

### Phase 1 : Découverte et Analyse des Données

![Module Antigravity 1](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%201.png)
**Module Antigravity 1 : Initialisation**
Ouverture de l'environnement Antigravity sur le dossier "Données HATVP".

![Module Antigravity 2](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%202.png)
**Module Antigravity 2 : Prompt Initial**
Vous demandez à l'agent d'analyser la structure de toutes les données du dossier.

![Module Antigravity 3](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%203.png)
**Module Antigravity 3 : Planification**
L'agent génère une liste de tâches (Task List) pour structurer son analyse.

![Module Antigravity 4](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%204.png)
**Module Antigravity 4 : Réflexion**
L'agent analyse le contexte ("Thinking") pour orienter ses prochaines actions.

![Module Antigravity 5](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%205.png)
**Module Antigravity 5 : Scripting**
Création du script Python `analyze_json.py` pour explorer le contenu des fichiers.

![Module Antigravity 6](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%206.png)
**Module Antigravity 6 : Compte-rendu**
L'agent résume sa découverte : un gros fichier JSON riche et des CSV relationnels plus légers.

![Module Antigravity 7](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%207.png)
**Module Antigravity 7 : Rapport (Début)**
Consultation du `Analysis Report.md` qui détaille la structure identifiée.

![Module Antigravity 8](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%208.png)
**Module Antigravity 8 : Rapport (Pistes)**
Focus sur le potentiel d'analyse identifié dans le rapport (cartographie des lobbies, réseaux).

### Phase 2 : Consolidation et Traitement des Données

![Module Antigravity 9](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%209.png)
**Module Antigravity 9 : Demande de Consolidation**
Vous demandez une jointure des tables pour faciliter l'analyse.

![Module Antigravity 10](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2010.png)
**Module Antigravity 10 : Plan Technique**
L'agent propose un plan pour créer un fichier unifié `hatvp_consolidated.csv`.

![Module Antigravity 11](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2011.png)
**Module Antigravity 11 : Lancement**
Vous validez le lancement du script de consolidation.

![Module Antigravity 12](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2012.png)
**Module Antigravity 12 : Debugging**
L'agent rencontre des erreurs d'alignement (headers) dans les fichiers CSV sources.

![Module Antigravity 13](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2013.png)
**Module Antigravity 13 : Pivot Stratégique**
L'agent décide d'abandonner les CSV pour extraire les données proprement depuis le fichier JSON maître.

![Module Antigravity 14](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2014.png)
**Module Antigravity 14 : Succès**
La consolidation est terminée, un fichier propre de 93k lignes est généré.

### Phase 3 : Développement de l'Application Web

![Module Antigravity 15](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2015.png)
**Module Antigravity 15 : Proposition App**
L'agent suggère de créer une interface web interactive pour explorer ces données.

![Module Antigravity 16](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2016.png)
**Module Antigravity 16 : Plan d'Implémentation App**
Détails techniques validés : Backend Flask + Frontend React/Vite.

![Module Antigravity 17](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2017.png)
**Module Antigravity 17 : Installation**
L'agent installe les dépendances et prépare la base de données SQLite.

![Module Antigravity 18](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2018.png)
**Module Antigravity 18 : Documentation**
Création du `Walkthrough.md` (Guide d'utilisation) et du script de lancement rapide.

![Module Antigravity 19](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2019.png)
**Module Antigravity 19 : Démarrage**
L'agent lance les serveurs via le terminal.

![Module Antigravity 20](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2020.png)
**Module Antigravity 20 : Confirmation**
Interaction où l'agent confirme que l'appli tourne ou attend votre feu vert.

![Module Antigravity 21](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2021.png)
**Module Antigravity 21 : App en cours**
Terminaux montrant le Backend (port 5000) et le Frontend (port 5173) actifs.

### Phase 4 : Exploration de l'Application (HATVP Explorer)

![Module Antigravity 22](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2022.png)
**Module Antigravity 22 : Vue Liste**
Découverte de l'interface "Représentants" avec le tableau des données.

![Module Antigravity 23](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2023.png)
**Module Antigravity 23 : Navigation**
Exploration de la liste (similaire à la 22).

![Module Antigravity 24](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2024.png)
**Module Antigravity 24 : Vue Statistiques**
Visualisation des graphiques (Top Secteurs d'activités, Top Organisations).

![Module Antigravity 25](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2025.png)
**Module Antigravity 25 : Vue Réseau**
Visualisation interactive des liens sous forme de graphe (noeuds et connexions).

![Module Antigravity 26](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2026.png)
**Module Antigravity 26 : Vue Détail**
Ouverture d'une fiche entreprise (exemple : BINANCE FRANCE SAS) dans une modale.

### Phase 5 : Itération et Amélioration

![Module Antigravity 27](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2027.png)
**Module Antigravity 27 : Feedback**
Retour dans VS Code, l'agent demande quelles données supplémentaires vous souhaitez voir.

![Module Antigravity 28](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2028.png)
**Module Antigravity 28 : Suggestions**
L'agent propose d'ajouter les données financières et les niveaux d'intervention.

![Module Antigravity 29](https://raw.githubusercontent.com/evhsl/vibecoding-course-assets/refs/heads/main/Module%20Antigravity/Visualiser%20une%20base%20de%20donn%C3%A9es%20complexe/Module%20Antigravity%2029.png)
**Module Antigravity 29 : Validation Finale**
Vous donnez l'instruction : "Intègre tout".
