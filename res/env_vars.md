# Bot de relais de télégramme

Ce programme est distribué dans l'espoir qu'il sera utile, mais SANS AUCUNE GARANTIE ; sans même la garantie implicite de QUALITÉ MARCHANDE ou d'ADÉQUATION À UN USAGE PARTICULIER. Voir [COPYING](./../COPYING) pour plus de détails.


## Variables d'environnement

#### Variables d'environnement obligatoires

* `TG_BOT_TOKEN` : créez un bot à l'aide de [@BotFather](https://telegram.dog/BotFather) et obtenez le jeton API Telegram.

* `ID_APP`
* `API_HASH` : obtenez ces deux valeurs à partir de [my.telegram.org/apps](https://my.telegram.org/apps).
  * N.B. : si Telegram est bloqué par votre FAI, essayez notre [bot Telegram](https://telegram.dog/UseTGXBot) pour obtenir les identifiants.

* `CANAL_AUTH` :
Créez un super groupe dans Telegram, ajoutez `@GoogleIMGBot` au groupe et envoyez /id dans le chat pour obtenir cette valeur.

* `DATABASE_URL` : ~~si vous utilisez Heroku, cette valeur est automatiquement remplie par le plugin Postgres.~~ si vous n'utilisez pas Heroku, lisez le guide sur [comment installer la base de données ?](https://github. com/SpEcHiDe/NoPMsBot/wiki/How-to-Install-Database-%3F).

#### Variables d'environnement facultatives

* `TG_BOT_WORKERS` : nombre de travailleurs à utiliser. 4 est le montant recommandé (et par défaut), mais votre expérience peut varier.
 __Note__ que devenir fou avec plus de travailleurs n'accélérera pas nécessairement votre bot, compte tenu de la quantité d'accès aux données sql et du fonctionnement des appels asynchrones python.

* `COMMM_AND_PRE_FIX` : Le préfixe de la commande. Telegram, par défaut, recommande l'utilisation de `/`, qui est le préfixe par défaut.

* `BAN_COMMAND` : La commande qui peut être utilisée par les administrateurs du bot pour bannir des utilisateurs. La valeur par défaut est "interdire".

* `UN_BAN_COMMAND` : La commande qui peut être utilisée par les administrateurs du bot pour débannir les utilisateurs. La valeur par défaut est `unban`.

* `START_COMMAND` : La commande pour vérifier si le bot est actif, ou pour que les utilisateurs démarrent le robot.

* `START_OTHER_USERS_TEXT` : envoyez un message dans votre `AUTH_CHANNEL` et collez message_id dans cette valeur.

* `ONLINE_CHECK_START_TEXT` : le message que les administrateurs du bot peuvent utiliser pour vérifier si le bot est en ligne.

* `DELETED_MESSAGES_NOTIFICATION_TEXT` : le message que les administrateurs du bot peuvent voir si un message a été supprimé par l'utilisateur.

* `DERP_USER_S_TEXT` : conservez la valeur par défaut, à moins que vous ne sachiez ce que vous faites.

* `IS_BLACK_LIST_ED_MESSAGE_TEXT` : Le message à afficher à l'utilisateur, lorsqu'un administrateur l'exclut du bot.

* `REASON_DE_LIMIT_ER` : conservez la valeur par défaut, à moins que vous ne sachiez ce que vous faites.

* `IS_UN_BANED_MESSAGE_TEXT` : Le message à afficher à l'utilisateur, lorsqu'un administrateur le débanni du bot.

* `BOT_WS_BLOCKED_BY_USER` : Le message à afficher à l'administrateur, si le bot a été bloqué par l'utilisateur.

* `LOG_FILE_ZZGEVC` : le chemin pour stocker les fichiers journaux.


## Crédits et merci à

* [ThankTelegram](https://telegram.dog/ThankTelegram)
* [Dan Tès](https://telegram.dog/haskell) pour sa [Bibliothèque Pyrogram](https://github.com/pyrogram/pyrogram)
