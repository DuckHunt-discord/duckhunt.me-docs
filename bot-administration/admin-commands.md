# Admin commands

Some commands are more complicated than others. In that case, they will be shown in bold and their arguments will be explained after this command list

| Command | Description |
| :--- | :--- |
| dh!setup | This is the first command you should use after inviting DuckHunt to a server. It create the server settings and have a configuration wizard to make it easier for you. |
| dh!add\_channel | After using dh!setup, use this command on the channels you want ducks to appear in. |
| dh!del\_channel | This disables a channel added by dh!add\_channel. |
| dh!del\_user | This removes an user from the database. |
| dh!del\_user\_id | This removes an user from the database. This comment is meant to be used on players that left the server. |
| dh!add\_admin | Set another server administrator as an admin. Note that users with the Administrator permission in discord are considered Administrators too. |
| dh!del\_admin | Deletes a server admin from the admins list. |
| **dh!coin** | Forces a duck to spawn. |
| dh!ducks | Shows the number of ducks that will spawn today, and the list of ducks that are on the channel. It can be considered as a cheat. |
| dh!give\_exp &lt;player&gt; &lt;amount&gt; | Gives a player some exp points. This is a cheat, not to be confused with dh!send\_exp. |
| **dh!settings set &lt;parameter&gt; &lt;value&gt;** | Modify server settings. You can go to the Bot Settings page to learn more about this command. |
| dh!settings reset &lt;parameter&gt; | Resets a parameter to the default value. Use this command and not dh!settings set to reset parameters, as it won’t cause issues with bot upgrades. |
| dh!game\_ban &lt;player&gt; | Bans a player from the game. You can’t ban admins, so please don’t try :\) |
| dh!game\_unban &lt;player&gt; | Unbans a player from the game. They will be able to play again. |
| dh!remove\_all\_scores\_and\_stats\_on\_this\_channel | Deletes a channel scores and stats. Please be sure you really want to do this. You cannot undo this. |

### The coin command

The coin command \(`dh!coin`\) will make a duck spawn in the current channel. Obviously, this can only be used in an enabled channel.

* `dh!coin` will spawn a simple, regular duck
* `dh!coin --super-duck --life 2` will spawn a super duck with 2 life points
* `dh!coin --moad --life 6` will spawn a MOAD with 6 life points
* `dh!coin --baby-duck` will spawn a baby duck

### The settings related command

List of settings and values you might use are described in more details on the [Edit Settings](edit-settings-settings-list.md) page.



