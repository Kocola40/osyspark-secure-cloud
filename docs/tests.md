# Plan de tests — OsySpark Secure Cloud

Toutes les manipulations sont autorisées **uniquement dans le laboratoire isolé**, sur des équipements et comptes de test.

| Réf. | Scénario | Critère d'acceptation | État |
|---|---|---|---|
| T01 | Accès du VLAN clients à l'administration | Refus journalisé | Non testé |
| T02 | Flux métier explicitement autorisé | Connexion réussie | Non testé |
| T03 | Connexion Keycloak avec MFA | Deuxième facteur requis | Non testé |
| T04 | Compte standard tentant une action admin | Opération refusée | Non testé |
| T05 | Erreurs de connexion remontées à Wazuh | Événement et horodatage visibles | Non testé |
| T06 | Trafic de test observé par Suricata | Log IDS vérifiable | Non testé |
| T07 | Restauration d'un fichier fictif | Empreinte SHA-256 identique, temps mesuré | Non testé |
| T08 | Automatisation Ansible répétée | Résultat stable sans dérive | Non testé |

## Modèle de preuve
Pour chaque test : date, topologie, versions, prérequis, commande ou action réalisée, résultat attendu, résultat observé, mesure, capture anonymisée et conclusion. Ne jamais publier d'identifiants, de secrets, d'adresses publiques ou de données personnelles.

**Important :** toutes les démonstrations sont au stade de préparation.
