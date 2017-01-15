Moderation is a [Module](https://github.com/Fabricio20/LewdWiki/wiki/Modules) that adds Moderation-Related features. (Bet you wouldn't guess!)

## Features
Current list of features available on this Module.
* Ban command (with Reason, Option to clear messages and to make a Silent ban).
* Prune command (up to 400 messages at a time and supports tagging users [Also supports silent mode]).

## Commands
| Command      | Description                                                       | Rank  |
|--------------|-------------------------------------------------------------------|-------|
| Ban          | Bans a user with given (or not) + optional deleting               | Admin |
| Prune/Censor | Clears the chat history (Up to 400 messages) and supports filters | Admin |
| Logs         | Enables Logging (Joins/Leaves/Bans/LewdErrors)                    | Admin |
| Register     | Configures an auto-registration system                            | Admin |

## Settings
List of [settings](https://github.com/Fabricio20/LewdWiki/wiki/Modules#settings) that are added by this module.

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

**PRUNEMESSAGE**<br>
&nbsp; **Description**: The message sent to the chat when a prune command is executed.<br>
&nbsp; **Default**: ``Deleted `${Messages}` Messages.``<br>
&nbsp; **Modifiable**: Yes<br>
&nbsp; **Type**: String (Text)