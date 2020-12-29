# Channels scores and stats

If someone wants to do a dashboard or something to control DuckHunt, there are a few API routes already. They all return JSON or HTTP404/403/500.

### **Routes**

`/api/channels` \[Global Authentication required\] -&gt; Returns some information about all channels enabled on the bot.  
`/api/channels/{channel_id}` \[Authentication required\] -&gt; Returns information about the channel, like the ducks currently spawned.  
`/api/channels/{channel_id}/settings` \[Authentication required\] -&gt; Returns channel settings  
`/api/channels/{channel_id}/top` -&gt; \[No authentication required\] Returns the top scores \(all players on the channel and some info about players\)  
`/api/channels/{channel_id}/player/{player_id}` -&gt; \[No authentication required\] Returns _all_ the data for a specific user

### **Authentication**

If you have one, pass the API key on the Authorization HTTP header.

Two types of keys exist :

* Channel specific keys, available with `dh!settings api_key`. They only work for a specific channel data. 
* Global keys, that allow UNLIMITED access to every channel data. They are available on request with me.

API keys \(local or global\) are uuid4, and look like this : `d84af260-c806-4066-8387-1d5144b7fa72`

### Examples

#### `/api/channels/{channel_id}` 

```javascript
{
  "id": 734880436789969000,
  "name": "testing",
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

More to come

