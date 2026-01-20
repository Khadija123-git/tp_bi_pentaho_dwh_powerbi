# TP – Pipeline OLTP → ETL Pentaho PDI → Data Warehouse → Reporting Power BI

## Objectif du TP

Construire un pipeline complet de Business Intelligence permettant de :
- Extraire les données d’une base OLTP (MySQL)
- Les transformer/nettoyer avec Pentaho PDI (Kettle)
- Les charger dans un Data Warehouse (schéma étoile, MySQL)
- Réaliser des analyses et tableaux de bord dynamiques dans Power BI

## Technologies utilisées

- MySQL (base OLTP et Data Warehouse)
- Pentaho Data Integration (PDI, aka Kettle)
- Power BI (reporting et visualisation)
- SQL (requêtes analytiques)
- CSV (exemples de données pour tests)

## Organisation du dépôt

- `/data_oltp/` : Exemples de jeux de données brutes OLTP (CSV)
- `/ktr/` : Transformations ETL Pentaho (.ktr)
- `/kjb/` : Jobs ETL (.kjb)
- `/schema/` : Diagrammes et schémas d’architecture, captures d’écran (images)
- `/sql/` : Scripts SQL (création du Data Warehouse, requêtes OLAP)
- `/powerbi/` : Fichier Power BI et captures des dashboards
- `/rapport.pdf` : Rapport détaillant toutes les étapes, résultats et difficultés

## Instructions pour exécuter

1. **Préparer la base OLTP**  
   - Créer les tables OLTP (clients, produits, commandes, lignes_commandes) dans MySQL
   - Importer les fichiers CSV (dans `/data_oltp/`) si besoin

2. **Lancer Pentaho PDI**  
   - Ouvrir les fichiers `.ktr` et `.kjb` dans `/ktr/` et `/kjb/`
   - Suivre l’ordre d’exécution défini dans `/kjb/orchestration.kjb`
   - S’assurer que les données sont bien chargées dans le Data Warehouse (`ventes_dwh`)
   - Valider avec les scripts SQL présents dans `/sql/`

3. **Reporting Power BI**  
   - Ouvrir le fichier `/powerbi/dashboard.pbix` dans Power BI Desktop
   - Se connecter sur la base DWH MySQL si besoin (ou utiliser les screenshots)
   - Explorer les tableaux de bord interactifs, vérifier les réponses aux questions analytiques

4. **Se référer au rapport pour toute explication détaillée, issues connues, ou dépannage.**

## Membres du groupe
- Khadija Nachid Idrissi
- Rajae Fdili
- Aya Hamim
  

