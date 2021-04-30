# Edit settings / Settings list

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

### Ducks per day

The [`ducks_per_day`](https://duckhunt.me/commands/settings/ducks_per_day) setting controls the amount of ducks that will spawn during a 24-hour period. It is _not_ an exact number since some ducks aren't depleting that counter :

* Mechanical ducks bought from the shop
* Decoys that might bring ducks
* MOADs children

To prevent spam, the amount you can set here is limited. To increase the limit, you can [make your server VIP](../players-guide/how-to-contribute-to-the-bot.md), get more players to join your server and play with DuckHunt, or ask in the support server with a good reason.

To set the number of ducks per day, the command would be `d!settings ducks_per_day [amount]`, for example, typing `d!settings ducks_per_day 150` would give you 150 ducks per day, or approximately 6 every hour.

The related setting, [`ducks_time_to_live`](https://duckhunt.me/commands/settings/ducks_time_to_live) sets the time a duck will stay before leaving the pond.

### Experience-related settings

Every time a hunter kills a duck, they earn some experience. Experience is the game currency, and as such, you can make the game harder or easier by changing the following values.

There are four main settings to control that amount.

* [`base_duck_exp`](https://duckhunt.me/commands/settings/base_duck_exp) the amount a normal duck gives when killed
* [`per_life_exp`](https://duckhunt.me/commands/settings/per_life_exp) the amount added to the total for every life a duck has
* [`clover_min_experience`](https://duckhunt.me/commands/settings/clover_min_experience) the minimum amount a clover will give for every duck killed during the 24 hours following the purchase
* [`clover_max_experience`](https://duckhunt.me/commands/settings/clover_max_experience) the maximum value for a clover.

The total experience a hunter earns after killing a duck can be summarized by this formula :

`total = base_duck_exp + per_life_exp * (duck_lives-1) + clover_value`

Keep in mind that shop prices are fixed, and that changing the clover values will **not** affect existing clovers. To make the game easier, we recommend using the following commands :

* `dh!settings base_duck_exp 15`
* `dh!settings per_life_exp 13`
* `dh!settings clover_min_experience 5`
* `dh!settings clover_max_experience 13`

Adjust these values as needed.

### Super ducks lives

When a super duck spawn, it gets a certain amount of health. Two settings control how many lives a super duck can get.

* [`super_ducks_min_life`](https://duckhunt.me/commands/settings/super_ducks_min_life) the minimum hp a super duck can have
* [`super_ducks_max_life`](https://duckhunt.me/commands/settings/super_ducks_max_life) the maximum hp a super duck can have

Players can use some AP ammo, or some Explosive ammo to respectively double or triple the damage they do to ducks.

You can also decide to show the health left/total health of ducks using the [`show_duck_lives`](https://duckhunt.me/commands/settings/show_duck_lives) setting.

We recommend the following values :

* `dh!settings super_ducks_min_life 3` \(Don't set it lower than 2\)
* `dh!settings super_ducks_max_life 9` \(Set it to 7 if your gameplay is not competitive\)
* `dh!settings show_duck_lives False` \(Setting it to `True` would allow people to wait until the last possible moment before shooting\)

### Night

DuckHunt V4 allow you to set times when the nights start and ends on the channel. At night, different ducks appear, and they spawn less frequently. Note that times are given in `UTC`.

Set the times the night start and ends with the [`night_time`](https://duckhunt.me/commands/settings/night_time) command.

For example, if you want night to start at 21:30 UTC, and end at 6:20 UTC, you can use the following command :

`dh!settings night_time 21h30 6h20`

### Weights

Duck weights control the chance of a specific duck type to spawn. The higher the weight is, the higher the chance for a duck to be of that type.

### Webhooks

Webhooks are what make DuckHunt V4 special. They give special names and profile pictures to the bot, and look like this :

![What do webhooks look like ?](../.gitbook/assets/webhooks.png)

As you can see, the two ducks have different avatars and names. This is done using webhooks. To enable webhooks on your channel, make sure DuckHunt has the permission to create webhooks, and set [`use_webhooks`](https://duckhunt.me/commands/settings/use_webhooks) to true, like so `dh!settings use_webhooks True`

You can also add some webhooks with [`dh!settings add_webhook`](https://duckhunt.me/commands/settings/add_webhook) to prevent some lag due to discord ratelimits.

Note that it's useless to have more than 2 webhooks in use by DuckHunt for now, given current rate limits. Also note the discord limit of 10 webhooks per channel.

### Prefix

DuckHunt uses two types of prefixes : global prefixes \(`dh!`, `dh`, and @mention\), that you cannot change or edit, and a server prefix, used in your server. By default, the prefix used is `!`. If you find some other conflicts with DuckHunt, and you can't fix it using permissions, you can change your local prefix here. For example, if you wanted to use `$` instead, you could do [`dh!settings prefix $`](https://duckhunt.me/commands/settings/prefix).

### Annoyances

Certains paramètres peuvent faire en sorte que le bot mentionne les joueurs dans certains cas. Le réglage de [`mentions_when_killed`](https://duckhunt.me/commands/settings/mentions_when_killed) sur `False` empêchera DuckHunt de mentionner les chasseurs s'ils sont tués.

De plus, les joueurs peuvent désactiver la mention lorsque le bot leur répond en utilisant la commande suivante : [`dh!settings ping False`](https://duckhunt.me/commands/settings/ping). Notez que ce paramètre s'applique à un compte utilisateur sur tous les serveurs où se trouve DuckHunt. Il ne peut pas être configuré par canal.

Un autre paramètre est [`my_language`](https://duckhunt.me/commands/settings/my_language), qui permet à un utilisateur de définir la langue que le robot doit utiliser lorsqu'il communique avec lui dans les DM.

Si les emojis vous font lag, vous pouvez en désactiver certains à l'aide de la commande suivante [`dh!settings use_emojis False`](https://duckhunt.me/commands/settings/use_emojis)

