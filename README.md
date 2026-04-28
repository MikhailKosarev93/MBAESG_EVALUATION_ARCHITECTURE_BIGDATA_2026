# Workshop – Data-Driven Marketing Analytics avec Snowflake et Streamlit

## Contexte
Ce projet a été réalisé dans le cadre du workshop Food & Beverage.  
Il vise à construire un pipeline analytique dans Snowflake à partir de plusieurs domaines de données : ventes, promotions, campagnes marketing, inventaire, avis produits, fournisseurs et données clients.

## Structure du projet
- `sql/` : scripts SQL de chargement, nettoyage et analyse
- `notebooks/` : notebooks Snowflake / Jupyter
- `analytics/` : documentation du data product analytique

## Contribution – Partie 3.1
La partie 3.1 consiste à construire un **data product analytique** dans le schéma `ANALYTICS`.

Les objets créés incluent :
- `SALES_ENRICHED`
- `CUSTOMER_SEGMENTS`
- `CAMPAIGNS_ENRICHED`
- `PROMOTIONS_ENRICHED`
- `REVIEWS_AGGREGATED`
- `INVENTORY_AGGREGATED`
- `SUPPLIER_INVENTORY_SUMMARY`
- `MARKETING_PERFORMANCE_MART`
- `V_MARKETING_PERFORMANCE`

## Objectif métier
Transformer les analyses exploratoires en tables analytiques réutilisables pour :
- le pilotage marketing,
- les dashboards,
- et, à terme, des cas d’usage de machine learning.

## Remarque de modélisation
Les jeux de données ne partagent pas tous de clés transactionnelles communes.  
Le data product a donc été construit à une granularité agrégée, principalement **mois × région**, afin de garantir la cohérence métier.
