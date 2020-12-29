# Quelques commandes utiles

{% hint style="warning" %}
**Ceci n'est pas une liste des commandes du bot.** C'est une liste de commandes qui pourraient vous être utiles sur le **serveur** de support Discord.
{% endhint %}

{% hint style="warning" %}
Pour une liste des commandes de DuckHunt, allez voir les pages : 

* [Les commandes administrateur](../bot-administration/admin-commands.md)
* [Les commandes du jeu](../players-guide/player-commands.md)[ ](../players-guide/player-commands.md)
{% endhint %}

Ce qui suit est uniquement un résumé des commandes les plus utiles. Pour plus d'information sur chaque bot, vous pouvez utiliser la commande`help`  du bot concerné.

{% hint style="success" %}
N'incluez **pas** les crochets comme &lt;&gt; ou \[ \]. Le &lt;&gt; indique un argument **obligatoire**, le \[ \] indique un argument **optionnel**.
{% endhint %}

### R. Danny \(Aide\)

R. Danny est principalement utilisé pour ses tags, qui permettent d'envoyer rapidement un message et de répondre aux questions fréquentes. 

| Command | Explanation |
| :--- | :--- |
| `?tag <tag name>` | Affiche le message `tag name`dans le canal utilisé. Les tags les plus utiles sont `wrong_channel_fr`, `setup_fr` et`manual_fr` |
| `?tag list` | Donne la liste de tous les tags. |
| `?tag make` | Vous permet de créer un tag. Commande interactive. |
| `?tag stats` | Affiche les tags les plus utilisés sur le serveur. |

R. Danny gère aussi le salon \#starboard . Pour l'utiliser, réagissez avec l'émoji ⭐️ sur un message que vous trouvez drôle. Si deux personnes réagissent avec ⭐️, le message sera conservé dans le starboard.

### Discord Pizza \(Fun\)

Ce bot vous permet de commander des pizzas \(virtuelles\), gratuitement. Les pizzas sont crées et livrées par de vrais humains, ceux qui restent obtiennent le rôle @Pizza.

| Commande | Explication |
| :--- | :--- |
| `(>order <votre commande>` | Commande une pizza. Votre commande peut être une pizza avec au plus 4 ingrédients. La pizza sera livrée dans le salon dans lequel vous avez passé la commande. |
| `(>myorder` | Vérifie l'avancement de votre commande. |
| `(>rules` | Vérifie les règles qui s'appliquent au bot et à la commande de pizzas. |

Si vous voyez un livreur, dites-lui qu'il est le bienvenu et qu'il peut rester sur le serveur, et qu'un modérateur lui donnera le rôle @Pizza dès que possible.

### Groovy \(Musique\)

Ahuman a dit prem's.

### Koishi \(Statistiques\)

| Commande | Explication |
| :--- | :--- |
| `b+histostatus` | Montre votre historique de statut heure par heure. |
| `b+histoguild` | Montre l'historique de toute la guilde. Prend longtemps à effectuer. |

### TeXiT \(Maths\)

TeXiT est utilisé pour les formules mathématiques. La syntaxe `$ inline LaTeX equation$` permet de mettre les équations en ligne, et la syntaxe `$$ equation $$` place les équations sur une ligne séparée du texte.

Il y a aussi quelques commandes utiles pour utiliser WolframAlpha et calculer.



| Commande | Explication |
| :--- | :--- |
| `,wolf <commande WA>` | Pose une question à WolframAlpha et retourne la première commande. Une question peut être n'importe quoi, de `2+2` à `Combien de calories dans un burger ?` |
| `,calc <expression>`  | Calcule quelques expressions mathématiques simples. |

### GetBeaned \(Modération\)

GetBeaned est notre bot de modération. Les commandes suivantes sont destinées aux modérateurs.

| Commande | Explication |
| :--- | :--- |
| `+ban <durée> {utilisateur} <raison>` | Bannit le ou les utilisateurs, avec un message optionnel donnant la raison. |
| `+softban {utilisateur} <raison>` | Bannit et débannit les utilisateurs, pour supprimer leurs messages récents. Vous pouvez ajouter une raison optionnelle. |
| `+kick {utilisateur} <raison>` | Éjecte les utilisateur du serveur. Ils pourront rejoindre de nouveau avec un lien d’invitation. |
| `+mute <durée> {utilisateur} <raison>` | Rend muet les utilisateurs sur le serveur. Ils ne pourront plus parler sans avoir été dé-mute ou quitté et rejoint de nouveau le serveur. |
| `+unmute {utilisateur_muet} <raison>` | Retire le rôle GetBeaned\_Muted aux utilisateurs, pour les laisser parler de nouveau. |
| `+unban {utilisateur_banni} <raison>` | Dé-bannit les utilisateur du serveur.  Ils pourront rejoindre de nouveau avec un lien d’invitation. |

Les commandes suivantes peuvent être utilisées par les modérateurs et les utilisateurs de confiance. 

| Commande | Explication |
| :--- | :--- |
| `+note {utilisateur} [raison]` | Ajoute une note au profil de l'utilisateur. N'a aucun effet, cette commande sert uniquement comme aide-mémoire pour le staff, ou bien pour les infractions vraiment mineures. |
| `+warn {utilisateur} <raison>` | Avertit les utilisateurs du serveur. Ne fait rien en lui-même, mais il y a des seuils qui s'appliquent sur les avertissements et peuvent causer l'éjection d'un utilisateur.  |
| `+snipe` | Récupère le dernier message supprimé d'un salon, utile si du spam sur un salon a été rapidement supprimé. |
| `+purge {arguments}` | Supprime un groupe de messages. Voir cette [page ](https://docs.getbeaned.me/bot-documentation/list-of-commands)pour plus d'informations. |
| `+rename [utilisateur] <surnom>` | Renomme un utilisateur. Si le surnom n'est pas spécifié, supprime le surnom. |
| `+inspect [utilisateur/message/salon/...]` | Donne des informations sur un ID ou un nom, et essaye de deviner de quoi il s'agit. |

Aucune de ces commandes ne sont destinées aux utilisateurs normaux.

### Autres bots

à faire  : GamesROB, Snail Racing \(Ahuman claims this one too\), Tatsu, FriendSpotter



