# win10script
This is the Ultimate Windows 10 Script from a creation from multiple debloat scripts and gists from github. Modified first by Chris Titus, then by William Sampson for Digital Storm to use.

## DS Additions

- ostweak.ps1 contains the command to run win10debloat from a file, rather than opening a powershell prompt first.
- Simply create a shortcut, set it to run as administrator, and add "powershell -f" to the start of the path the shortcut uses.

## Modifications
- Disabling most of Chris Titus's added programs.
- Turning off tweaks which may be too dangerous to ship to customers.

Comment any thing you don't want out... Example:

```
########## NOTE THE # SIGNS! These disable lines This example shows UACLow being set and Disabling SMB1
### Security Tweaks ###
	"SetUACLow",                  # "SetUACHigh",
	"DisableSMB1",                # "EnableSMB1",

########## NOW LETS SWAP THESE VALUES AND ENABLE SMB1 and Set UAC to HIGH
### Security Tweaks ###
	"SetUACHigh",
	"EnableSMB1",
```
