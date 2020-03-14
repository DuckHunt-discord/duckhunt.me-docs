# Useful commands

{% hint style="warning" %}
**This is not a command list for the DuckHunt bot.**  
This is a list of commands you might want to know when interacting on the DuckHunt **Support** Server.

For a list of duckhunt commands, please read

* [The admin commands](../bot-administration/admin-commands.md)
* [The player commands ](../players-guide/player-commands.md)
{% endhint %}

The following is only an overview of the commands we find to be the most useful. For more information about them, feel free to run the `help`command for the respective bot.

{% hint style="success" %}
Do **not** include brackets like &lt;&gt; or \[\] in the commands. A &lt;&gt; bracket mention a **required** argument, and \[\] brackets refer to **optional** arguments.
{% endhint %}

### R. Danny \(Support\)

R. Danny is mainly used for tags, to quickly send a message for an often asked question, a formula or many others.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Explanation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>?tag &lt;tag name&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Displays the <code>tag name</code>in the current channel.</p>
        <p>Useful tags include <code>wrong_channel</code>, <code>setup</code> and <code>manual</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>?tag list</code>
      </td>
      <td style="text-align:left">Lists every tag currently available.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>?tag make</code>
      </td>
      <td style="text-align:left">Lets you create a tag. This is an interactive command.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>?tag stats</code>
      </td>
      <td style="text-align:left">Displays the most-used tags on the server.</td>
    </tr>
  </tbody>
</table>R. Danny also manage the \#starboard channel. To use it, react with a ⭐️ on a message you find funny. If two people react with ⭐️, the message will be kept on the starboard.

### Discord Pizza \(Fun\)

This bot allow you to order \(virtual\) pizzas 🍕, for free. Pizzas are made and delivered by real humans \(those who decide to stay get the @Pizza role\).

| Command | Explanation |
| :--- | :--- |
| `(>order <your order>` | Order a pizza. Your order can be a pizza with at most 4 ingredients. The pizza will be delivered in the channel where you ran the command. |
| `(>myorder` | Check your order status. |
| `(>rules` | Check the rules that apply to pizza orders. |

If you see a deliverer, please tell him **he is welcome to stay** on the server. Tell him a moderator will be there soon to give them the pizza role.

### Groovy \(Music\)

Ahuman calls dibs

### Koishi \(Statistics\)

| Command | Explanation |
| :--- | :--- |
| `b+histostatus` | Show your status history by hour of the day. |
| `b+histoguild` | Show status history for the whole guild. Takes a long time to run. |

### TeXiT \(Math\)

TeXiT is used to render math formulaes. Use the `$ inline LaTeX equation$` syntax for inline equations and `$$ equation $$` to place equations on their own line.

There is also a few useful commands to query WolframAlpha and calculate 

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Explanation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>,wolf &lt;wolfram alpha query&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Query WolframAlpha and return the first result.</p>
        <p>A query can be anything from <code>2+2</code> to <code>how many calories in a burger</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>,calc &lt;expression&gt;</code> 
      </td>
      <td style="text-align:left">Calculate some simple math.</td>
    </tr>
  </tbody>
</table>### GetBeaned \(Moderation\)

GetBeaned is our moderation bot. The follwing commands are to be used by moderators.

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
| `+warn {users} <reason>` | Warns users on the server. While warns by themselves don't do anything, thresholds apply to warns and users may get kicked if they reach it. |
| `+snipe` | Recover the last deleted message from the channel. Useful if you had seen some spam on the channel that quickly got deleted. |
| `+purge {arguments}` | Remove messages in bulk. See the [command documentation](https://docs.getbeaned.me/bot-documentation/using-the-purge-command-to-remove-messages) for more information. |
| `+rename [user] <nickname>` | Rename a user with an optional nickname. If nickname is not specified, removes the nickname |
| `+inspect [user/message/channel/...]` | Provides information about a given ID or name, and try to guess what that object is. |

No commands here are meant to be used regularly by normal users.

### Other bots

TODO \(GamesROB, Snail Racing \(Ahuman claims this one too\), Tatsu, FriendSpotter\)



