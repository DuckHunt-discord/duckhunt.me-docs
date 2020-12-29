# Channels scores and stats

{% hint style="info" %}
You'll need to request an API key from Eyesofcreeper\#0001 to use the following endpoints.

It should be passed as a query parameter: `api-agent`
{% endhint %}

{% api-method method="get" host="https://duckhunt.api-d.com" path="/web/duckstats.php" %}
{% api-method-summary %}
Get a hunter score on a channel
{% endapi-method-summary %}

{% api-method-description %}
This endpoint gives you statistics on a specific user. You will get the more results by using this method.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="cid" type="integer" required=true %}
The channel ID where you want the user stats
{% endapi-method-parameter %}

{% api-method-parameter name="pid" type="integer" required=true %}
The Player ID of whom you want the stats of.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Player statistics successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "id": 2242,
    "id_": 138751484517941259,
    "name": "Eyesofcreeper#0001",
    "channel_id": 195260818215010304,
    "banned": 0,
    "confisque": 0,
    "dazzled": 0,
    "enrayee": 0,
    "mouille": 0,
    "sabotee": "-",
    "sand": 0,
    "exp": 1946,
    "lastGiveback": 1582632361,
    "trefle_exp": 2,
    "ap_ammo": 0,
    "balles": 2,
    "chargeurs": 4,
    "detecteurInfra": 1577976851,
    "detecteur_infra_shots_left": 6,
    "explosive_ammo": 1577977217,
    "graisse": 1574779167,
    "life_insurance": 0,
    "sight": 0,
    "silencieux": 1577976568,
    "sunglasses": 0,
    "trefle": 1577976542,
    "self_killing_shoots": 0,
    "shoots_almost_killed": 0,
    "shoots_frightened": 13,
    "shoots_harmed_duck": 38,
    "shoots_infrared_detector": 0,
    "shoots_jamming_weapon": 9,
    "shoots_no_duck": 31,
    "shoots_sabotaged": 7,
    "shoots_tried_while_wet": 0,
    "shoots_with_jammed_weapon": 8,
    "shoots_without_bullets": 76,
    "shoots_without_weapon": 1,
    "shoots_fired": 390,
    "shoots_missed": 99,
    "killed_ducks": 209,
    "killed_normal_ducks": 198,
    "killed_super_ducks": 8,
    "killed_baby_ducks": 1,
    "killed_mother_of_all_ducks": 1,
    "killed_mechanical_ducks": 0,
    "killed_players": 5,
    "best_time": 1.163198,
    "exp_won_with_clover": 192,
    "givebacks": 81,
    "life_insurence_rewards": 0,
    "reloads": 117,
    "reloads_without_chargers": 6,
    "trashFound": 11,
    "unneeded_reloads": 44,
    "used_exp": 0,
    "found_explosive_ammo": 1,
    "found_almost_empty_explosive_ammo": 3,
    "found_chargers": 1,
    "found_chargers_not_taken": 0,
    "found_bullets": 4,
    "found_bullets_not_taken": 0,
    "found_silencers": 1,
    "found_infrared_detectors": 2,
    "found_grease": 1,
    "murders": 0,
    "avatar_url": "https://cdn.discordapp.com/avatars/138751484517941259/a_7b8ab8ec5cc3f97198eb3ac85d65f292.gif?size=1024",
    "hugs": 3,
    "hugs_no_duck": 1,
    "hugged_baby_ducks": 2,
    "hugged_nohug_ducks": 1,
    "hugs_human": 2,
    "channel_name": "game-all-time",
    "badges": {
        "banned": 0,
        "no_weapon": false,
        "admin": true,
        "moderator": false,
        "translator": false,
        "bug_hunter": false,
        "proficient": false,
        "retired_staff": false,
        "partner": false,
        "donator": false,
        "enigma_event_winner_june_2018": false
    },
    "achievements": {
        "time_played_1": true,
        "time_played_2": true,
        "clueless": false,
        "scientist": false,
        "max_level": false,
        "cheater": false,
        "baby_lover": true,
        "murderer": false,
        "first_blood": true,
        "ducks_killed_1": true,
        "ducks_killed_2": true,
        "ducks_killed_3": false,
        "ducks_killed_4": false,
        "ducks_killed_5": false,
        "ducks_killed_6": false,
        "lucky_user": false
    }
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a user or a channel matching the parameters provided.
{% endapi-method-response-example-description %}

