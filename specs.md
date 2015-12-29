Specs
=====

Menu
----

- Name: The name of the menu, used for the back function
- Prompt Name (default: name): An alternative name for the prompt
- Numbered (default: true): Controls whether the items are numbered or not
- Auto-select (default: false): Controls whether the menu auto selects an only match


Reserved Menu Names
-------------------

- main: The main menu, where the program starts
- setup: A section to initialize state and declare functions

Items
-----

- Name: the name to be printed
- Type: (internal to menumaker, not exposed in API)
	- can be either "back", "item", or "nop"
- Link: The next menu to navigate to
- Action: The action to run when the item is selected
	- $SELECTION: rofi's selected text, can be used in the action
