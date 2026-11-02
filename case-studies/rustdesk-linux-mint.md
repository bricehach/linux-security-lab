# RustDesk sous Linux Mint : intégration et démarrage automatique

**Auteur : Fabrice Hacardiaux**  
**Travaux d'origine : novembre 2025 — synthèse publiée le 2 novembre 2026**  
**Statut : configuration et contrôles partiels rapportés ; test distant de bout en bout à documenter.**

## Objectif

Administrer à distance un poste Linux Mint 22.2 et obtenir un démarrage prévisible de RustDesk : composant de service au démarrage du système et interface disponible à l'ouverture de session.

## Situation et choix travaillés

Les échanges décrivent d'abord une installation Flatpak, puis une installation au format `.deb`. Le travail a porté sur l'articulation entre le service systemd, le lancement de l'interface et le pare-feu UFW.

Les points de configuration étudiés incluaient :

- l'unité `rustdesk.service` ;
- le lancement de l'interface par un fichier d'autostart ;
- la distinction entre le fonctionnement du service et celui de l'interface utilisateur ;
- l'examen des processus et des écoutes réseau ;
- les permissions de contrôle, de transfert et de presse-papiers.

Les notes comprennent aussi une checklist de configuration RustDesk : identification du poste, mode d'autorisation, permissions, paramètres réseau et journalisation. Cette checklist est un support documentaire, pas la preuve que tous ses réglages ont été appliqués.

## État des observations conservées

| Élément | État dans les notes historiques |
|---|---|
| Installation `.deb` | Mentionnée comme environnement de travail |
| Service systemd | Rapporté `enabled` et `active` |
| Processus RustDesk | Plusieurs processus rapportés, dont service et interface |
| Connexion distante | Usage rapporté dans un échange ; test final après configuration du démarrage encore proposé |
| Redémarrage puis prise en main complète | Pas de compte rendu de validation joint |

Ces observations proviennent des notes historiques. Les captures et sorties originales ne sont pas jointes à cette première synthèse.

## Ce que le cas illustre

L'installation d'un paquet ne suffit pas à documenter un service exploitable. Il faut aussi distinguer le démarrage système, la session graphique, la connectivité et les permissions accordées.

Ce cas mobilise la gestion des paquets, systemd, l'autostart, le diagnostic réseau et le contrôle des accès.

## Limites et prochaine validation

Les anciennes règles de ports ne sont pas reproduites comme configuration recommandée : leur pertinence dépend du rôle réel du poste et de l'architecture RustDesk utilisée.

Une version reproductible devra préciser :

1. la version de RustDesk et le mode de connexion ;
2. le rôle du poste et les éventuels serveurs associés ;
3. les fichiers de configuration réellement appliqués, anonymisés ;
4. le comportement après redémarrage et avant/après ouverture de session ;
5. un test distant, les permissions vérifiées et les journaux utiles ;
6. la procédure de désactivation ou de retour arrière.

Aucun auto-hébergement de serveur RustDesk ni validation globale de sécurité n'est présenté comme réalisé.

[Retour à l'accueil](../README.md)
