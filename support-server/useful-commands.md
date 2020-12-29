# Useful commands

**This is not a command list for the DuckHunt bot.**  
This is a list of commands you might want to know when interacting on the DuckHunt **Support** Server.

For a list of DuckHunt commands, please see the [command list](https://duckhunt.me/commands).

The following is only an overview of the commands we find to be the most useful. For more information about them, feel free to run the `help`command for the respective bot.

{% hint style="success" %}
Do **not** include brackets like &lt;&gt; or \[\] in the commands. A &lt;&gt; bracket mention a **required** argument, and \[\] brackets refer to **optional** arguments.
{% endhint %}

## R. Danny \(Support\)

R. Danny is mainly used for tags to quickly send a message for an often asked question, a formula or many others.

| Command | Explanation |
| :--- | :--- |
| `?tag <tag name>` | Displays the `tag name`in the current channel. Useful tags include `wrong_channel`, `setup` and `manual`  |
| `?tag list` | Lists every tag currently available. |
| `?tag make` | Lets you create a tag. This is an interactive command. |

R. Danny also manages the \#starboard channel. To use it, react with a ⭐️ on a message you find funny. If two people react with ⭐️, the message will be kept on the starboard.

## **Koishi \(Statistics\)**

| Command | Explanation |
| :--- | :--- |
| `b+histostatus` | Show your status history by hour of the day. |
| `b+histoguild` | Show status history for the whole guild. Takes a long time to run. |

## GetBeaned \(Moderation\)

GetBeaned is our moderation bot. The following commands are to be used by moderators.

| Command | Explanation |
| :--- | :--- |
| `+ban <duration> {users} <reason>` | Ban the users provided in the command, with an optional reason. |
| `+softban {users} <reason>` | Ban and unban the users given to remove the recent messages they sent. You may add a reason to be displayed. |
| `+kick {users} <reason>` | Kick the users from your server. They will be able to rejoin using a new invite link. |
| `+mute <duration> {users} <reason>` | Mute users on the server. They won't be able to speak until unmuted or until they leave and rejoin the server. |
| `+unmute {muted_users} <reason>` | Remove the GetBeaned\_Muted role from users, to let them talk again. |
| `+unban {banned_users} <reason>` | Unban users from your server. They'll be able to rejoin using a new invite. |

The following commands can be used by moderators and trusted users.

| Command | Explanation |
| :--- | :--- |
| `+note {users} [reason]` | Add a simple note to the user profile. Doesn't do anything by itself, this mostly serves as a reminder from staff or for very minor infractions. |
| `+warn {users} <reason>` | Warns users on the server. While warns by themselves don't do anything, thresholds apply to warns, and users may get kicked if they reach it. |
| `+snipe` | Recover the last deleted message from the channel. Useful if you had seen some spam on the channel that quickly got deleted. |
| `+purge {arguments}` | Remove messages in bulk. See the [command documentation](https://docs.getbeaned.me/bot-documentation/using-the-purge-command-to-remove-messages) for more information. |
| `+rename [user] <nickname>` | Rename a user with an optional nickname. If nickname is not specified, removes the nickname |
| `+inspect [user/message/channel/...]` | Provides information about a given ID or name, and tries to guess what that object is. |

No commands here are meant to be used regularly by normal users.



