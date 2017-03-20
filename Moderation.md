Moderation is a [Module](https://github.com/Fabricio20/LewdWiki/wiki/Modules) that adds Moderation-Related features. (Bet you wouldn't guess!)

## Features
Current list of features available on this Module.
* Ban command (with Reason, Option to clear messages and to make a Silent ban).
* Prune command (Supports tagging users [Also supports silent mode]).
* Logging (Joins/Leaves/Bans/Errors etc..).
* Auto-Registration System (Auto add roles to users when they type something on a specific channel).

## Commands
| Command      | Description                                                       | Rank  |
|--------------|-------------------------------------------------------------------|-------|
| Ban          | Bans a user with given (or not) + optional deleting               | Admin |
| Prune/Censor | Clears the chat history (Up to 400 messages) and supports filters | Admin |
| Logs         | Enables Logging (Joins/Leaves/Bans/LewdErrors)                    | Admin |
| Register     | Configures an auto-registration system                            | Admin |
<hr>

### Welcome
**Description**: Provides a way to set a welcome message for new users.<br>
**Subcommands**: 
```java
- enable  : Enables this feature.
- disable : Disables this feature.
- show    : Shows your current settings for this feature.
- set     : Sets the message to send.
- channel : Sets the channel to send the message in.
- dm      : Enables/Disable sending the message in dms.
```
**Tutorials**:<br>
A) Setting the channel #welcome as the greeting channel.
```java
@LewdBot welcome channel #welcome
```
B) Setting the greeting message.
```java
@LewdBot welcome set Welcome {USER} to {GUILD}!
```
C) Enabling DM mode (Sends the message on DMs).
```java
@LewdBot welcome dm true
```