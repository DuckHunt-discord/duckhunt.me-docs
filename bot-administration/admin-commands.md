# Admin commands

Some commands are more complicated than others. In that case, they'll be shown in bold and their arguments will be explained after this command list.

Command                                        | Description
:--------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------
dh!setup                                       | This is the first command you should use after inviting DuckHunt to a server. It creates the server settings and has a configuration wizard to make it easier for you.
dh!add_channel                                 | After using dh!setup, use this command on the channels you want ducks to appear in.
dh!del_channel                                 | This disables a channel added by dh!add_channel.
dh!del_user                                    | This removes a user from the database.
dh!del_user_id                                 | This removes a user from the database. This comment is meant to be used on players that left the server.
dh!add_admin                                   | Set another server administrator as an admin. Note that users with the Administrator permission in discord are considered Administrators too.
dh!del_admin                                   | Deletes a server admin from the admin list.
**dh!coin**                                    | Forces a duck to spawn.
dh!ducks                                       | Shows the number of ducks that will spawn today, and the list of ducks that are on the channel. It can be considered as a cheat.
dh!give_exp <player> <amount>                  | Gives a player some exp points. This is a cheat, not to be confused with dh!send_exp.
**dh!settings set <parameter> <value>**        | Modify server settings. You can go to the Bot Settings page to learn more about this command.
dh!settings reset <parameter>                  | Resets a parameter to the default value. Use this command and not dh!settings set to reset parameters, as it won't cause issues with bot upgrades.
dh!game_ban <player>                           | Bans a player from the game. You can't ban admins, so please don't try :)
dh!game_unban <player>                         | Unbans a player from the game. They will be able to play again.
dh!remove_all_scores_and_stats_on_this_channel | Deletes a channel's scores and stats. Please be sure you really want to do this. You cannot undo this.

## The coin command

The coin command (`dh!coin`) will make a duck spawn in the current channel. Obviously, this can only be used in an enabled channel.

- `dh!coin` will spawn a simple, regular duck
- `dh!coin --super-duck --life 2` will spawn a super duck with 2 life points
- `dh!coin --moad --life 6` will spawn a MOAD with 6 life points
- `dh!coin --baby-duck` will spawn a baby duck

## The settings related command

List of settings and values you might use are described in more details on the [Edit Settings](edit-settings-settings-list.md) page.
