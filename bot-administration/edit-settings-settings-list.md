---
description: still need to edit the comment
---

# Instellingen/ lijst van instellingen

Om een instelling aan te passen moet je `dh!settings set <paramter> <waarde>` gebruiken.

Je kunt de aangepaste instellingen zien met `dh!settings modified`  

Om een instelling te resetten, gebruik `dh!settings reset <parameter>`

<table>
  <thead>
    <tr>
      <th style="text-align:left">Parameter</th>
      <th style="text-align:left">Type</th>
      <th style="text-align:left">
        <p>standaard</p>
        <p>-waarde</p>
      </th>
      <th style="text-align:left">uitleg</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">announce_level_up</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Toggle the level up/down announcements</td>
    </tr>
    <tr>
      <td style="text-align:left">bang_lag</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">0.5</td>
      <td style="text-align:left">Time in seconds between a hunter&#x2019;s shot and what happens. This
        can be disabled by setting it to 0.</td>
    </tr>
    <tr>
      <td style="text-align:left">chance_to_kill_on_missed</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Probability in percent that a hunter will kill someone when missing a
        shot</td>
    </tr>
    <tr>
      <td style="text-align:left">clover_max_exp</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">10</td>
      <td style="text-align:left">Maximum experience bonus given by a clover</td>
    </tr>
    <tr>
      <td style="text-align:left">clover_min_exp</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Minimum experience bonus given by a clover</td>
    </tr>
    <tr>
      <td style="text-align:left">delete_commands</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Anti-flood parameter: delete commands from hunters after execution</td>
    </tr>
    <tr>
      <td style="text-align:left">disable_decoys_when_ducks_are_sleeping</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Make decoys ineffective when ducks are sleeping (see sleeping_ducks_start
        and sleeping_ducks_stop)</td>
    </tr>
    <tr>
      <td style="text-align:left">duck_frighten_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Probability in percent that a duck will get afraid and fly off when a
        hunter shoots at him.</td>
    </tr>
    <tr>
      <td style="text-align:left">ducks_per_day</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">48</td>
      <td style="text-align:left">Number of ducks that will spawn on a channel each day</td>
    </tr>
    <tr>
      <td style="text-align:left">emoji_used</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">:duck:</td>
      <td style="text-align:left">Emoji used by the bot if the emoji_ducks setting is enabled</td>
    </tr>
    <tr>
      <td style="text-align:left">exp_won_per_duck_killed</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">10</td>
      <td style="text-align:left">Experience points earned by a hunter per killed duck</td>
    </tr>
    <tr>
      <td style="text-align:left">killed_mentions</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Toggle mentioning people that get shot by other hunters. It can be annoying,
        so you can disable it here.</td>
    </tr>
    <tr>
      <td style="text-align:left">language</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">en_EN</td>
      <td style="text-align:left">Language used by the bot. Use the format 2letterslanguagecode_2LETTERSCOUNTRYCODE
        (<code>fr_FR</code>, <code>hu_HU</code>, <code>en_US</code>&#x2026;). If
        the language is not found, this will default to English.</td>
    </tr>
    <tr>
      <td style="text-align:left">mention_in_topscores</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Mention hunters in the topscores (this does NOT send notifications). It
        can break the scoreboard with long names.</td>
    </tr>
    <tr>
      <td style="text-align:left">multiplier_miss_chance</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Change the chance to miss on shooting. A lower value will make hunter
        miss less, a higher value will make hunter miss more.</td>
    </tr>
    <tr>
      <td style="text-align:left">pm_most_messages</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Send non-essential answers by PM to a hunter (reload, shop&#x2026;)</td>
    </tr>
    <tr>
      <td style="text-align:left">prefix</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">!</td>
      <td style="text-align:left">Prefix used by the bot. If DuckHunt commands conflict with another bot,
        you can change it here. Regardless of this setting, DuckHunt will always
        react to the prefix dh!</td>
    </tr>
    <tr>
      <td style="text-align:left">randomize_mechanical_ducks</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">3-level parameter. If it&#x2019;s set at 0, a mechanical duck will have
        a set look. If set to 1, his shout will get randomized. At 2, the mechanical
        duck will be indistinguishable from a normal one.</td>
    </tr>
    <tr>
      <td style="text-align:left">show_super_ducks_life</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Show super ducks life when they aren&#x2019;t killed</td>
    </tr>
    <tr>
      <td style="text-align:left">sleeping_ducks_start</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">Used with sleeping_ducks_stop to define an interval using military time
        hours (24h format) where the ducks won&#x2019;t spawn. The ducks_per_day
        setting will STILL be respected. You must only enter hours in UTC. Example
        : <code>dh!settings set sleeping_ducks_start 22</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">sleeping_ducks_stop</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">See sleeping_ducks_start. Example : <code>dh!settings set sleeping_ducks_stop 10</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">100</td>
      <td style="text-align:left">Probability that a duck that spawns will be a normal duck (this is a weighted
        probability system)</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Probability that a duck that spawns will be a super duck</td>
    </tr>
    <tr>
      <td style="text-align:left">baby_ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">2</td>
      <td style="text-align:left">Probability that a duck that spawns will be a baby duck</td>
    </tr>
    <tr>
      <td style="text-align:left">mother_of_all_ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Probability that a duck that spawns will be a mother of all ducks</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_exp_multiplier</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">1.1</td>
      <td style="text-align:left">To get experience earned when a hunter kill a superduck, we use the formula</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_maxlife</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">7</td>
      <td style="text-align:left">Maximum life of a super duck</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_minlife</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">3</td>
      <td style="text-align:left">Minimum life of a super duck</td>
    </tr>
    <tr>
      <td style="text-align:left">tax_on_user_give</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Percentage of exp that will be taken as a tax when a player uses the send_exp
        command. This can be disabled by setting it to 0.</td>
    </tr>
    <tr>
      <td style="text-align:left">time_before_ducks_leave</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">660</td>
      <td style="text-align:left">Time in seconds before a duck leaves of boredom if he isn&#x2019;t killed.</td>
    </tr>
    <tr>
      <td style="text-align:left">tts_ducks</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Try to speak when ducks appear. Experimental setting.</td>
    </tr>
    <tr>
      <td style="text-align:left">user_can_give_exp</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Allow users to send each other experience points with the send_exp command.</td>
    </tr>
    <tr>
      <td style="text-align:left">users_can_find_objects</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Allow users to find objects in bushes. Some objects are trash, some objects
        will benefit the hunter.</td>
    </tr>
  </tbody>
</table>