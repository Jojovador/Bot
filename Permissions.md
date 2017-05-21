## Introduction
As of LewdBot `5.2_192` a new permission system was introduced, it's purpose is to allow server owners to permit or deny users from using certain features on a per-role basis.

**Important**: LewdBot has a built-in override system for the permissions, Guild Owners and LewdBot-Admins will be exempt from these permission checks.

## Commands and Usage
The new permissions system can be configured by using a set of subcommands. Below are a series of examples on how to use those subcommands.<br>
These examples assume the prefix on your guild is `!`, if this isn't the case, adapt your commands as needed.<br>

### Getting a role's permission
```java
!perms get ROLENAME
```
With the `get` subcommand you can get a list of permissions a role has and their statuses (denied/allowed).

### Resetting a role's permission
```java
!perms reset ROLENAME
```
With the `reset` subcommand you can reset a role's set of permissions (remove all of them) without having to do perm by perm.

### Clearing a role of a permission
```java
!perms clear ROLENAME PERMISSION
```
With the `clear` subcommand you can remove the state of a permission from a role (goes back to default value).

### Setting a permission for a role
```java
!perms set ROLENAME PERMISSION VALUE
```
This is the most important command, with it you will be able to set the state of a permission for a role, which means allow it or deny it (If you want to reset the state to default, check the clear command ^).<br>
**PS**: Value should be either `allow` or `deny`;

## List of Permissions
```java
MANAGE_PERMISSIONS - To manage the permissions for all roles (use the !perms command)

MUSIC_CONNECT - To summon LewdBot
MUSIC_PLAY    - To make LewdBot play
MUSIC_PAUSE   - To make LewdBot pause
MUSIC_ADD     - To add a song to the queue
MUSIC_REMOVE  - To remove a song from the queue
MUSIC_CLEAR   - To clear the queue
MUSIC_LOCK    - To lock the queue [Future]
MUSIC_SHUFFLE - To shuffle the playlist
MUSIC_LIST    - To list the musics in the queue
MUSIC_VIP     - To toggle vip mode
MUSIC_CHAT    - To set the music chat

MOD_KICK      - For kicking users (Default: False)
MOD_BAN       - For banning users (Default: False)
MOD_PREFIX    - For changing the prefix (Default: False)
MOD_SETUP     - For using the setup (Default: False)
MOD_LOGS      - For managing logs (Default: False)
MOD_RAID      - For activating raid mode (Default: False) [Future]
MOD_SENDINVITE - For sending invites (Default: False) [Future]
MOD_WELCOME   - For the welcome command  (Default: False)
MOD_MODULES   - For the modules command (Default: False)
MOD_COLOR     - For the color command (Default: False)
MOD_IGNORE    - For the ignore command (Default: False)
MOD_PRUNE     - For the prune command (Default: False)
MOD_LOCK      - For the Lock command (Default: False)
MOD_REGISTER  - For the color command (Default: False)

FUN_CALC      - For the calc command (Default: True)
FUN_CHAT      - For the chat command (Default: True)
FUN_DEFINE    - For the define command (Default: True)
FUN_FLIP      - For the flip command (Default: True)
FUN_ROLL      - For the roll command (Default: True)
FUN_PROFILE   - For the profile command (Default: True)

NSFW_R34      - For the r34 command (Default: True)
```
## Groups of Permissions
These are used so you don't need to type all permissions.
```java
MODERATE     - All permissions starting with MOD_
MANAGE_MUSIC - All permissions starting with MUSIC_
LEWD         - All permissions starting with NSFW_
FUN          - All permissions starting with FUN_
```