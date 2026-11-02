# Linux Security Lab

> Linux, administration système et sécurité appliqués à la cybersécurité.

Ce dépôt regroupe mes travaux autour de **Linux comme système à comprendre, administrer, observer et sécuriser**. Kali Linux et Parrot Security y apparaissent comme des environnements spécialisés, mais ils ne constituent pas à eux seuls l'objectif du repository.

Ma démarche consiste à maîtriser les bases du système : utilisateurs, permissions, processus, services, réseau, logs, shell et durcissement. Cette compréhension est indispensable pour utiliser correctement les outils cyber et interpréter ce qu'ils montrent.

> **Avant d'utiliser un outil de sécurité sous Linux, je veux comprendre le système sur lequel il s'exécute.**

---

## Positionnement dans mon parcours

```text
Infrastructure IT
      ↓
Windows + Linux
      ↓
Administration système
      ↓
Réseau / services / permissions
      ↓
Logs / processus / événements
      ↓
Hardening
      ↓
Outils de cybersécurité
      ↓
SOC / DFIR / Investigation
      ↓
Automatisation Bash / Python
```

Linux constitue donc une **fondation technique de mon orientation cybersécurité**, au même titre que Windows et le réseau.

---

## Ressources publiées et progression

Ce dépôt constitue le point central de mes travaux Linux, en lien avec mes laboratoires réseau, SOC et mes travaux d'automatisation.

### Déjà publié

- [tmux sur Debian](fundamentals/tmux/) : présentation, commandes de démarrage et cours complet au format Word.

### Rubriques à enrichir

L'arborescence ci-dessous constitue une organisation de travail. La présence d'une rubrique ne signifie pas qu'un guide complet ou un laboratoire validé y est déjà disponible.

Les prochaines publications seront sélectionnées parmi les travaux existants suffisamment complets : maintenance Kali et Parrot, diagnostic, audit avec Lynis et chkrootkit, outils réseau et automatisation Bash. Chaque document devra être relu et son état de vérification indiqué avant publication.

### Format des publications

Chaque guide, script ou laboratoire précise, selon le sujet :

- le problème ou l'objectif ;
- la distribution, la version et les prérequis ;
- les étapes et commandes expliquées ;
- les résultats attendus et, pour un laboratoire réalisé, les observations obtenues ;
- les contrôles de réussite, les limites et le retour arrière si applicable ;
- son statut : support documentaire, procédure testée ou laboratoire reproduit.

Les contenus communs sont conservés ici et référencés depuis les dépôts réseau ou SOC pour éviter les copies divergentes.

---

## Axes de travail

- administration Linux ;
- arborescence et système de fichiers ;
- utilisateurs et groupes ;
- permissions et élévation de privilèges ;
- processus et services ;
- systemd ;
- réseau Linux ;
- logs et journalctl ;
- paquets et mises à jour ;
- Bash et automatisation ;
- hardening ;
- diagnostic ;
- Kali Linux ;
- Parrot Security ;
- outils de sécurité et d'audit.

---

## Structure du dépôt

```text
linux-security-lab/
│
├── fundamentals/        # Arborescence, shell, fichiers, commandes
├── users-permissions/   # Comptes, groupes, sudo, droits
├── processes-services/  # Processus, systemd, services
├── networking/          # Interfaces, IP, DNS, sockets, diagnostic
├── logs-monitoring/     # journalctl, syslog et investigation
├── package-management/  # apt, mises à jour et versions
├── hardening/           # Réduction de surface d'attaque et contrôles
├── bash-automation/     # Scripts et automatisation
├── kali-parrot/         # Environnements spécialisés cyber
└── security-tools/      # Outils d'audit, analyse et investigation
```

---

## Méthode de travail

```text
Comprendre la fonction
        ↓
Observer l'état du système
        ↓
Utiliser la commande appropriée
        ↓
Interpréter le résultat
        ↓
Modifier si nécessaire
        ↓
Vérifier l'effet
        ↓
Analyser les logs
        ↓
Documenter
```

L'objectif n'est pas d'accumuler des commandes, mais de comprendre **ce qu'elles interrogent ou modifient**.

---

## Linux et cybersécurité

| Domaine Linux | Utilité cyber |
|---|---|
| Utilisateurs / groupes | contrôle des identités et privilèges |
| Permissions | protection des fichiers et limitation des accès |
| Processus | identification d'activités normales ou suspectes |
| Services | compréhension de la surface exposée |
| Réseau | observation des connexions et services à l'écoute |
| Logs | détection, investigation et chronologie |
| Paquets | suivi des versions et correctifs |
| Bash | automatisation et collecte d'informations |
| Hardening | réduction de la surface d'attaque |

---

## Distributions utilisées

### Debian et Linux Mint

Environnements de travail et d'apprentissage pour consolider l'administration système et les mécanismes fondamentaux de Linux. Le cours tmux publié est consacré à Debian.

### Kali Linux

Utilisé dans des laboratoires contrôlés pour l'apprentissage et l'utilisation d'outils de sécurité.

### Parrot Security

Utilisé comme environnement orienté sécurité, notamment en machine virtuelle et en installation physique de laboratoire.

Les outils présents dans ces distributions sont utilisés uniquement dans des environnements autorisés, personnels ou pédagogiques.

---

## Outils et sujets associés

Selon les laboratoires, ce dépôt pourra documenter notamment :

- Nmap ;
- Wireshark ;
- Netcat ;
- Lynis ;
- chkrootkit ;
- audit et hardening ;
- diagnostic réseau ;
- journalctl et logs Linux ;
- Bash ;
- analyse de services et processus.

---

## Formation

Ces travaux s'inscrivent dans ma formation **Conseiller en cybersécurité à l'IFAPME de Charleroi** et dans mon laboratoire personnel de cybersécurité.

---

## Objectif du dépôt

Ce repository doit montrer progressivement une démarche reproductible :

```text
Comprendre → Administrer → Observer → Sécuriser → Vérifier → Investiguer → Automatiser
```

Le but est de démontrer que Linux n'est pas seulement pour moi une plateforme portant des outils cyber, mais un **système que je cherche à comprendre suffisamment pour pouvoir le sécuriser et l'analyser correctement**.

---

### Fabrice Hacardiaux

**Infrastructure Windows / Linux • Cybersécurité / SOC • DFIR • Automatisation**

[Profil GitHub](https://github.com/bricehach) • [LinkedIn](https://www.linkedin.com/in/fabricehacardiaux)
