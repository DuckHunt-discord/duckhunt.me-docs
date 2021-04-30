# FAQ

## Comment puis-je jouer ?

Le meilleur moyen est de lire notre [guide du joueur](players-quickstart.md).

## Comment installer le bot ?

Voir le [QuickStart pour les administrateurs](../bot-administration/admin-quickstart.md). N'oubliez pas d'activer le [canal](https://duckhunt.me/commands/settings/enabled) !

## Le bot ne fonctionne pas ?

Titres alternatifs : Il n'y a presque pas de commandes sur mon canal ?, La commande bang/reload ne fonctionne pas, Le bot reste silencieux.

Vous n'avez pas [activé](https://duckhunt.me/commands/settings/enabled) le canal, n'est-ce pas ? Vous devriez peut-être lire le guide de [démarrage rapide pour les administrateurs](../bot-administration/admin-quickstart.md).

## Can I see the source code?

Sure you can! Head to [GitHub](https://github.com/DuckHunt-discord) for it!

The project is separated in a few repositories :

* The [documentation](https://github.com/DuckHunt-discord/duckhunt.me-docs) you are currently reading \(edits links for specific pages are also available on the sidebar\). Written in Markdown, very easy to edit for beginners and experts alike.
* The [bot](https://github.com/DuckHunt-discord/DHV4) itself, with all the [commands](https://duckhunt.me/commands), and the [API](../the-duckhunt-api/channels-scores-and-stats.md). Written in Python, using the discord.py library.
* The [website](https://github.com/DuckHunt-discord/DHV4_Web), used to format and display this documentation, but also to render statistics pages. Written using Django, HTML&CSS, Jinja2, and a touch of JS.
* The [docker config](https://github.com/DuckHunt-discord/DuckHunt_Docker), tying all of this together, and allowing for an easy deployment of the bot.

## I want to self-host DuckHunt/I want my own copy of DuckHunt. How do I do it?

This is clearly not recommended. The official bot is the best choice in 99.9% of the cases. Note that no support will be given for self-hosted versions, and you have to update the bot in a timely fashion. However, if you still want to try it, the best way to go ahead would be to use [the docker configuration files](https://github.com/DuckHunt-discord/DuckHunt_Docker).

Don't forget to claim the Selfhoster [role](../support-server/list-of-roles.md) on the [support server](https://discordapp.com/invite/2BksEkV) to be pinged for important updates.

## I found a bug! Where should I go?

Congratulations! You can go to [our support server](https://discordapp.com/invite/2BksEkV) to report it, or open an [issue on GitHub](https://github.com/DuckHunt-discord/DHV4/issues).

## I have a feature request/suggestion!

That's not really a question, but you can go to [GitHub](https://github.com/DuckHunt-discord/DHV4/issues) to suggest things! You can also use the \#🙋suggestions channel on the [support server](https://duckhunt.me/support).

## I love you!

Me too ! ❤️

## Can I donate to support the development of the bot ?

See [this page](how-to-contribute-to-the-bot.md)! Thanks 😁.

## Is there a way to simulate different settings ?

Yes there is ! Steefgozercool\#6710 made an Excel spreadsheet where you can simulate any combination of settings and plays to see what happens to scores. Click [here](https://cdn.discordapp.com/attachments/262720111591292928/794993119304613958/Duckhunt_experience_calculator_DHV4_beta_NEW.xlsx) to download it.