```
Player or channel not found!
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://duckhunt.api-d.com" path="/web/duckstats.php" %}
{% api-method-summary %}
Get scores for a channel
{% endapi-method-summary %}

{% api-method-description %}
Get the whole scoreboard for a channel
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="cid" type="integer" required=true %}
The channel ID you want the top scores for
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
This is the list of the players. It is ordered by the exp amount in the current implementation, but it might change in the future.
{% endapi-method-response-example-description %}

```javascript
{
    "players": [
        {
            "id": 2403,
            "id_": 193747774079107073,
            "name": "sos#5187",
            "channel_id": 6,
            "banned": 0,
            "confisque": 0,
            "dazzled": 0,
            "enrayee": 0,
            "mouille": 0,
            "sabotee": "-",
            "sand": 0,
            "exp": 288888,
            "lastGiveback": 1579682603,
            "trefle_exp": 1,
            "ap_ammo": 1528437831,
            "balles": 1,
            "chargeurs": 6,
            "detecteurInfra": 1579769004,
            "detecteur_infra_shots_left": 6,
            "explosive_ammo": 1543688355,
            "graisse": 1543586152,
            "life_insurance": 0,
            "sight": 0,
            "silencieux": 1543586600,
            "sunglasses": 1541260191,
            "trefle": 1543584466,
            "self_killing_shoots": 0,
            "shoots_almost_killed": 0,
            "shoots_frightened": 191,
            "shoots_harmed_duck": 2179,
            "shoots_infrared_detector": 67,
            "shoots_jamming_weapon": 324,
            "shoots_no_duck": 445,
            "shoots_sabotaged": 11,
            "shoots_tried_while_wet": 3,
            "shoots_with_jammed_weapon": 40,
            "shoots_without_bullets": 350,
            "shoots_without_weapon": 3,
            "shoots_fired": 30041,
            "shoots_missed": 460,
            "killed_ducks": 26766,
            "killed_normal_ducks": 24709,
            "killed_super_ducks": 1730,
            "killed_baby_ducks": 121,
            "killed_mother_of_all_ducks": 202,
            "killed_mechanical_ducks": 3,
            "killed_players": 25,
            "best_time": 0.264288,
            "exp_won_with_clover": 140676,
            "givebacks": 509,
            "life_insurence_rewards": 0,
            "reloads": 3244,
            "reloads_without_chargers": 316,
            "trashFound": 662,
            "unneeded_reloads": 239,
            "used_exp": 0,
            "found_explosive_ammo": 48,
            "found_almost_empty_explosive_ammo": 64,
            "found_chargers": 125,
            "found_chargers_not_taken": 2,
            "found_bullets": 153,
            "found_bullets_not_taken": 0,
            "found_silencers": 37,
            "found_infrared_detectors": 47,
            "found_grease": 97,
            "murders": 1,
            "avatar_url": "https://cdn.discordapp.com/avatars/193747774079107073/3708634b95d099722b44608c60426046.jpg?size=1024",
            "hugs": 298,
            "hugs_no_duck": 35,
            "hugged_baby_ducks": 279,
            "hugged_nohug_ducks": 19,
            "hugs_human": 0
        },
        // ... Many users like this
    ],
    "channel_name": "game-all-time",
    "channel_id": 195260818215010304,
    "total_normal_ducks": 217684,
    "total_super_ducks": 12051,
    "total_baby_ducks": 914,
    "total_moad_ducks": 1675,
    "total_mechanical_ducks": 42,
    "total_players_killed": 2345
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
The channel ID given is not stored in the database.
{% endapi-method-response-example-description %}

```
Channel not found!
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

