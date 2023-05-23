# How to add commands

To add the commands to your Nightbot, copy them from the corresponding text file above into the `Message` field of a new command you set up in your Nightbot dashboard under [`commands > custom`](https://nightbot.tv/commands/custom) or add them by using `!addcom [commandname_with_no_spaces] [copied command code]` in your chat.


# fishh
**Usage**

`fishh`

Returns a random emote based on a weight given in config.

**Config:**
```js
cfg = {
  max: number // total amount of lots - has to be more than all emote lots combined
  def: string // default emote on "bad draw"
  emotes: { // emotes
    key: // with given amount of lots
      string[] // list of emotes with this amount
  }
}
```

> Note:
> Recommended to use with `fishh` 7tv emote and the emotes from this set: [7tv](https://7tv.app/emote-sets/63c907d8dedb49b243838d89).
> Feel free to change to a completely different emote set.

# fact

**Usage** 

`!fact [fact number]`

Returns a random fact or a fact that matches the number in the given parameter.

> Note:
> If you want to contribute a fact to be publicly available create a Pull Request with the change in the [facts.json](https://github.com/c-scholz/tm-shenanigans/blob/master/facts.json) file.


# nickname

To use the command replace the following keywords in the command with the corresponding values.
Use `${name}` to display the name in the texts.
Only replace text **inside** the backticks ``` ` TEXT_TO_REPLACE ` ```.
| VARIABLE | value |
| --- | ---  |
| USER_MSG   | message that displays if user requesting themselves                         |            
| MSG        | default message that's returned when no user found                          |
| NAME_TEMPL | template text to display found examples                                     |


**Usage**

`!nickname [twitch_username]`

Returns a random nickname of the issued user. If the user has no nickname it returns a default message. If user issueing the command is the user that's requested it returns a user message.

> Note:
> If you want to contribute your nickname to be publicly available create a Pull Request with the change in the [nicknames.json](https://github.com/c-scholz/tm-shenanigans/blob/master/nicknames.json) file.


# at

To use the command replace `CAMPAIGN_ID` in the command code with an official campaign's Id.

You can find the campaign Ids on [trackmania.io](https://trackmania.io/#/campaigns)

> Note:
> You can also set the command up to use a club campaign.
> For this instead replace `https://trackmania.io/api/officialcampaign/CAMPAIGN_ID` with `https://trackmania.io/api/campaign/CAMPAIGN_ID`

**Usage**

`!at [track_number]`

Returns the author time of the given track number of a campaign.

# cotd

**Usage**

`!cotd`

Returns the current TOTD with AT. Tells when next 7pm COTD is or whether Qualification/Knockout stage is in progress.


# rank

To use the command replace the following keywords in the command with the corresponding values.

| VARIABLE | value |
| --- | ---  |
| PLAYER_ID  | player uid that can be found at the end of the URL of your own [trackmania.io](https://trackmania.io) profile page |         
| PLAYER     | Player name                                                                                                        |

**Usage**

`!rank`

Returns the Matchmaking rank of the player set in the command.

# bonk

To use the command replace `PLAYER` in the command code with the Streamer's name.

**Usage**

`!bonk`

Returns a message with a counter.

# medals

| VARIABLE | value |
| --- | --- |
| CAMPAIGN_URL | custom campaign URL for example `https://trackmania.io/api/campaign/33721/27523` |

**Usage**

!medals [track number]

Returns the Author and Gold Medal times of the queried track of the custom campaign.

> Note: Change the campaign id based on the API call of trackmania.io. `https://trackmania.io/#/campaigns/2080/32622` becomes `https://trackmania.io/api/campaign/2080/32622`.
