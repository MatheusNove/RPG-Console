# RPG-Console
This is a windows inspired console.


The project is set up to work on web, the MainScene.gd has a conversation with javescript.
It works great for web and cellphones. So far it has only been release on itch.io without plans to release in other platforms.

To use the console you have to create a resource with class name "Command" and put it in the exported array "CommandList" in the CommandReader node in the MainScene.tscn

Setting a command:
The resource needs the commandName so it can be triggered
The commandDescrip is the text that it will be shown after the command triggers
Image is optional. it will appear alaways after the text.
ErrorType is the type of error it will print if it has a flag
ActiveFlag is a flag that will activated when the command is trigger
PrevFlagRequire is the flag that needs to be active for the command to trigger otherwise the ErrorType will be triggered

Flags are resources as well, they can create just like Commands but they are a Flag
The node "FlagManager.tscn" is the one that activades them
