# Quelles sont les nouveautés de Duckhunt V4 ?

DuckHunt V4 est une réécriture complète du bot DuckHunt. En tant que tel, vous pouvez vous attendre à de nombreux changements, comme de nouveaux canards, de nouveaux événements, un meilleur leveling, et plus encore.

## Nouveau canards

Sur V3, il n'y avait que quelques types de canards :

* La [MOAD](players-guide/types-of-ducks.md#moad-mother-of-all-ducks) \(Mother of All Ducks, ou Mère de tous les Canards en français\)
* Le [Super Canard](players-guide/types-of-ducks.md#super-ducks)
* Le [Canard mécanique](players-guide/types-of-ducks.md#mechanical)
* Le [Canard normal](players-guide/types-of-ducks.md#normal-ducks)
* Le [Bébé canard](players-guide/types-of-ducks.md#baby)

Sur la V4, ces canards ont été conservés, et de nouveaux sont apparus :

* Le [Canard en Armure](players-guide/types-of-ducks.md#canards-en-armure) \(résiste à la plupart des tirs\)
* Le [Prof Canard](players-guide/types-of-ducks.md#prof-pr-duck) \(demande des calculs\)
* Le [Canard Doré](players-guide/types-of-ducks.md#canard-dore) et le [Canard en Plastique](players-guide/types-of-ducks.md#canard-en-plastique) \(qui valent respectivement plus et moins d'exp\)
* Le [Canard Kamikaze](players-guide/types-of-ducks.md#kamikaze) \(tue les autres canards\)
* Le [Canard Fantôme](players-guide/types-of-ducks.md#canard-fantome) \(n'envoie pas de messages quand il arrive\)
* Les canards de nuit : le [Canard de Nuit](players-guide/types-of-ducks.md#canard-de-la-nuit) et le [Canard Endormi](players-guide/types-of-ducks.md#canard-de-la-nuit).

### Le Boss Canard

Un autre type de canard est le Boss Canard. Il apparait dans le salon \#genetically-modified-ducks sur le serveur officiel de DuckHunt uniquement, et donne à tous ceux qui contribuent à le tuer une "Boîte de Foie Gras" qu'ils peuvent utiliser dans n'importe quel salon du jeu.

## Design

{% hint style="info" %}
Pour que le nouveau design fonctionne, DuckHunt a besoin de la permission `manage_webhooks` dans son salon. Si vous voyez encore des canards à l'ancien design, demande à un admin de changer la permission, puis d'utiliser la commande  `dh!settings use_webhooks True` dans le salon.
{% endhint %}

Les canards ont un meilleur design avec le pouvor des webhooks : chaque canard a maintenant un avatar customisé \(fait par Calgeka - /kalʒɛka/\#5963\)

![Regarde les diff&#xE9;rentd avatars, noms et messages.De haut en bas : Normal, MOAD, Super, Armure.](.gitbook/assets/webhooks-example.png)

## Un site web tout neuf

Le site web de DuckHunt a aussi été amélioré. Plus de statistiques sont enregistrées et sont accessibles aux joueurs sur leur page perso, incluant leurs meilleurs temps par type de canard, et bien d'autres.

![Avec aussi un th&#xE8;me sombre !](.gitbook/assets/new-graphs.png)

Vous y trouverez aussi la [liste des commandes](https://duckhunt.me/commands), une [documentation](https://duckhunt.me/fr/docs/) complète pour la V4, les informations [en direct](https://duckhunt.me) sur l'evènement en cours et le nombre de canards dans tout Discord, ainsi qu'une page de [statut](https://duckhunt.me/status) pour vérifier si le bot va bien !

## New shop items

Global usage of the shop items have been simplified, and some new items like the [autoreloader](https://duckhunt.me/commands/shop/reloader) have been added.

## A prestige system

A new prestige system will keep the game fun and different, allowing you to get access to exclusive bonuses.

Prestige is a way for you to restart the DuckHunt adventure, resetting your account \(experience, statistics, ...\) In exchange for the reset, you'll get new items to help you progress faster.

Learn more [here](players-guide/levels-and-experience.md#prestige-levels).

## Inline help, statistics, and topscores

If you don't like to open a website to see your statistics and the commands list, DuckHunt V4 has got you covered : the [`dh!help`](https://duckhunt.me/commands/) command sends you the list of commands, directly in discord !

![You can see your current level too !](.gitbook/assets/inline-information-about-a-hunter.png)

## A channel to follow to see new events and freetime in the chat

{% hint style="info" %}
This needs some setup : your server admin must follow the channel in your duckhunt channel to transfer messages. This cannot be automated by the bot.
{% endhint %}

Don't miss new events when following the new \#🦆duckhunt-informations channel.

![These are autopublished directly to your channel](.gitbook/assets/messages-sent-in-the-informations-channel.png)

## More ducks

By using webhooks, we are able to reduce the pressure on DuckHunt, and as such, you can now set the `duck_per_day` higher than previously. Overall, you should be able to get twice as more ducks in a day compared to V3.

## Stable bot

This update should also make the bot more stable, with less reliance on caches, more detailed error messages, and less downtime.

By using intents, the bot will be faster to answer commands than the previous version, and should get overwhelmed less often.

## New commands

Some new commands like [me](https://duckhunt.me/commands/me), [shooting\_stats](https://duckhunt.me/commands/shooting_stats), [best\_times](https://duckhunt.me/commands/best_times), [kills\_stats](https://duckhunt.me/commands/kills_stats), and a lot more have been added to the bot. Will you be able to find them [all](https://duckhunt.me/commands) ?

## A complete API for developers

If you want to integrate your own bot with DuckHunt, it's easier than ever. You can go ahead and read the [DuckHunt API page](the-duckhunt-api/channels-scores-and-stats.md).

## Settings overhaul

{% hint style="success" %}
On V4, settings are **no longer defined per server**. Most of them can now be edited on a per-channel basis ! Good news if there are two or more Duckhunt channels in your server.
{% endhint %}

Many settings have been changed to facilitate a channel setup. Included are [settings presets](https://duckhunt.me/commands/settings/templates) used to configure a server very quickly.

Don't worry, your settings from V3 have been migrated, just like the scores of players on your channels.

### Players settings

Players can also set some preferences globally, like their preferred [language](https://duckhunt.me/commands/settings/my_language) or if they wish to be [pinged](https://duckhunt.me/commands/settings/ping) \(or not\) by messages sent to them by the bot.

## Improved translations

Translations have been improved, with native time formats and more. You can also see the available languages directly from Discord

![The translators command list all the languages you can get on the bot](.gitbook/assets/translators.png)

Of course, you can still [contribute to translations](players-guide/how-to-contribute-to-the-bot.md#translating-the-bot) if you desire.

