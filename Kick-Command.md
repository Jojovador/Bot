### The Ban command
**Description**: The `kick` command is used to quickly kick users directly from chat. It currently supports mass kicks by @ing users or by using a regex pattern, it also supports giving a reason which will be added to the audit logs.

**Usage**: `!kick <user|/pattern/|@user...> [reason]`

**Aliases**: None<br>
**Subcommands**: None (only params)

**Limitations**:<br>
Users will not be kicked if:
- They are the guild owner
- They have the `KICK_MEMBERS` permission
- They have the `MOD_KICK` LewdBot permission
- They are LewdBot

### Examples:

**1 - Kicking a user by name**<br>
```java
@LewdBot kick Fabricio20
```
This would simply kick Fabricio20 from the server (pls don't).

**2- Kicking a user by name with a reason**<br>
```java
@LewdBot kick Fabricio20 Liking ducks
```
This would kick Fabricio20 because he likes ducks (Will add `Liking ducks` to audit logs)

**3 - Kicking a set of users by mention**<br>
```java
@LewdBot kick @Fabricio20 @spong
```
This would simply kick Fabricio20 and Spong.<br>
**Note**: This variation (mention) does not support a reason.

**4 - Kicking a set of users by regex**<br>
```java
@LewdBot kick "/\d/"
```
This would kick all users with a number in their name.<br>
```java
@LewdBot kick "/\d/" Having a number
```
Once again, kicks all users with a number in their name, but with the `Having a number` reason.