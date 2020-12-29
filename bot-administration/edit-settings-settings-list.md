# Edit settings / Settings list

To set a setting, use `dh!settings set <parameter> <value>`

You can view modified settings by using `dh!settings modified`

For resetting a setting to its default value, use `dh!settings reset <parameter>`

Parameter                              | Type    | Default value | Comment
:------------------------------------- | :------ | :------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
announce_level_up                      | bool    | True          | Toggle the level up/down announcements
bang_lag                               | float   | 0.5           | Time in seconds between a hunter's shot and what happens. This can be disabled by setting it to 0.
chance_to_kill_on_missed               | integer | 5             | Probability in percent that a hunter will kill someone when missing a shot
clover_max_exp                         | integer | 10            | Maximum experience bonus given by a clover
clover_min_exp                         | integer | 1             | Minimum experience bonus given by a clover
delete_commands                        | bool    | False         | Anti-flood parameter: delete commands from hunters after execution
disable_decoys_when_ducks_are_sleeping | bool    | True          | Make decoys ineffective when ducks are sleeping (see sleeping_ducks_start and sleeping_ducks_stop)
duck_frighten_chance                   | integer | 5             | Probability in percent that a duck will be frightened and fly off when a hunter shoots at him
ducks_per_day                          | integer | 48            | Number of ducks that will spawn on a channel each day
emoji_used                             | string  | :duck:        | Emoji used by the bot if the emoji_ducks setting is enabled
exp_won_per_duck_killed                | integer | 10            | Experience points earned by a hunter per killed duck
killed_mentions                        | bool    | True          | Toggle mentioning people that get shot by other hunters. It can be annoying, so you can disable it here.
language                               | string  | en_EN         | Language used by the bot. Use the format 2letterslanguagecode_2LETTERSCOUNTRYCODE (`fr_FR`, `hu_HU`, `en_US`...). If the language is not found, this will default to English.
mention_in_topscores                   | bool    | False         | Mention hunters in the topscores (this does NOT send notifications). It can break the scoreboard with long names.
multiplier_miss_chance                 | float   | 1             | Change the chance to miss on shooting. A lower value will make hunter miss less, a higher value will make hunter miss more.
pm_most_messages                       | bool    | False         | Send non-essential answers by PM to a hunter (reload, shop...)
prefix                                 | string  | !             | Prefix used by the bot. If DuckHunt commands conflict with another bot, you can change it here. Regardless of this setting, DuckHunt will always react to the prefix dh!
randomize_mechanical_ducks             | integer | 0             | 3-level parameter. If it's set at 0, a mechanical duck will have a set look. If set to 1, his shout will get randomized. At 2, the mechanical duck will be indistinguishable from a normal one.
show_super_ducks_life                  | bool    | False         | Show super ducks life when they aren't killed
sleeping_ducks_start                   | integer | 0             | Used with sleeping_ducks_stop to define an interval using military time hours (24h format) where the ducks won't spawn. The ducks_per_day setting will STILL be respected. You must only enter hours in UTC. Example : `dh!settings set sleeping_ducks_start 22`
sleeping_ducks_stop                    | integer | 0             | See sleeping_ducks_start. Example : `dh!settings set sleeping_ducks_stop 10`
ducks_chance                           | integer | 100           | Probability that a duck that spawns will be a normal duck (this is a weighted probability system)
super_ducks_chance                     | integer | 5             | Probability that a duck that spawns will be a super duck
baby_ducks_chance                      | integer | 2             | Probability that a duck that spawns will be a baby duck
mother_of_all_ducks_chance             | integer | 1             | Probability that a duck that spawns will be a mother of all ducks
super_ducks_exp_multiplier             | float   | 1.1           | To get experience earned when a hunter kills a superduck, we use the formula $$rounded_integer(exp_won_per_duck_killed _super_ducks_exp_multiplier_ duck_life)$$
super_ducks_maxlife                    | integer | 7             | Maximum life of a super duck
super_ducks_minlife                    | integer | 3             | Minimum life of a super duck
tax_on_user_give                       | integer | 5             | Percentage of exp that will be taken as a tax when a player uses the send_exp command. This can be disabled by setting it to 0.
time_before_ducks_leave                | integer | 660           | Time in seconds before a duck leaves out of boredom if he isn't killed.
tts_ducks                              | bool    | False         | Try to speak when ducks appear. Experimental setting.
user_can_give_exp                      | bool    | True          | Allow users to send each other experience points with the send_exp command.
users_can_find_objects                 | bool    | True          | Allow users to find objects in bushes. Some objects are trash, some objects will benefit the hunter.
