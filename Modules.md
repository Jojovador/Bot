Modules are blocks of code packed into external "plug-ins" that work on a guild-basis, providing new features for guild owners and allowing them to completely control the behavior of LewdBot on their servers.

### List of Modules
| Name       | Description                                          | Default | Wiki Page                |
|------------|------------------------------------------------------|---------|--------------------------|
| Moderation | Provides Moderation tools (Like ban, logs, etc..)    | Enabled | [Moderation][moderation] |
| NSFW       | Provides NSFW content (ExHentai/E-Hentai/R34)        | Enabled | Link                     |
| Music      | Provides the ability to play music on voice channels | Enabled | Link                     |

### Settings
Settings are variables present on modules that users can change to customize how the module behaves. (For example translating success messages).

There are currently 4 types of variables:

| Name    | Description                     |
|---------|---------------------------------|
| String  | Text, no real restrictions      |
| Integer | Numbers that are not fractional |
| Double  | Numbers that _are_ fractional   |
| Boolean | Yes/No (true/false) values      |

To change such variables, you need to use the _set_ subcommand on the module command, for Example:<br>
`@LewdBot modules set Music CHATENABLED false`

[moderation]: https://github.com/Fabricio20/LewdWiki/wiki/Moderation