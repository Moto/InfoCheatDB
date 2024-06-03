# Windows 11 Tips & Fixes

## Removing Invalid Entries in the Add/Remove Programs Tool

> :warning: WARNING: If you use Registry Editor incorrectly, you may cause serious problems that may require you to reinstall your operating system. Microsoft cannot guarantee that you can solve problems that result from using Registry Editor incorrectly. Use Registry Editor at your own risk.

The following steps remove only the registry entries related to a program as it appears in the Add/Remove Programs tool. To completely uninstall a program that was not completely removed by clicking the Change/Remove button in the Add/Remove Programs tool, you need to clean up the physical directory structure on disk and in the registry also.

> :warning: Use extreme caution when you perform either of these tasks.

### To remove a program reference viewable in the Add/Remove Programs tool:


Start Registry Editor (Regedit.exe).

Locate the following key:

HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Uninstall​

OR​

All users​
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall

Locate the key to be deleted by locating the key name created by the program. If the name of the key is not apparent, browse through each key and note the value for DisplayName. This is the viewable string in the Add/Remove Programs tool.

Using the Registry menu, export the selected registry key to make a backup. Store the .reg file in a safe location in case you need to import it at a later date.

Delete the selected registry key and its values. 

> :warning: Do not delete the entire Uninstall key!

Quit Registry Editor.

Verify that the reference in the Add/Remove Programs tool is no longer visible.