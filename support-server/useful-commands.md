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

R. Danny is mainly used for tags to quickly send a message for an often asked question, a formula or many others.

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
</table>

R. Danny also manages the \#starboard channel. To use it, react with a ⭐️ on a message you find funny. If two people react with ⭐️, the message will be kept on the starboard.

### Discord Pizza \(Fun\)

This bot allows you to order \(virtual\) pizzas 🍕, for free. Pizzas are made and delivered by real humans \(those who decide to stay get the @Pizza role\).

| Command | Explanation |
| :--- | :--- |
| `(>order <your order>` | Order a pizza. Your order can be a pizza with up to 4 ingredients. The pizza will be delivered in the channel where you ran the command. |
| `(>myorder` | Check your order status. |
| `(>rules` | Check the rules that apply to pizza orders. |

If you see a deliverer, please **tell them they are welcome to stay** on the server. Then tell them a moderator will be there soon to give them the pizza role.

### _Groovy \(Music\)_

### Groovy\#7254 \(Originally Marv\) is a music bot that I believe to be better than rhythm.

**Adding songs to your queue**

You can add songs to a queue by using the **play** command \(-play, -p\) or by using the **search** command \(-search, -s\)

To use play, name the song you would like to add to the queue, or provide a link to it. Examples: -play simpleflip's nightmare -p website.com/video

To use search, look up the song as you would on google. Groovy will then provide a list of search results from youtube. Examples: -search penguins screaming -s people screaming

To add a recording from your files, use -f -f \(and select an audio file from your files. Use this as if you wanted to post an image with -f as the message\)

**Managing your queue**

To view songs that had been added to the queue, use -q To remove a song from the q, use -r You can use -r \# to remove a song by their position in the queue, for example: -r 5 You can remove a song by typing out part of their name or the entire name, for example: -r shimmer To skip a song, use -skip or -n To skip backwards, use -b To jump to a song, use -j Jump would be used the same as remove. To move a song, use -m Use move with the position in the queue. For example: -m 11, 2 The song you are moving would be 11, you are moving it to the 2nd position in the queue

To loop the queue \(or a certain song\) use -l \(twice for the queue, a 3rd time to cancel the loop\)

**managing the song**

To pause a song, use -pause \(resume with -play\) To check what time you are at, use -np To fast forward, use -ff for example: -ff \(defaults to skipping 15s ahead\) -ff 20m 10s \(skips 20 minutes and 10 seconds ahead\)

To rewind, use -rw for example: -rw \(defaults to rewinding 15s\) -rw 20m 10s \(rewind 20 minutes and 10 seconds behind\)

To go to a certain part of the song, use -seek -seek 3m 10s \(this will bring you to the point of 3m and 10s in the song. \)Koishi \(Statistics\)

| Command | Explanation |
| :--- | :--- |
| `b+histostatus` | Show your status history by hour of the day. |
| `b+histoguild` | Show status history for the whole guild. Takes a long time to run. |

### TeXiT \(Math\)

TeXiT is used to render math formulas. Use the `$ inline LaTeX equation$` syntax for inline equations and `$$ equation $$` to place equations on their own line.

There are also a few useful commands to query WolframAlpha and calculate 

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
</table>

