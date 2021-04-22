# Commandes utiles

**Il ne s'agit pas d'une liste de commandes pour le bot DuckHunt.** 

Il s'agit d'une liste de commandes que vous pourriez vouloir connaître lorsque vous interagissez avec le serveur de **support** de DuckHunt.

Pour une liste des commandes de DuckHunt, veuillez consulter la [liste des commandes](https://duckhunt.me/commands).

Ce qui suit n'est qu'un aperçu des commandes que nous trouvons les plus utiles. Pour plus d'informations à leur sujet, n'hésitez pas à lancer la commande `help` du bot concerné.

{% hint style="success" %}
N'incluez **pas** de parenthèses comme &lt;&gt; ou \[\] dans les commandes. Une parenthèse &lt;&gt; mentionne un argument **obligatoire**, et les parenthèses \[\] font référence à des arguments **facultatifs**.
{% endhint %}

## R. Danny \(Support\)

R. Danny est principalement utilisé pour les tags afin d'envoyer rapidement un message pour une question souvent posée, une formule ou bien d'autres encore.

| Commande | Explication |
| :--- | :--- |
| `?tag <tag name>` | Affiche le `nom du tag` dans le canal actuel. Les tags utiles incluent `wrong_channel`, `setup` et `manual`. |
| `?tag list` | Répertorie touts les tags actuellement disponibles. |
| `?tag make` | Permet de créer un tag. Il s'agit d'une commande interactive. |

R. Danny gère également la chaîne \#starboard. Pour l'utiliser, réagissez avec une ⭐️ sur un message que vous trouvez drôle. Si cinq personnes réagissent avec une ⭐️, le message sera conservé sur le starboard.

## **Koishi \(Statistiques\)**

| Commande | Explication |
| :--- | :--- |
| `b+histostatus` | Affichez l'historique de votre statut par heure de la journée. |
| `b+histoguild` | Montre l'historique du statut pour toute la guilde. Prend beaucoup de temps pour fonctionner. |

## GetBeaned \(Modération\)

GetBeaned est notre bot de modération. Les commandes suivantes doivent être utilisées par les modérateurs.

| Commande | Explication |
| :--- | :--- |
| `+ban <duration> {users} <reason>` | Bannit les utilisateurs fournis dans la commande, avec une raison facultative. |
| `+softban {users} <reason>` | Bannit et débannit les utilisateurs donnés pour supprimer les messages récents qu'ils ont envoyés. Vous pouvez ajouter une raison à afficher. |
| `+kick {users} <reason>` | Expulse les utilisateurs désignés de votre serveur. Ils pourront se reconnecter en utilisant un nouveau lien d'invitation. |
| `+mute <duration> {users} <reason>` | Mute les utilisateurs désignés sur le serveur. Ils ne pourront pas parler jusqu'à ce qu'ils soient unmute ou jusqu'à ce qu'ils quittent et rejoignent le serveur à nouveau. |
| `+unmute {muted_users} <reason>` | Retire le rôle GetBeaned\_Muted des utilisateurs, pour leur permettre de parler à nouveau. |
| `+unban {banned_users} <reason>` | Débannit les utilisateurs de votre serveur. Ils pourront revenir en utilisant une nouvelle invitation. |

Les commandes suivantes peuvent être utilisées par les modérateurs et les personnes de confiance.

| Command | Explanation |
| :--- | :--- |
| `+note {users} [reason]` | Ajoute une simple note au profil de l'utilisateur. Cela ne fait rien en soi, et sert surtout de rappel pour le staff ou pour des infractions très mineures. |
| `+warn {users} <reason>` | Averti les utilisateurs sur le serveur. Alors que les avertissements en eux-mêmes ne font rien, des seuils s'appliquent aux avertissements, et les utilisateurs peuvent être expulsés s'ils les atteignent. |
| `+snipe` | Récupérer le dernier message supprimé du canal. Utile si vous avez vu des spams sur le canal qui ont été rapidement supprimés. |
| `+purge {arguments}` | Supprime les messages en vrac. Consultez la [documentation de la commande](https://docs.getbeaned.me/tutorials/using-the-purge-command-to-remove-messages) pour plus d'informations. |
| `+rename [user] <nickname>` | Renomme un utilisateur avec un surnom optionnel. Si le surnom n'est pas spécifié, supprime le surnom. |
| `+inspect [user/message/channel/...]` | Fournit des informations sur un ID ou un nom donné, et tente de deviner ce qu'est cet objet puis donne des informations à propos de celui-ci. |

Aucune commande ici n'est destinée à être utilisée par des utilisateurs normaux.

