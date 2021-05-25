# Édition des réglages / Liste des préférences

## Que sont les paramètres ?

Les paramètres sont utilisés pour personnaliser l'expérience de chasse sur votre canal. \(✨ Nouveau sur la V4 : les paramètres sont désormais par canal\).

### Quels sont _tout_ les paramètres ?

Vous pouvez voir les paramètres auxquels vous pouvez accéder, et les autorisations requises pour les modifier, vous pouvez voir la [liste des sous-commandes des paramètres](https://duckhunt.me/commands/settings).

Cette page est là pour expliquer ce que font exactement les paramètres, et comment les configurer. Ils sont classés ici dans un ordre arbitraire d'"importance". Plus le paramètre est important, plus il sera élevé.

Notez que certains paramètres peuvent maintenant être affichés ici. Utilisez le lien ci-dessus pour les afficher tous.

## Commandes utiles

Vous pouvez utiliser `dh!settings [your_setting_name]` pour voir la valeur du paramètre actuel... Ou vous pouvez aussi regarder tous les paramètres en faisant `dh!settings` pour obtenir un lien vers les paramètres actuels de votre canal. N'oubliez pas de rafraîchir la page après les avoir mis à jour ;\)

## Paramètres les plus importants

### La langue du serveur

Il s'agit de la langue utilisée sur le serveur. En définissant cette option, les messages du robot seront traduits dans la langue de votre serveur.

Pour voir toutes les langues disponibles, utilisez la commande [`dh!translators`](https://duckhunt.me/commands/translators).

N'oubliez pas que le bot est traduit par des humains comme vous. Si vous souhaitez voir une langue qui ne figure pas dans cette liste, vous pouvez demander à [traduire le bot](../players-guide/how-to-contribute-to-the-bot.md). Si une langue n'est pas finie, certaines phrases peuvent être envoyées en anglais à la place.

Parfois, vous pouvez constater des erreurs de grammaire ou des fautes de frappe. Dans ce cas, veuillez contacter directement le traducteur pour qu'il les corrige, ou bien prévenez-nous sur le[ serveur d'assistance.](https://discordapp.com/invite/2BksEkV)

### Canards par jour

Le paramètre [`ducks_per_day`](https://duckhunt.me/commands/settings/ducks_per_day) contrôle le nombre de canards qui vont apparaître pendant une période de 24 heures. Ce n'est pas un nombre exact puisque certains canards n'épuisent pas ce compteur :

* Canards mécaniques achetés au magasin
* Les leurres qui peuvent amener des canards
* Les enfants des [MOADs](../players-guide/types-of-ducks.md#moad-mother-of-all-ducks-mere-de-tous-les-canards)

Pour éviter le spam, le montant que vous pouvez définir ici est limité. Pour augmenter la limite, vous pouvez [rendre votre serveur VIP](../players-guide/how-to-contribute-to-the-bot.md#donner), faire en sorte que plus de joueurs rejoignent votre serveur et jouent avec DuckHunt, ou demander au serveur de support avec une bonne raison.

Pour définir le nombre de canards par jour, la commande sera `dh!settings ducks_per_day [montant]`, par exemple, en tapant `dh!settings ducks_per_day 150`, vous obtiendrez 150 canards par jour, soit environ 6 par heure.

Le paramètre associé, [`ducks_time_to_live`](https://duckhunt.me/commands/settings/ducks_time_to_live), définit le temps que les canards resteront avant de quitter l'étang.

### Paramètres liés à l'expérience

Chaque fois qu'un chasseur tue un canard, il gagne de l'expérience. L'expérience est la monnaie du jeu, et en tant que telle, vous pouvez rendre le jeu plus difficile ou plus facile en modifiant les valeurs suivantes.

Il existe quatre paramètres principaux pour contrôler cette quantité.

* [`base_duck_exp`](https://duckhunt.me/commands/settings/base_duck_exp) le montant que donne un canard normal lorsqu'il est tué
* [`per_life_exp`](https://duckhunt.me/commands/settings/per_life_exp) le montant ajouté au total pour chaque vie d'un canard
* [`clover_min_experience`](https://duckhunt.me/commands/settings/clover_min_experience) le montant minimum qu'un trèfle donnera pour chaque canard tué dans les 24 heures suivant l'achat
* [`clover_max_experience`](https://duckhunt.me/commands/settings/clover_max_experience) la valeur maximale pour un trèfle.

L'expérience totale qu'un chasseur acquiert après avoir tué un canard peut être résumée par cette formule :

`total = base_duck_exp + per_life_exp * (duck_lives-1) + clover_value`

Gardez à l'esprit que les prix des boutiques sont fixes et que la modification des valeurs des trèfles n'affectera pas les trèfles existants. Pour faciliter le jeu, nous vous recommandons d'utiliser les commandes suivantes :

* `dh!settings base_duck_exp 15`
* `dh!settings per_life_exp 13`
* `dh!settings clover_min_experience 5`
* `dh!settings clover_max_experience 13`

Ajustez ces valeurs si nécessaire.

### La vie des super canards

Lorsqu'un super canard apparaît, il reçoit un certain nombre de points de vie. Deux paramètres contrôlent le nombre de vies qu'un super canard peut obtenir.

* [`super_ducks_min_life`](https://duckhunt.me/commands/settings/super_ducks_min_life) la vie minimale qu'un super canard peut avoir
* [`super_ducks_max_life`](https://duckhunt.me/commands/settings/super_ducks_max_life) la vie maximale qu'un super canard peut avoir

Les joueurs peuvent utiliser des munitions AP ou des munitions explosives pour respectivement doubler ou tripler les dégâts qu'ils infligent aux canards.

Vous pouvez également décider d'afficher la santé restante/la santé totale des canards en utilisant le paramètre [`show_duck_lives`](https://duckhunt.me/commands/settings/show_duck_lives)`.`

Nous recommandons les valeurs suivantes :

* `dh!settings super_ducks_min_life 3` \(Ne le réglez pas plus bas que 2\)
* `dh!settings super_ducks_max_life 9` \(Réglez-le sur 7 si votre jeu n'est pas compétitif\).
* `dh!settings show_duck_lives False` \(En le réglant sur True, les gens pourront attendre le dernier moment avant de tirer.\)

### Nuit

DuckHunt V4 vous permet de définir les heures auxquelles les nuits commencent et se terminent sur la chaîne. La nuit, des canards différents apparaissent, et ils apparaissent moins fréquemment. Notez que les heures sont données en `UTC`.

Définissez les heures de début et de fin de la nuit avec la commande [`night_time`](https://duckhunt.me/commands/settings/night_time).

Par exemple, si vous voulez que la nuit commence à 21:30 UTC et se termine à 6:20 UTC, vous pouvez utiliser la commande suivante :

`dh!settings night_time 21h30 6h20`

### Pondérations

Les pondérations des canards contrôlent la probabilité qu'un type de canard spécifique apparaisse. Plus le poids est élevé, plus la probabilité qu'un canard soit de ce type est élevée.

### Webhooks

Les Webhooks sont ce qui rend DuckHunt V4 spécial. Ils donnent des noms spéciaux et des photos de profil au bot, et ressemblent à ceci :

![&#xC0; quoi ressemblent les webhooks ?](../.gitbook/assets/webhooks.png)

Comme vous pouvez le voir, les deux canards ont des avatars et des noms différents. Ceci est fait en utilisant des webhooks. Pour activer les webhooks sur votre canal, assurez-vous que DuckHunt a la permission de créer des webhooks, et mettez [`use_webhooks`](https://duckhunt.me/commands/settings/use_webhooks) à true, comme ceci `dh!settings use_webhooks True`

Vous pouvez également ajouter quelques webhooks avec [`dh!settings add_webhook`](https://duckhunt.me/commands/settings/add_webhook) pour éviter un certain lag dû aux ratelimits de discord.

Notez qu'il est inutile d'avoir plus de 2 webhooks utilisés par DuckHunt pour le moment, étant donné les limites de débit actuelles. Notez également la limite discord de 10 webhooks par canal.

### Préfixes

DuckHunt utilise deux types de préfixes : les préfixes globaux \(`dh!`, `dh`, et @mention\), que vous ne pouvez pas changer ou modifier, et un préfixe de serveur, utilisé dans votre serveur. Par défaut, le préfixe utilisé est `!` Si vous trouvez d'autres conflits \(d'autres bots utilisant le même préfixe\) avec DuckHunt, et que vous ne pouvez pas les résoudre en utilisant les permissions, vous pouvez changer votre préfixe local. Par exemple, si vous voulez utiliser $ à la place, vous pouvez faire [`dh!settings prefix $`](https://duckhunt.me/commands/settings/prefix).

### Embêtements

Certains paramètres peuvent faire en sorte que le bot mentionne les joueurs dans certains cas. Le réglage de [`mentions_when_killed`](https://duckhunt.me/commands/settings/mentions_when_killed) sur `False` empêchera DuckHunt de mentionner les chasseurs s'ils sont tués.

De plus, les joueurs peuvent désactiver la mention lorsque le bot leur répond en utilisant la commande suivante : [`dh!settings ping False`](https://duckhunt.me/commands/settings/ping). Notez que ce paramètre s'applique à un compte utilisateur sur tous les serveurs où se trouve DuckHunt. Il ne peut pas être configuré par canal.

Un autre paramètre est [`my_language`](https://duckhunt.me/commands/settings/my_language), qui permet à un utilisateur de définir la langue que le robot doit utiliser lorsqu'il communique avec lui dans les DM.

Si les emojis vous font lag, vous pouvez en désactiver certains à l'aide de la commande suivante [`dh!settings use_emojis False`](https://duckhunt.me/commands/settings/use_emojis)