### GetBeaned \(Moderation\)

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
| `+warn {users} <reason>` | Warns users on the server. While warns by themselves don't do anything, thresholds apply to warns, and users may get kicked if they reach it. |
| `+snipe` | Recover the last deleted message from the channel. Useful if you had seen some spam on the channel that quickly got deleted. |
| `+purge {arguments}` | Remove messages in bulk. See the [command documentation](https://docs.getbeaned.me/bot-documentation/using-the-purge-command-to-remove-messages) for more information. |
| `+rename [user] <nickname>` | Rename a user with an optional nickname. If nickname is not specified, removes the nickname |
| `+inspect [user/message/channel/...]` | Provides information about a given ID or name, and tries to guess what that object is. |

No commands here are meant to be used regularly by normal users.

### Other bots

TODO \(GamesROB, Snail Racing \(Ahuman claims this one too\), Tatsu, FriendSpotter\)



Snail Racing - race snails

```text
            **How to race your snail:**
```

To start a race, use `!s start` _or_ `!s race`

-You cannot start a race while one is already started or waiting to start

The bot will default to start the race in 15s.

-You can change the time it takes for the race to began by specifying how long you want in the start command Ex: `!s race 10s`   
-You can only use 5-30. Anything below 5 or above 30 will automatically be put on the max or min Ex: !s race 100 \(The bot will set the time for 30s instead\)

Within this time, people are allowed to join the race using `!s enter`

-You cannot enter a race when it already began. You cannot enter a race you started. You can only join after !s `race`/`start` is used, and before the race begins.   
-An infinite amount of people can join a race, but the rewards for the win do not increase.

-If nobody joins your race, then you will automatically go against an A.I.

```text
       **Win?**
```

The chance at winning a race is random \(does not depend on level\)  
-In the event of a tie, the topmost player automatically wins. 

Whenever you win a race, you will gain 5 exp and a prize A prize is an item. To open your prize, use `!s open`   
-You may open all of your prizes by using `!s openall`. Please note that this will give you the **rupee value** of all of the prizes, not each individual one.   
     --A **rupee** is Snail Racing currency. Rupees will be mentioned later.  
 -You cannot steal someone's prize. To check all of your prizes, use `!s items`

Whenever you level up, you will receive a set amount of rupees for the level you achieved   
-To check your level, use `!s level`   
-To check the levelboard, use `!s levelboard`

```text
              **Why is it called a levelboard?**
```

There are 2 types of boards, there is the levelboard, and the **leaderboard**

The leaderboard is item specific. This is used to see who has the most of what item in the server Ex: `!s leaderboard crap`

```text
                  **What else are items good for??**
```

There are a few things you can do with your items:   
-You can accumulate them and see them in your inventory   
-You can `!s give` items Ex: `!s give rupee 400 (user)`   
-You can `!s buy` items \(with rupees\) Ex: `!s buy freshcrap 100`   
-You can `!s sell` items \(for rupees\) Ex: `!s sell freshcrap 100`   
     --You can also use `!s sellall` to get rid of all your items \(for rupees\)   
-You can also gamble with your items.  
  
**Gambling** You can bet your items by using `!s bet` Ex: `!s bet rupee 200` Ex: `!s bet crap`   
-The chance at winning a bet is 50/50. Bets are **not** dependent on races.   
    --One time I lost 9 times in a row \(lost 1 million~ rupees\) 

Say you bet 200 rupees:   
-If you win, you will gain 200 rupees   
-if you lose, you will lose 200 rupees   
  --You cannot go into negatives. You cannot bet more than you own. 

To check your gambling statistics, use `!s stats`

```text
 **I'm not reading all of this.** 
```

Use !s help -The bot will DM you a list of commands. If you need help on using them \(or you need them explained\), ping/DM `<@316788628476919808>` \(Ahuman\)  
  
That's about it! Here is a few tips below :\) 

-If you are trying to grind, use `!s race 5` to make the race start asap   
-Whenever you see someone typing, it would be nice to use `!s race 10`, as this gives them a chance to join the race if they want to. I do this, because I am **nice**   
-When betting, its statistically impossible to lose 9 times in a row. I like to bet a small amount, and when i lose i double it. that way when i do win the bet, i will get all my rupees back. after winning, i go back to the small amount   
_what?_   
Ex: `!s bet rupee 20` \(lose, -20\)  
`!s bet rupee 40` \(lose, -60\) `!s bet rupee 80` \(lose, -140\) `!s bet rupee 160` \(win, +20\) repeat if you are daring, try tripling your rupees instead of doubling. This provides more risk, but a higher return.  
-I still lost 9 times in a row.

