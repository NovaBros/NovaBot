## [Changelog](https://novabros.github.io/NovaBot/version)
## To-do

### Core Stuff
- [ ] Upgrade to rewrite branch
  - It's gonna be a bitch
- [ ] Add logging
  - Commands, errors, autosaves, etc
- [ ] Proper `on_command` exception handling
- [ ] Format HelpFormatter

### Mod Stuff
- [ ] `clear [NUM] <USER>` command, to clear NUM messages from optional USER
- [ ] `nbspeak [CHANNEL] [MESSAGE]` to speak as NovaBot

### Other Stuff
- [ ] `on_message` content checking, to find possible memes
- [ ] Riot API integration
  - Gambling on active games
- [ ] Integrate parsed `todo.md` into `n!todo`
- [ ] Recreate Tatsumaki score system
  - Make it do other fun stuff
- [ ] `remind <MESSAGE> [TIME]` to set remind timers
  - Use a bunch of regex to parse hours/minutes/seconds
  - `n!remind 5` should set a 5 minute timer
  - `n!remind 5s` should be 5 seconds
  - `n!remind 2h5m30` should be 2 hours 5 minutes 30 seconds
- [ ] `roll [X] [Y]` to roll an X-sided die Y times
- [ ] Other RNG things
- [ ] `spell` for memespelling, like with pictures of other stuff or something
- [ ] Change `cookie` so that `cookie.json` is updated every 10-30 minutes, rather than on each `cookie` command
- [ ] Change `Tommy` so that `tommy.json` is updated every few hours, rather than on each `tommyadd` and `tommyremove` command
