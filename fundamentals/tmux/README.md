# tmux sur Debian

Ce dossier rassemble le cours consacré à **tmux**, le multiplexeur de terminal utilisé pour organiser plusieurs sessions de travail et reprendre un terminal après une coupure de connexion SSH.

## Support de cours

[ Télécharger le cours complet au format Word ](Cours_complet_tmux_Debian.docx)

## Contenu

Le cours progresse des concepts de base vers les usages plus avancés :

- architecture serveur, client, sessions, fenêtres et panneaux ;
- installation et vérification sur Debian ;
- raccourcis et gestion des sessions ;
- navigation entre fenêtres et panneaux ;
- historique, recherche et copier-coller ;
- cibles et commandes tmux ;
- configuration de `~/.tmux.conf` ;
- reprise d’une session après une coupure SSH ;
- automatisation d’espaces de travail ;
- dépannage, sécurité et bonnes pratiques.

## Limite à retenir

tmux permet aux programmes de continuer lorsque le client terminal ou la connexion SSH disparaît, tant que le serveur et le processus tmux restent actifs. Il ne restaure pas les processus après un redémarrage du serveur.

## Démarrage rapide

```bash
sudo apt update
sudo apt install tmux
tmux new -A -s travail
```

Détacher sans fermer le travail : **Ctrl+b**, puis **d**. Pour reprendre :

```bash
tmux attach -t travail
```

