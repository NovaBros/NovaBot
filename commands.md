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

`tommy <ID>` returns a random Tommy quote, or a specific one if an ID number is given  
`tommylist` returns a full list of Tommy quotes with their unique identifiers. The list self destructs after some time.  
`tommyremove [ID]` removes a specific Tommy quote from the list  
`tommyadd <subject> | [quote]` adds a Tommy quote to the list, with optional `subject` header

Command | Description
:-|:-
`tommy <ID>` | Returns a random Tommy quote, or a specific one if an ID number is given.
`tommylist`  | Returns a full list of Tommy quotes with their unique identifiers. The list self destructs after some time.
`tommyremove [ID]` | Removes a specific Tommy quote from the list.
`tommyadd <subject>\|[quote]` | Adds a Tommy quote to the list, with optional `subject` header.
