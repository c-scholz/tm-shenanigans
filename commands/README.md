# How to add commands

To add the commands to your Nightbot, copy them from the text file into the `Message` field of a new command you set up in your Nightbot dashboard under [`commands > custom`](https://nightbot.tv/commands/custom) or add them by using `!addcom ![commandname_with_no_spaces] [copied command code]`


# fact

**Usage** 

`!fact [fact number]`

Returns a random fact or a fact that matches the number in the given parameter.


# nickname

To use the command replace the following words in the command with the corresponding text.
Use `${name}` to display the name in the texts.
Only replace text inside the backticks ``` `TEXT_TO_REPLACE` ```.
| VARIABLE | value |
| --- | ---  |
| USER_MSG   | message that displays if user requesting themselves                         |            
| MSG        | default message that's returned when no user found                          |
| NAME_TEMPL | template text to display found examples                                     |


**Usage**

`!nickname [twitch_username]`

Returns a random nickname for the default STREAMER_NAME or given username. Will return a default sentence if name cant be found or user issueing the command is the same as the name from the default or param.


# at

To use the command replace `CAMPAIGN_ID` in the command code with a campaign's Id:

You can find the campaign Ids on [trackmania.io](https://trackmania.io/#/campaigns)

**Usage**

`!at [track_number]`

Returns the author time of the given track number of a campaign.
