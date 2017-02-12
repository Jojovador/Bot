## Introduction
As of LewdBot `5.2_192` a new permission system was introduced, it's purpose is to allow server owners to permit or deny users from using certain features on a per-role basis.

**Important**: LewdBot has a built-in override system for the permissions, Guild Owners and LewdBot-Admins will be exempt from these permission checks.

**Names used on this page and their special meanings**:<br>
* Allow  -> Allowing a permission, by setting it's status to true.
* Deny   -> Denying a permission, by setting it's status to false.
* Revoke -> Removing a permission by deleting it from the list of permissions.

## Commands and Usage
The new permissions system can be configured by using a set of subcommands. Below are a series of examples on how to use those subcommands.<br>
These examples assume the prefix on your guild is `!`, if this isn't the case, adapt your commands as needed.<br>

### Getting a role's permission
```java
!perms get ROLENAME
```
With the `get` subcommand you can get a list of permissions a role has and their statuses (denied/allowed).

### Adding permissions to a role
```java
!perms add ROLENAME PERMISSIONAME
!perms add ROLENAME PERMISSIONAME PERMISSIONAME ...
```
With the `add` subcommand you can add (allow) a permission or an array of permissions to a role.

### Removing permissions from a role
```java
!perms rem ROLENAME PERMISSIONAME
!perms rem ROLENAME PERMISSIONAME PERMISSIONAME ...
```
With the `remove` subcommand you can remove (deny) a permission or an array of permissions from a role.

### Setting a role's permission status
```java
!perms set ROLENAME PERMISSIONAME true
!perms set ROLENAME PERMISSIONAME false
```
With the `set` subcommand you can set the status of a permission on a role.

### Deleting a role's permission
```java
!perms del ROLENAME PERMISSIONAME
!perms del ROLENAME PERMISSIONAME PERMISSIONAME ...
```
With the `delete` subcommand you can revoke a permission or an array of permissions from a role.<br>
**Important**: The difference here (from remove) is that you are not negating the permission, instead, cleaning it out of the list of permissions (setting it's value to the default).

### Clearing all the permissions from a role.
```java
!perms clear ROLENAME
```
With the `clear` subcommand you can reset all the permissions (revoke but not deny) from a role.

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