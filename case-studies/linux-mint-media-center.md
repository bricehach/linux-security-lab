# Poste multimédia personnalisé sous Linux Mint

**Auteur : Fabrice Hacardiaux**  
**Travaux d'origine : novembre 2025 — synthèse publiée le 2 novembre 2026**  
**Statut : retour d'expérience documentaire ; configuration finale et tests à compléter.**

## Besoin et contraintes

Réutiliser un Dell 1749 comme poste multimédia connecté par HDMI à une télévision non intelligente. L'environnement décrit dans les notes de travail est Linux Mint 22.2 Cinnamon, avec 8 Go de RAM et deux SSD de 500 Go.

Le besoin portait sur Kodi, les contenus directs et replays France/Belgique, les radios et l'accès aux services multimédias par navigateur. L'équilibre recherché associait simplicité d'utilisation, performances adaptées à un ancien ordinateur et maîtrise de la configuration.

## Personnalisation travaillée

| Partie | Travail décrit dans les notes |
|---|---|
| Interface multimédia | Articulation entre Kodi, navigateur et raccourcis |
| Navigateur | Choix de Chromium et d'un profil Replay distinct, sans mot de passe enregistré |
| Réseau | Poste câblé sur un switch ; configuration DNS via NetworkManager |
| Administration distante | Utilisation de RustDesk rapportée ; travail complémentaire sur son démarrage automatique |
| Sécurité | Examen du pare-feu et des services nécessaires |
| Stockage réseau | Accès local à un NAS envisagé, sans exposition web externe |

## Éléments documentaires retrouvés

- Procédure Kodi avec Catch-Up TV & More pour explorer les contenus France/Belgique : proposée dans les échanges, sans compte rendu complet de tests.
- Script nommé `set-adguard-dns.sh` : produit dans les échanges pour configurer le DNS avec NetworkManager, prévoir une vérification et un retour aux DNS automatiques.
- Retour utilisateur positif après présentation de la procédure DNS ; les sorties de contrôle ne sont pas jointes à cette publication.
- Projet de profil Kodi de référence et de déploiement automatisé : proposition de conception, sans preuve retrouvée d'un déploiement terminé.

Les anciens scripts ne sont pas joints : cette publication décrit les travaux retrouvés et ne reconstitue pas leur code de mémoire.

## Démarche d'intégration

Le travail relie un besoin d'usage à des décisions système : choisir les composants, adapter l'interface, organiser l'administration distante et examiner les services exposés. La personnalisation concerne ainsi l'ensemble du poste, au-delà de l'installation d'une application.

Les compétences mobilisées sont l'intégration Linux, l'adaptation au matériel existant, la configuration réseau, l'administration distante et la documentation.

## Vérifications à joindre pour une version reproductible

1. Version actuelle du système et des applications.
2. Captures de l'interface et liste des composants effectivement utilisés.
3. Tests HDMI, audio et navigation entre les usages.
4. Export anonymisé de la configuration réseau et du pare-feu.
5. Version relue des scripts, résultats de test et retour arrière.

Aucun résultat de performance, validation globale de sécurité ou fonctionnement de tous les services multimédias n'est revendiqué ici.

## Travaux associés

- [Administration distante RustDesk](rustdesk-linux-mint.md)
- [Audit et durcissement Linux](../hardening/audit-hardening-worklog.md)
- [Accueil du laboratoire](../README.md)
