# Channels scores and stats

Si quelqu'un veut faire un tableau de bord ou quelque chose pour contrôler DuckHunt, il y a déjà quelques routes API. Elles renvoient toutes JSON ou HTTP404/403/500.

## **Routes**

* `/api/channels` \[Authentification globale requise\] Renvoie des informations sur tous les canaux activés sur le bot.
* `/api/channels/{channel_id}` \[Authentification requise\] Renvoie des informations sur le canal, comme les canards actuellement apparus.
* `/api/channels/{channel_id}/settings` \[Authentification requise\] Renvoie les paramètres du canal
* `/api/channels/{channel_id}/top` \[Pas d'authentification requise\) Renvoie les meilleurs scores \(tous les joueurs sur le canal et quelques informations sur les joueurs\).
* `/api/channels/{channel_id}/player/{player_id}` \[No authentication required\] Returns _all_ the data for a specific user
* `/api/help/commands` \[No authentication required\] Returns all the commands registered with the bot.
* `/api/status` \[No authentication required\] Returns the status of every shard the bot currently has connected to the gateway.
* `/api/stats` \[No authentication required\] Get some global statistics about the bot.

## **Authentication**

If you have one, pass the API key on the `Authorization` HTTP header.

Two types of keys exist :

* Channel specific keys, available with `dh!settings api_key`. They only work for a specific channel data.
* Global keys, that allow UNLIMITED access to every channel data. They are available on request with me.

API keys \(local or global\) are uuid4, and look like this : `d84af260-c806-4066-8387-1d5144b7fa72`

## Examples

### `/api/channels/`

```javascript
[
  {
    "channel_name": "abcdef",
    "channel_discord_id": 1234,
    "guild_discord_id": 5678,
    "guild_name": "zyklm",
    "prefix": "!",
    "vip": false,
    "language": "fr"
  }
]
```

Of course, you get a list entry for every channel the bot sees.

### `/api/channels/{channel_id}`

Without authentication:

```javascript
{
  "id": 1234,
  "name": "hunting-ducks",
  "authentication": false
}
```

When authenticated:

```javascript
{
  "id": 734880436789969000,
  "name": "testing",
  "authenticated": true,
  "ducks": [
    {
      "category": "normal",
      "spawned_at": 1606758060.786562,
      "spawned_for": 31.57122492790222,
      "lives_left": 1,
      "lives": 1,
      "webhook_parameters": {
        "avatar_url": "https://media.discordapp.net/attachments/734810933091762188/735596788408385750/PicsArt_07-22-03.38.37.png",
        "username": "A duck"
      }
    },
    {
      "category": "super",
      "spawned_at": 1606758064.417822,
      "spawned_for": 27.93997597694397,
      "lives_left": 6,
      "lives": 6,
      "webhook_parameters": {
        "avatar_url": "https://cdn.discordapp.com/emojis/436542355504627712.png",
        "username": "Big Duck"
      }
    },
    {
      "category": "armored",
      "spawned_at": 1606758068.249334,
      "spawned_for": 24.10846996307373,
      "lives_left": 4,
      "lives": 4,
      "webhook_parameters": {
        "avatar_url": "https://media.discordapp.net/attachments/737978240966066177/738378965294645289/armored_duck.png",
        "username": "Strong Duck"
      }
    },
    {
      "category": "ghost",
      "spawned_at": 1606758071.5668979,
      "spawned_for": 20.790913105010986,
      "lives_left": 1,
      "lives": 1,
      "webhook_parameters": {
        "avatar_url": "https://cdn.discordapp.com/attachments/737978240966066177/737978554754793524/ghost_duck1.png",
        "username": "Invisible Duck"
      }
    },
    {
      "category": "mechanical",
      "spawned_at": 1606758075.8841631,
      "spawned_for": 16.473657846450806,
      "lives_left": 1,
      "lives": 1,
      "webhook_parameters": {
        "avatar_url": "https://media.discordapp.net/attachments/734810933091762188/735596788408385750/PicsArt_07-22-03.38.37.png",
        "username": "A duck"
      },
      "creator": null
    },
    {
      "category": "prof",
      "spawned_at": 1606758079.162167,
      "spawned_for": 13.195664882659912,
      "lives_left": 1,
      "lives": 1,
      "webhook_parameters": {
        "avatar_url": "https://cdn.discordapp.com/emojis/436542355257163777.png",
        "username": "Pr. Duck"
      },
      "operation": "15 + 30",
      "answer": 45
    }
  ]
}
```

### `/api/channels/{channel_id}/settings`

TODO

### `/api/channels/{channel_id}/top`

```javascript
[
  {
    "user_id": "432975131032158210",
    "user_name": "No one",
    "user_discriminator": "8277",
    "member_access_level_override": 50,
    "experience": 1000000000000,
    "best_times": {},
    "killed": {},
    "killed_total": 0,
    "last_giveback": 1609712255.956109,
    "shooting_stats": {
      "missed": 1,
      "got_killed": 2,
      "bullets_used": 1,
      "shots_when_jammed": 2,
      "shots_jamming_weapon": 1
    }
  },
  {
    "user_id": "251996890369884161",
    "user_name": "Subtleknifewielder",
    "user_discriminator": "1927",
    "member_access_level_override": 500,
    "experience": 2147483654,
    "best_times": {
      "normal": 92.49768447875977
    },
    "killed": {
      "baby": 1,
      "super": 294,
      "normal": 2574
    },
    "killed_total": 2869,
    "last_giveback": 1612404799.824978,
    "shooting_stats": {
      "killed": 9,
      "missed": 184,
      "reloads": 601,
      "revives": 1,
      "got_killed": 1,
      "brains_eaten": 1,
      "bullets_used": 3429,
      "empty_reloads": 98,
      "shots_when_dead": 1,
      "shots_with_duck": 1,
      "unneeded_reloads": 131,
      "shots_when_jammed": 1,
      "shots_without_ducks": 39,
      "shots_jamming_weapon": 66,
      "shots_when_sabotaged": 4,
      "shots_when_confiscated": 1,
      "bonus_experience_earned": 15825,
      "max_brains_eaten_at_once": 1,
      "shots_stopped_by_detector": 6,
      "shots_with_empty_magazine": 102
    }
  }
]
```

### `/api/channels/{channel_id}/player/{user_id}`

```javascript
{
  "user_id": "432975131032158210",
  "user_name": "No one",
  "user_discriminator": "8277",
  "member_access_level_override": 50,
  "id": 186990,
  "shooting_stats": {
    "missed": 1,
    "got_killed": 2,
    "bullets_used": 1,
    "shots_when_jammed": 2,
    "shots_jamming_weapon": 1
  },
  "magazines": 2,
  "prestige_last_daily": 1609712255.956065,
  "experience": 1000000000000,
  "weapon_sabotaged_by_id": null,
  "spent_experience": 0,
  "bought_items": {},
  "bullets": 6,
  "resisted": {},
  "first_seen": 1609712255.956043,
  "last_giveback": 1609712255.956109,
  "stored_achievements": {},
  "prestige": 0,
  "prestige_dailies": 0,
  "best_times": {},
  "hugged": {
    "nothing": 1
  },
  "givebacks": 0,
  "channel_id": "195260313082265600",
  "member_id": 163310,
  "hurted": {},
  "active_powerups": {
    "wet": 0,
    "dead": 2,
    "sand": 0,
    "grease": 0,
    "jammed": 1,
    "confiscated": 0,
    "homing_bullets": 0
  },
  "found_items": {},
  "killed": {},
  "killed_total": 0,
  "frightened": {}
}
```

### `/api/help/commands`

```javascript
{
  "ping": {
    "name": "ping",
    "short_doc": "Check that the bot is online, give the latency between the bot and Discord servers.",
    "brief": null,
    "help": "Check that the bot is online, give the latency between the bot and Discord servers.",
    "usage": null,
    "aliases": [],
    "enabled": true,
    "description": "",
    "signature": "",
    "invoke_with": "ping"
  },
  "manage_bot": {
    "name": "manage_bot",
    "short_doc": "Manage the bot current state by starting and stopping ducks spawning, leaving, and planning ducks spawn for the",
    "brief": null,
    "help": "Manage the bot current state by starting and stopping ducks spawning, leaving, and planning ducks spawn for the\nday.\n\nThese commands do not use the translation system, and will always show in english",
    "usage": null,
    "aliases": [
      "bot_administration",
      "emergencies"
    ],
    "enabled": true,
    "description": "",
    "signature": "",
    "invoke_with": "manage_bot",
    "subcommands": {
      "update_event": {
        "name": "manage_bot update_event",
        "short_doc": "Force the current event to change, and reroll a new one.",
        "brief": null,
        "help": "Force the current event to change, and reroll a new one.",
        "usage": null,
        "aliases": [
          "event",
          "reroll_event",
          "change_event",
          "regen_event"
        ],
        "enabled": true,
        "description": "",
        "signature": "[force=True]",
        "invoke_with": "manage_bot update_event [force=True]"
      },
      "stop_spawns": {
        "name": "manage_bot stop_spawns",
        "short_doc": "Stop ducks from spawning immediately, everywhere. Ducks don't get removed from the planification,",
        "brief": null,
        "help": "Stop ducks from spawning immediately, everywhere. Ducks don't get removed from the planification,\nso once the stop is over, ducks will spawn more quickly than usual.\n\nDuck will still be able to leave, even if this lock is set.",
        "usage": null,
        "aliases": [
          "disable_spawns"
        ],
        "enabled": true,
        "description": "",
        "signature": "",
        "invoke_with": "manage_bot stop_spawns"
      },
      "give_trophy": {
        "name": "manage_bot give_trophy",
        "short_doc": "Congratulate an user giving him a trophy.",
        "brief": null,
        "help": "Congratulate an user giving him a trophy.",
        "usage": null,
        "aliases": [],
        "enabled": true,
        "description": "",
        "signature": "<trophy_key> <user> [value=True]",
        "invoke_with": "manage_bot give_trophy <trophy_key> <user> [value=True]"
      },
      "start_spawns": {
        "name": "manage_bot start_spawns",
        "short_doc": "Allow ducks spawning again, everywhere. Ducks will spawn more quickly than usual if a planification isn't done.",
        "brief": null,
        "help": "Allow ducks spawning again, everywhere. Ducks will spawn more quickly than usual if a planification isn't done.",
        "usage": null,
        "aliases": [
          "restart_spawns",
          "enable_spawns"
        ],
        "enabled": true,
        "description": "",
        "signature": "",
        "invoke_with": "manage_bot start_spawns"
      },
      "force_boss_spawn": {
        "name": "manage_bot force_boss_spawn",
        "short_doc": "Force a boss to spawn",
        "brief": null,
        "help": "Force a boss to spawn",
        "usage": null,
        "aliases": [
          "spawn_boss",
          "boss",
          "boss_spawn"
        ],
        "enabled": true,
        "description": "",
        "signature": "",
        "invoke_with": "manage_bot force_boss_spawn"
      },
      "planify": {
        "name": "manage_bot planify",
        "short_doc": "Reset ducks planning, setting the ducks left to spawn counts to a value proportional to the time left spawning",
        "brief": null,
        "help": "Reset ducks planning, setting the ducks left to spawn counts to a value proportional to the time left spawning\nducks today. This is executed everyday at midnight.",
        "usage": null,
        "aliases": [
          "replan",
          "replanning",
          "replanify",
          "plan_spawns"
        ],
        "enabled": true,
        "description": "",
        "signature": "",
        "invoke_with": "manage_bot planify"
      }
    },
    "access_value": 500,
    "access_name": "BOT_MODERATOR"
  }
}
```

### `/api/status`

```javascript
{
  "bot_latency": 2.75,
  "shards_status": [
    {
      "shard_id": 0,
      "latency": 0.12,
      "ready": true,
      "guilds": [
        {
          "id": 1234,
          "name": "Whatever",
          "members": 99999
        }
      ]
    }
  ]
}
```

### `/api/stats`

```javascript
{
    "members_count": 1454404,
    "guilds_count": 14776,
    "channels_count": 487246,
    "players_count": 193477,
    "alive_ducks_count": 1234,
    "uptime": 1613427642,
    "current_event_name": "CALM",
    "current_event_value": [
        "Everything is calm",
        "Nothing is happening right now."
    ],
    "global_ready": true
}
```

Uptime here is the time the bot started, as a unix timestamp.

