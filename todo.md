## [Changelog](https://novabros.github.io/NovaBot/version) | [To-Do](https://novabros.github.io/NovaBot/todo) | [Commands](https://novabros.github.io/NovaBot/commands)
## To-do

### Core Stuff
- Add logging
  - Commands, errors, autosaves, etc
- Proper `on_command` exception handling
- Format HelpFormatter
- Add `utils.permissions.py` to handle command checks across all plugins
- Add `permissions.json` to use as read/write for permissions across all plugins
- Change `__main__` to be mostly be a class so things like `send_cmd_help` are importable

### Mod Stuff
- `clear [NUM] <USER>` command, to clear NUM messages from optional USER
- `nbspeak [CHANNEL] [MESSAGE]` to speak as NovaBot
- Add `permissions.json` to handle special permissions, like TommyAuth

### Other Stuff
- `on_message` content checking, to find possible memes
- Riot API integration
  - Gambling on active games
- Integrate parsed `todo.md` into `n!todo`
- Recreate Tatsumaki score system
  - Make it do other fun stuff
- `remind <MESSAGE> [TIME]` to set remind timers
  - Use a bunch of regex to parse hours/minutes/seconds
  - `n!remind 5` should set a 5 minute timer
  - `n!remind 5s` should be 5 seconds
  - `n!remind 2h5m30` should be 2 hours 5 minutes 30 seconds
- Other RNG things
- `spell` for memespelling, like with pictures of other stuff or something
- Change `cookie` so that `cookie.json` is updated every 10-30 minutes, rather than on each `cookie` command
- Change `Tommy` so that `tommy.json` is updated every few hours, rather than on each `tommyadd` and `tommyremove` command

### Far Future
- Upgrade to rewrite branch
- Generate webpages to show user information (cookies, levels)
