## [Changelog](https://novabros.github.io/NovaBot/version) | [To-Do](https://novabros.github.io/NovaBot/todo) | [Commands](https://novabros.github.io/NovaBot/commands)
## Commands  
Because of the way some of the commands are parsed, and how the help command works, it may be difficult to find the full functionality of a command.  
Commands will be listed here in much more detail.

### Syntax
Arguments wrapped in `[square brackets]` are required.  
Arguments wrapped in `<angle brackets>` are optional.
These conventions are likely only true here.  
`help` commands may say something completely different, but they are not accurate (yet).

## Plugins
### Tommy
The Tommy plugin offers some commands to view and manage quotes from Tommy.  
All commands except for `tommy` are restricted to special TommyAuthorized users.

Command|Description
:-|:-
`tommy <ID>` | Returns a random Tommy quote, or a specific one if an ID number is given.
`tommy add <subject>|[quote]` | Adds a Tommy quote to the list, with optional `subject` header. Make sure to use a `| pipe` character to separate the subject if used.
`tommy list`  | Returns a full list of Tommy quotes with their unique identifiers. The list self destructs after some time.
`tommy remove [ID]` | Removes a specific Tommy quote from the list.

### Fun
The Fun plugin has some fun tools and games that will probably be divided into separate projects at some point.

Command|Description
:-|:-
`cookie [person]` | Send a cookie to another person. This command is on a cooldown.
`cookiejar` | Take a gander at your cookie stash.
`roll <sides> <dice>` | Roll a \<sides>-sided die \<dice> times and return the sum. Defaults to a single d20 roll.
`ship [person1] [person2]` | Find the shipping match between two people.
`strawpoll <title => [option1 | option2...]` | Create a strawpoll with optional title and a bunch of options. Identify title by putting an `= equals` sign after it, and separate options with `| pipe` characters. `n!strawpoll Favorite Color = Red | Blue | Green` works, and so does `n!strawpoll League of Legends | DotA 2 | World of Warcraft`.

### Test
Test and debug commands for me and mods.

Command | Description
:-|:-
`_ret` | Prints a bundle of message information to the console.
`commands <plugin>` | Embeds a link to the command page, at optional `plugin` anchor.
`get_by_id` | Get a member by ID.
`get_by_name` | Get a member by name.
`members` | Get the member count of the current server.
`ping [num] <buffer>` | Send `num` ping messages to the channel with `buffer` seconds in between each ping.
`todo` | Embeds a link to the to-do list.
`version <version_code>` | Returns the current version and its changelog, as well as a link to the full changelog. If a specific version code is passed as the argument, it returns that version. Get version codes with `versions`. Get future versions with `new`, `future`,  `unreleased`, or `next`.
`versions` | List versions for use in `version` command.
