# HaxBall Client
This a client for the HTML game [HaxBall](https://www.haxball.com/play), built with a custom build of [nativefier](https://github.com/nativefier/nativefier) in order for the browser extension [HaxBall All-in-one Tool](https://github.com/xenonsb/Haxball-Room-Extension) to be supported.

The app works on Windows, macOS and Linux, and is 64-bit only.

## Features
* Every feature of the All-in-one Tool, including
  * Auto-join
  * Room search
  * Kick/Ban quick buttons
  * Local mute
  * Hide chat toggle
  * **R** as a REC hotkey
  * Chat shortcuts\*
* Dedicated button to make the UI transparent
* Custom command-line (see below)
* Support for high refresh rate monitors (e.g. 144fps if you have a 144Hz monitor)

\* *these were originally featured in the All-in-one Tool, but given that they do not work in the client they have been rewritten from scratch (see below)*.

### Command-line
The horizontal bar on the top has two functions: **redirect you to a room** given its link and launch **custom commands**. 

#### Available commands
##### Shortcuts
Shortcuts let you type frequent commands/messages by expanding a shorter piece of text.
* `shortcut add A,B`
* `shortcut remove A`
* `shortcut list`

For example, you may be someone who often changes extrapolation and you'd prefer not to type the full command each time. To do so, you can create a new shortcut by entering in the command bar

`shortcut add /e,/extrapolation`

so that every time you type in the game chat `/e` you will instead get `/extrapolation`.
If you wish to remove it, you can then use

`shortcut remove /e`

This particular shortcut is included by the default in the client, but you can create whatever shortcut you want (even entire messages)!

##### Player Auth management
Your Player Auth is often used by headless rooms' admins to authenticate you or to save your in-game statistics. If you want to view your Public Auth or Private Key, or change the latter, type the commands
* `auth`
* `auth yournewprivatekey`

##### Extrapolation / Avatar
If you want to view/change your extrapolation/avatar without entering a room or opening the console, type in the command bar
* `extra`
* `extra newvalue`
* `avatar`
* `avatar newavatar`
* `clearavatar`

##### Client info
* `help`
* `info`
* `version`
* `changelog`

## How to build
*Coming soon!*
