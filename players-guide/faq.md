# FAQ

## Comment puis-je jouer ?

Le meilleur moyen est de lire notre [guide du joueur](players-quickstart.md).

## Comment installer le bot ?

Voir le [QuickStart pour les administrateurs](../bot-administration/admin-quickstart.md). N'oubliez pas d'activer le [canal](https://duckhunt.me/commands/settings/enabled) !

## Le bot ne fonctionne pas ?

Titres alternatifs : Il n'y a presque pas de commandes sur mon canal ?, La commande bang/reload ne fonctionne pas, Le bot reste silencieux.

Vous n'avez pas [activé](https://duckhunt.me/commands/settings/enabled) le canal, n'est-ce pas ? Vous devriez peut-être lire le guide de [démarrage rapide pour les administrateurs](../bot-administration/admin-quickstart.md).

## Puis-je voir le code source ?

Bien sûr que vous pouvez ! Rendez-vous sur [GitHub](https://github.com/DuckHunt-discord) pour le faire !

Le projet est séparé en plusieurs répositoires :

* La [documentation](https://github.com/DuckHunt-discord/duckhunt.me-docs) que vous êtes en train de lire \(des liens d'édition pour des pages spécifiques sont également disponibles dans la barre latérale\). Écrit en Markdown, très facile à éditer pour les débutants comme pour les experts.
* Le [bot](https://github.com/DuckHunt-discord/DHV4) lui-même, avec toutes les [commandes](https://duckhunt.me/commands), et l['API](../the-duckhunt-api/channels-scores-and-stats.md). Écrit en Python, en utilisant la bibliothèque discord.py.
* Le [site web](https://github.com/DuckHunt-discord/DHV4_Web), utilisé pour formater et afficher cette documentation, mais aussi pour rendre les pages de statistiques. Écrit avec Django, HTML&CSS, Jinja2, et une touche de JS.
* La [configuration docker](https://github.com/DuckHunt-discord/DuckHunt_Docker), qui lie tout cela ensemble et permet un déploiement facile du robot.

## Je veux héberger moi-même DuckHunt/je veux ma propre copie de DuckHunt. Comment puis-je le faire ?

Ce n'est clairement pas recommandé. Le bot officiel est le meilleur choix dans 99,9 % des cas. Notez qu'aucune assistance ne sera fournie pour les versions auto-hébergées et que vous devrez mettre à jour le robot en temps voulu. Toutefois, si vous voulez quand même l'essayer, la meilleure façon de procéder est d'utiliser les fichiers de [configuration de Docker](https://github.com/DuckHunt-discord/DuckHunt_Docker).

N'oubliez pas de prendre le rôle de [Selfhoster](../support-server/list-of-roles.md) sur le [serveur de support](https://discordapp.com/invite/2BksEkV) pour être informé des mises à jour importantes.

## J'ai trouvé un bug ! Où dois-je aller ?

Félicitations ! Vous pouvez vous rendre sur notre [serveur de support](https://discordapp.com/invite/2BksEkV) pour le signaler, ou ouvrir un [problème sur GitHub](https://github.com/DuckHunt-discord/DHV4/issues).

## J'ai une demande/suggestion de fonctionnalité !

Ce n'est pas vraiment une question, mais vous pouvez aller sur [GitHub](https://github.com/DuckHunt-discord/DHV4/issues) pour suggérer des choses ! Vous pouvez également utiliser le canal \#🙋suggestions sur le [serveur de support](https://duckhunt.me/support).

## Je t'aime !!!

Moi aussi ! ❤️

## Puis-je faire un don pour soutenir le développement du robot ?

Voir [cette page](how-to-contribute-to-the-bot.md) ! Merci 😁.

## Existe-t-il un moyen de simuler différents paramètres ?

Oui, il y en a un ! Steefgozercool\#6710 a créé une feuille de calcul Excel où vous pouvez simuler n'importe quelle combinaison de paramètres et de jeux pour voir ce qui arrive aux scores. Cliquez [ici](https://cdn.discordapp.com/attachments/262720111591292928/794993119304613958/Duckhunt_experience_calculator_DHV4_beta_NEW.xlsx) pour la télécharger.

