# How to add commands

To add the commands to your Nightbot, copy them from the text file into the `Message` field of a new command you set up in your Nightbot dashboard under [`commands > custom`](https://nightbot.tv/commands/custom) or add them by using `!addcom ![commandname_with_no_spaces] [copied command code]`


# fact

**Usage** 

`!fact [fact number]`

Returns a random fact or a fact that matches the number in the given parameter.

> Note:
> If you want to contribute a fact to be publicly available create a Pull Request with the change in the [facts.json](https://github.com/c-scholz/tm-shenanigans/blob/master/facts.json) file.


# nickname

To use the command replace the following keywords in the command with the corresponding values.
Use `${name}` to display the name in the texts.
Only replace text inside the backticks ``` `TEXT_TO_REPLACE` ```.
| VARIABLE | value |
| --- | ---  |
| USER_MSG   | message that displays if user requesting themselves                         |            
| MSG        | default message that's returned when no user found                          |
| NAME_TEMPL | template text to display found examples                                     |


**Usage**

`!nickname [twitch_username]`

Returns a random nickname of the issued user. If the user has no nickname returns a default message. If user issueing the command is the user that's requested it returns a user message.

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
| PLAYER_ID  | player uid that can be found at the end of the URL of your own Trackmania.io profile page |            
| PLAYER     | Player name                                                                               |

**Usage**

`!rank`

Returns the Matchmaking rank of the player set in the command.

# bonk

To use the command replace `PLAYER` in the command code with the Streamer's name.

**Usage**

`!bonk`

Returns a message with a counter.
