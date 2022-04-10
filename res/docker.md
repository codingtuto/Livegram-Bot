# Bot de relais de télégramme

Ce programme est distribué dans l'espoir qu'il sera utile, mais SANS AUCUNE GARANTIE ; sans même la garantie implicite de QUALITÉ MARCHANDE ou d'ADÉQUATION À UN USAGE PARTICULIER. Voir [COPYING](./../COPYING) pour plus de détails.


#### La manière facile [ 🐳 ]

J'écris ceci à nouveau, car j'ai vu de nombreux utilisateurs recommander **SUDO** d'installer Docker.
Il n'est pas recommandé d'utiliser "sudo", lors de l'utilisation de Docker.
Les autorisations GNU/Linux sont hautement personnalisables et il n'est généralement pas nécessaire d'avoir l'autorisation "ROOT", ~~à moins que vous ne sachiez ce que vous faites~~.
Vous pouvez toujours installer toutes les dépendances de votre système [avec les autorisations ROOT],
mais soyez conscient des problèmes potentiels lorsque vous le faites. Les packages installés
peut entrer en conflit avec les packages installés du gestionnaire de packages système, ce qui peut
causer des problèmes sur la route et des erreurs lors de la mise à jour de packages en conflit.
**Tu étais prévenu.**

- **Install docker** : suivez le docker officiel [guide d'installation](https://docs.docker.com/engine/install/).

- **Installez Docker-compose** : suivez le [guide d'installation] du compositeur officiel (https://docs.docker.com/compose/install/).

- **créer un fichier CONFIG** :
  - ```wget https://raw.githubusercontent.com/SpEcHiDe/NoPMsBot/master/sample_config.env -O config.env```
  - modifiez le fichier en supprimant le `#` dans les champs obligatoires et en ajoutant des valeurs.

- **téléchargement du fichier YAML `docker-compose` de NoPMsBot** :
  - ```wget https://raw.githubusercontent.com/SpEcHiDe/NoPMsBot/master/docker-compose.yml```

- **démarrez le bot** : ```docker-compose up -d```

- Le bot devrait fonctionner maintenant. Vérifiez les journaux avec ```docker-compose logs -f```


## Crédits et merci à

* [ThankTelegram](https://telegram.dog/ThankTelegram)
* [Dan Tès](https://telegram.dog/haskell) pour sa [Bibliothèque Pyrogram](https://github.com/pyrogram/pyrogram)
