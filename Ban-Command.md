### The Ban command
**Description**: The `ban` command is used to quickly ban users directly from chat. It currently supports mass bans by @ing users or by using a regex pattern, it also supports giving a reason which will be added to the audit logs.

**Usage**: `!ban <user|/pattern/|@user...> [reason]`

**Aliases**: None<br>
**Subcommands**: None (only params)

**Limitations**:<br>
Users will not be banned if:
- They are the guild owner
- They have the `BAN_MEMBERS` permission
- They have the `MOD_BAN` LewdBot permission
- They are LewdBot

### Examples:

**1 - Banning a user by name**<br>
```java
@LewdBot ban Fabricio20
```
This would simply ban Fabricio20 from the server (pls don't).

**2- Banning a user by name with a reason**<br>
```java
@LewdBot ban Fabricio20 Liking ducks
```
This would ban Fabricio20 because he likes ducks (Will add `Liking ducks` to audit logs)

**3 - Banning a set of users by mention**<br>
```java
@LewdBot ban @Fabricio20 @spong
```
This would simply ban Fabricio20 and Spong.<br>
**Note**: This variation (mention) does not support a reason.

**4 - Banning a set of users by regex**<br>
```java
@LewdBot ban "/\d/"
```
This would ban all users with a number in their name.<br>
```java
@LewdBot ban "/\d/" Having a number
```
Once again, bans all users with a number in their name, but with the `Having a number` reason.