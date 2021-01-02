# What's new in DuckHunt V4 ?

DuckHunt V4 is a complete rewrite of the DuckHunt bot. As such, you can expect many changes, like new ducks, new events, better leveling, and more.

## New ducks

On V3 there used to be only a few types of ducks :

* The [MOAD](players-guide/types-of-ducks.md#moad-mother-of-all-ducks)
* The [Super Duck](players-guide/types-of-ducks.md#super-ducks)
* The [Mechanical Duck](players-guide/types-of-ducks.md#mechanical)
* The [Normal Duck](players-guide/types-of-ducks.md#normal-ducks)
* The [Baby Duck](players-guide/types-of-ducks.md#baby)

On V4, these ducks have been kept, and new ones have appeared :

* The [Armored Duck](players-guide/types-of-ducks.md#armored) \(resists shots\)
* The [Pr. Duck](players-guide/types-of-ducks.md#prof-pr-duck) \(needs maths\)
* The [Golden Duck](players-guide/types-of-ducks.md#golden) and the [Plastic Duck](players-guide/types-of-ducks.md#plastic) \(worth more and less experience\)
* The [Kamikaze Duck](players-guide/types-of-ducks.md#kamikaze) \(kill other ducks\)
* The [Ghost Duck](players-guide/types-of-ducks.md#ghost) \(don't send a spawn message\)
* Nightly Ducks, like the Night Duck and the Sleeping Duck

### The Duck Boss

Another type of duck is the Duck Boss. The Duck Boss appears on the \#genetically-modified-ducks channel on the DuckHunt Server only, but when killed gives everyone who contributed to the kill a "box of foie gras" they can use on any channel in the game.

## Design

{% hint style="info" %}
For the new design to work, DuckHunt will need the `manage_webhooks` permission on his channel. If you still see older-looking ducks, ask an admin to add the correct permission, and then to run the `dh!settings use_webhooks True`command.
{% endhint %}

Ducks are better designed with the power of webhooks: every duck now gets a custom avatar \(made by Calgeka - /kalʒɛka/\#5963\)

![Look at all the different avatars, names, and messages. From top to bottom : Normal, MOAD, Super, Armored](.gitbook/assets/webhooks-example.png)

## A brand-new website

DuckHunt website just got better. More stats are collected and shown to players on their personal webpages, including best times per type of ducks killed, and a lot more.

![Also featuring a dark theme](.gitbook/assets/new-graphs.png)

You'll also find the [list of commands](https://duckhunt.me/commands), good [documentation](https://duckhunt.me/docs/) made for V4, [live data](https://duckhunt.me) like the current event and the number of ducks overall, and also a [status page](https://duckhunt.me/status) used to check if the bot is healthy.

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

