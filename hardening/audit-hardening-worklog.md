# Audit et durcissement Linux — travaux et état documentaire

**Auteur : Fabrice Hacardiaux**  
**Publication : 2 novembre 2026**  
**Statut : inventaire de travaux et méthode de restitution ; rapports d'exécution à intégrer.**

## Périmètre

Cet axe rassemble les travaux de diagnostic, d'audit et de durcissement Linux, en complément des configurations personnalisées du poste Linux Mint et des laboratoires de sécurité.

L'objectif documentaire est de relier chaque constat à son contexte, à une vérification et, si une correction est appliquée, à un contrôle de son effet.

## Matière identifiée

| Sujet | Éléments disponibles dans l'historique de travail | Limite actuelle |
|---|---|---|
| UFW / GUFW | Travail sur la politique du pare-feu, les règles, les services et les écoutes ; script `check_firewall_ufw.sh` produit dans les échanges | Code original et sorties à récupérer et relire |
| Services Linux Mint | Examen de CUPS, SSH, Avahi et UPnP selon leur utilité | Désactivation effective de chaque service à documenter |
| DNS / NetworkManager | Script `set-adguard-dns.sh`, vérification et retour aux DNS automatiques prévus | Version originale et preuves de test non jointes |
| Lynis | Travaux d'audit et de durcissement identifiés dans les échanges | Rapports, constats retenus et corrections à retrouver |
| LinPEAS | Travaux de recherche de faiblesses rappelés par l'auteur lors de la préparation du portfolio | Cible, version, sorties et pistes vérifiées à retrouver |
| chkrootkit | Sujet de diagnostic et d'interprétation des signalements identifié dans les échanges | Sorties et conclusions vérifiées à retrouver |

Cette page ne présente aucun score d'audit, résultat d'exploitation ou diagnostic de compromission comme établi.

## Organisation des publications

- **Audit et durcissement** : contexte, constats, décisions de correction et comparaison avant/après.
- **Recherche de mauvaises configurations** : environnement de laboratoire, pistes relevées et vérifications.
- **Diagnostic** : symptômes, observations, hypothèses, résultats et limites.
- **Automatisation** : scripts originaux relus, prérequis, tests et retour arrière.

Les outils sont documentés dans le contexte des travaux réalisés ; leur présence dans cet inventaire ne signifie pas qu'un laboratoire complet est déjà publié.

## Fiche de restitution commune

Pour chaque cas, conserver :

| Champ | Contenu à fournir |
|---|---|
| Besoin | Pourquoi le contrôle est réalisé |
| Environnement | Distribution, version, rôle de la machine et périmètre autorisé |
| État initial | Configuration et observations avant intervention |
| Exécution | Outil, version, options et date |
| Constat | Extrait anonymisé de la sortie, avec contexte |
| Vérification | Contrôle du constat et limites de l'interprétation |
| Décision | Correction retenue, reportée ou écartée et justification |
| Résultat | Comparaison avant/après et vérification de l'usage normal |
| Retour arrière | Méthode de restauration si une modification est appliquée |

## Prochaines pièces à intégrer

Les priorités sont les scripts originaux d'audit UFW et de configuration DNS, puis un cas Lynis et un cas LinPEAS accompagnés de leurs observations. Leur publication comme procédures testées dépendra de la récupération des sources et de la vérification des résultats.

## Cas associés

- [Poste multimédia Linux Mint](../case-studies/linux-mint-media-center.md)
- [RustDesk sous Linux Mint](../case-studies/rustdesk-linux-mint.md)
- [Accueil du laboratoire](../README.md)
