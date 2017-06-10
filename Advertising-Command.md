### The Advertising command
**Description**: The `advertising` command is used to change how LewdBot reacts to people advertising guilds on your server.

**Usage**: `!advertising <allow/deny/ban>`

**Aliases**: `advertising`, `ads`<br>
**Subcommands**: None (only params)

**Limitations**:<br>
Users will not be banned/kicked if:
- They are the guild owner
- They are a guild admin
- They have the `MOD_ADVERTISE` permission
- They have the `MOD_SENDINVITE` LewdBot permission
- They are LewdBot

### Examples:

**1 - Advertising kick**
```java
@LewdBot advertising deny
```
This would kick and delete messages of users who try to advertise.

**2 - Advertising ban**
```java
@LewdBot advertising ban
```
This would ban users who try to advertise.

**3 - Reverting back to default**
```java
@LewdBot advertising allow
```
This would allow users to advertise on your server (default).