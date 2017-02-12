## Introduction
As of LewdBot `5.2_192` a new permission system was introduced, it's purpose is to allow server owners to permit or deny users from using certain features on a per-role basis.

**Important**: LewdBot has a built-in override system for the permissions, Guild Owners and LewdBot-Admins will be exempt from these permission checks.

## Examples
Below are a series of examples aimed to teach you how to setup the new permissions system.<br>
These examples assume the prefix on your guild is `!`, if this isn't the case, adapt your commands as needed.<br>

### Example 1 - Music only for DJs
In this example we will set up permissions for a role called `DJ`, allowing it to fully manage music features. We are also going to remove music permissions from the default role.<br>
**Warning**: Before starting, make sure you have a role called `DJ`.

```java
!perms add DJ MANAGE_MUSIC
```
With this command, we add the MANAGE_MUSIC permission group to the DJ role, that way we don't have to type all music permissions.<br>

```java
!perms rem everyone MANAGE_MUSIC
```
With this command we remove all music-related permissions from the `everyone` role (Default role).

And that's it, now the role `DJ` is the only one who can use music features, you can now safely add that role to your fellow DJs and they will be able to manage your guild's music.

## List of Permissions

//TODO