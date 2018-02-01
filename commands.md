## [Changelog](https://novabros.github.io/NovaBot/version)
## [To-Do](https://novabros.github.io/NovaBot/todo)
## Commands  
Because of the way some of the commands are parsed, and how the help command works, it may be difficult to find the full functionality of a command.  
Commands will be listed here in much more detail.

### Syntax
Arguments wrapped in `[square brackets]` are required.  
Arguments wrapped in `<angle brackets>` are optional.
### Tommy
The Tommy plugin offers some commands to view and manage quotes from Tommy.  
All commands except for `tommy` are restricted to special TommyAuthorized users.

Command|Description
:-|:-
`tommy <ID>` | Returns a random Tommy quote, or a specific one if an ID number is given.
`tommylist`  | Returns a full list of Tommy quotes with their unique identifiers. The list self destructs after some time.
`tommyremove [ID]` | Removes a specific Tommy quote from the list.
`tommyadd <subject>|[quote]` | Adds a Tommy quote to the list, with optional `subject` header. Make sure to use a `| pipe` character to separate the subject if used.

### Fun
The Fun plugin has some fun tools and games that will probably be divided into separate projects at some point.

Command|Description
:-|:-
`strawpoll <title => [option1 | option2...]` | Create a strawpoll with optional title and a bunch of options. Identify title by putting an `= equals` sign after it, and separate options with `| pipe` characters. `n!strawpoll Favorite Color = Red | Blue | Green` works, and so does `n!strawpoll League of Legends | DotA 2 | World of Warcraft`.
`ship [person1] [person2]` | Find the shipping match between two people.
`cookie [person]` | Send a cookie to another person. This command is on a cooldown.
`cookiejar` | Take a gander at your cookie stash.

### Test
Test and debug commands for me and mods.

Command | Description
:-|:-
`members` | Get the member count of the current server.
`get_by_id` | Get a member by ID.
`get_by_name` | Get a member by name.
`ping [num] <buffer>` | Send `num` ping messages to the channel with `buffer` seconds in between each ping.
`_ret` | Prints a bundle of message information to the console.
`todo` | Embeds a link to the to-do list.
`commands <target>` | Embeds a link to the command page, at optional `target` anchor.
`version <version_code>` | Returns the current version and its changelog, as well as a link to the full changelog. If a specific version code is passed as the argument, it returns that version. Get version codes with `versions`. Get future versions with `new`, `future`,  `unreleased`, or `next`.
`versions` | List versions for use in `version` command.
