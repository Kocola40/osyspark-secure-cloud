# Roadmap — réalisation du laboratoire

| Phase | Objectif | Preuve attendue | État |
|---|---|---|---|
| P1 Cadrage | Besoins, périmètre et risques | Analyse des risques | À faire |
| P2 Réseau | Hyperviseur, OPNsense, VLAN | Plan IP, tests ACL | À faire |
| P3 Identité | Keycloak, MFA, RBAC | Captures et journal d'accès | À faire |
| P4 Supervision | Wazuh, éventuellement Suricata | Alertes contrôlées | À faire |
| P5 Résilience | Sauvegardes restic | Mesure de restauration | À faire |
| P6 Soutenance | Rapport et démonstration | Vidéo/captures expurgées | À faire |

Ordre conseillé : vérifier le matériel, construire deux VMs de test et un pare-feu, valider la segmentation, puis ajouter progressivement IAM, logs et sauvegardes. Pour chaque phase, consigner la date, les versions, le résultat observé et les limites ; aucun test ne doit être présenté comme réussi sans preuve.
