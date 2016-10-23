Moderation is a [Module](https://github.com/Fabricio20/LewdWiki/wiki/Modules) that adds Moderation-Related features. (Bet you wouldn't guess!)

## Features
Current list of features available on this Module.
* Ban command (with Reason, Option to clear messages and to make a Silent ban).

## Commands
| Command    | Description                                          | Rank    |
|------------|------------------------------------------------------|---------|
| Ban        | Bans a user with given (or not) reason               | Admin   |

## Settings

**BANMESSAGEDM**<br>
&nbsp; **Description**: The ban message sent to the user when he gets banned.<br>
&nbsp; **Default**: ``You were banned from `${Guild}` by `${Admin}`. **Reason**: ${Message}``<br>
&nbsp; **Modifiable**: Yes<br>
&nbsp; **Type**: String (Text)

**BANMESSAGE**<br>
&nbsp; **Description**: The ban message sent to the chat when someone gets banned.<br>
&nbsp; **Default**: ``**${User}** was banned from the server by `${Admin}`. **Reason**: ${Message}``<br>
&nbsp; **Modifiable**: Yes<br>
&nbsp; **Type**: String (Text)
