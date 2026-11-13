# OsySpark Secure Cloud — Portfolio M1

**Projet académique Cloud + Cybersécurité · Objectif : 0 € de dépenses supplémentaires.**

Ce dépôt contient le **site portfolio statique** et les supports de préparation d'un laboratoire destiné à une soutenance de Master 1. L'étude de cas concerne une **startup fictive** de 8 collaborateurs, susceptible d'atteindre 20 utilisateurs. Le portfolio présente un **projet en conception**, pas un service commercial ni un environnement déjà déployé.

## Ce qui est prêt

- `index.html` : portfolio responsive, autonome, sans framework ni ressources externes.
- `docs/architecture.md` : architecture conceptuelle, laboratoire et segmentation.
- `docs/roadmap.md` : jalons de construction avec livrables.
- `docs/tests.md` : protocoles des huit scénarios de validation.
- `docs/budget.md` : cadre « zéro achat » et limites du budget.
- `docs/publication.md` : guide de publication gratuite sur GitHub Pages.
- `preuves/README.md` : règles de publication de captures, mesures et résultats.

> **Statut initial :** architecture proposée, démonstrations non réalisées. Ne modifier les statuts des tests qu'après vérification réelle.

## Technologies envisagées

| Besoin | Outil libre / gratuit | Rôle |
|---|---|---|
| Virtualisation | Proxmox VE | VMs et réseau virtualisé |
| Pare-feu | OPNsense | VLAN, ACL, VPN |
| IAM | Keycloak | SSO / MFA de laboratoire |
| Collaboration | Nextcloud | Fichiers et partage |
| SIEM | Wazuh | Supervision des événements |
| IDS | Suricata | Détection réseau |
| Sauvegarde | restic | Copies chiffrées et restauration |
| Automatisation | Ansible | Configurations reproductibles |
| Publication | GitHub Pages | Site portfolio public sans achat de domaine |

### Contrainte matérielle

L'installation simultanée de tous les composants peut dépasser les ressources d'un ordinateur standard. **32 Go de RAM** constituent un objectif de confort pédagogique, et **Wazuh recommande 8 GiB de RAM et 4 vCPU pour 1 à 25 agents** dans son installation centralisée de démarrage. Si tu disposes de 8 à 16 Go de RAM, réalise les scénarios en séquence ou choisis un sous-ensemble d'outils : le budget doit rester à 0 € de dépenses supplémentaires, et non pousser à acheter du matériel.

## Lancer le site localement

Double-clique sur `index.html` pour l'ouvrir dans un navigateur. Aucun environnement Node.js ni compilation nécessaire.

Optionnel :

```bash
python3 -m http.server 8000
```

Puis ouvre `http://localhost:8000`.

## Publier gratuitement

Voir [`docs/publication.md`](docs/publication.md). Pour GitHub Free, le dépôt doit être **public**. Ne jamais y ajouter des mots de passe, des fichiers `.env`, des clés API, des exports d'identité, des journaux contenant des informations personnelles ni des captures avec des informations sensibles.

## Définition de « zéro euro »

0 € signifie **aucun nouvel achat ou abonnement prévu** grâce aux solutions libres, à la machine existante et à GitHub Pages. Cela ne signifie **pas** qu'une infrastructure de production d'entreprise coûterait réellement 0 € : temps humain, électricité, connexion, renouvellement, support et hébergement réel ont un coût.

## Crédits et sources

- Cas d'étude original : « Infrastructure informatique d'une startup en création » (EduSpark, document pédagogique, mai 2025).
- [GitHub Pages – documentation officielle](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
- [Proxmox VE – démarrer](https://proxmox.com/en/products/proxmox-virtual-environment/get-started)
- [OPNsense – documentation](https://docs.opnsense.org/intro.html)
- [Wazuh – prérequis](https://documentation.wazuh.com/current/quickstart.html)
- [Keycloak – site officiel](https://www.keycloak.org/)

## Suite

1. Adapter les informations publiques du portfolio.
2. Publier le dépôt, puis ajouter son URL dans le pied de page du site.
3. Réaliser les modules du laboratoire selon la roadmap.
4. Ajouter des captures et mesures authentiques, puis mettre à jour les statuts.
5. Construire le diaporama de soutenance à partir des preuves obtenues.