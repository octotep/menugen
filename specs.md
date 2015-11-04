Specs
=====

Menu
----

- Name: The name of the menu, used for the back function
- Prompt Name (default: name): An alternative name for the prompt
- Numbered (default: true): Controls whether the items are numbered or not
- Auto-select (default: true): Controls whether the menu auto selects an only match
- Back (default: true): Controls whether menumaker generates a back menu option

- Source (default: static): Sets the source for generating the menu
	- if static, reads items from the menu array
	- if generated, used sourcecmd to generate items
- Sourcecmd: Used to generate menu options
- Menu: an associative array, used if the menu is static


Reserved Menu Names
-------------------

- main: The main menu, where the program starts
- setup: A section to initialize state and declare functions

Items
-----

- Name: the name to be printed
- Separated by comma
	- Menu name: The name of the next menu
	- Command: Name of the command to run on selection
		- $ROFIRESULT: The result of the current selection
