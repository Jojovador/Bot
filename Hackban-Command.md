### The Hackban command
**Description**: The `hackban` command is used to quickly ban a set of users from their ids. Ideal for banning spambots.

**Usage**: `!hackban <id...>`

**Aliases**: `hackban`, `hakban`<br>
**Subcommands**: None (only params)

**Limitations**:<br>
Users will not be banned if:
- They are the guild owner
- They have the `BAN_MEMBERS` permission
- They have the `MOD_BAN` LewdBot permission
- They are LewdBot

### Examples:

**1 - Banning some known spambots**
```java
@LewdBot hackban 267591176461221889 267569377895776256 267572440228429825 271530557614194689
```
This would ban some user accounts that were being used by Spambots back in 2016.