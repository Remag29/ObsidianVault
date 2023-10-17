# Scénarios pour un contrôle d’accès dépendant du contexte opérationnel

Mise en lumière de cas “d’urgence” qui peuvent conditionner l’accès à des données jugé sensible/secrète (exemple des dossiers santé pour les médecins).

> *\[…], la décision d’accorder ou non l’accès n’est pas seulement prise selon le sujet (et ses habilitations), l’action et l’objet (et sa classification) \[...], mais également selon la situation opérationnelle et le contexte dans lesquels l’accès est demandé.*

# Contrôle d’accès basé attributs
![[Pasted image 20231013102745.png]]
> _Figure 1: Architecture fonctionnelle typique pour mettre en œuvre le contrôle d’accès basé attributs._

**PEP** : _Policy Enforcement Point_
Intercepte toutes les requêtes des clients pour mettre en œuvre le contrôle d’accès

**PDP** : _Policy Decision Point_
Chargé d’évaluer la politique de contrôle d’accès fournis par le **PAP**

**PAP** : _Policy Administration Point_


**PIP** : _Policy Information Point_
Calcule le contexte opérationnel.
 
