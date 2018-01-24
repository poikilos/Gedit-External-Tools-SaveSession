# Gedit-External-Tools-SaveSession
Save and Restore sessions with Gedit (External Tools via hotkeys)

## Installation
* Requires:  **gedit-plugins**, **qarma** (or zentity) packages
* Download and install from the web:
```
mkdir -p ~/.config/gedit/tools
cd "$HOME/Downloads"
# cd ~/.config/gedit/tools
# git clone https://github.com/89luca89/Gedit-External-Tools-Session
# or
git clone https://github.com/expertmm/Gedit-External-Tools-SaveSession.git
cd Gedit-External-Tools-SaveSession
chmod +x install
./install
```
* restart gedit
* enable the **External-tools** plugin in menu button, Preferences, Plugins
* menu button, Manage External Tools
* click each "Session" plugin and set the hotkey (by clicking the blank hotkey field):
  * Session Save As: Ctrl Alt A (make a new session)
  * Session Save: Ctrl Alt S (Save using last saved or loaded session name)
  * Session Restore: Ctrl Alt R (restore named session by choosing session file from $HOME/.config/Gedit-Sessions
* Now you can enjoy this plugin! 

## Changes in expertmm Fork
(2018-01-23)
* Session is named with GUID in case of desktops (such as Xfce4) where zenity or qarma do not support the `--save` option (which silently fails and instead shows an open dialog) -- see also <https://github.com/luebking/qarma/issues/25>
* changed data folder from `$HOME/Projects/Gedit-Sessions` to `$HOME/.config/Gedit-Sessions`
* save most recent session file in $HOME/Projects/Gedit-Sessions/.current-name
* use quotes for all paths (replace ~ with $HOME since that changes is necessary in quotes)

## Screenshots

  `Ctrl+Alt+R will prompt to restore a session`

![photo_2016-12-10_19-11-18](https://cloud.githubusercontent.com/assets/598882/21075211/825b7d64-bf0c-11e6-8308-0ee638f4d52a.jpg)

`Ctrl+Alt+S will prompt to save a session (new or overwriting an existing one`


![photo_2016-12-10_19-10-49](https://cloud.githubusercontent.com/assets/598882/21075206/8240a82c-bf0c-11e6-94ce-c452ca17e9f7.jpg)
![photo_2016-12-10_19-11-02](https://cloud.githubusercontent.com/assets/598882/21075207/824812e2-bf0c-11e6-9b8f-60b02b36ca9c.jpg)
![photo_2016-12-10_19-11-08](https://cloud.githubusercontent.com/assets/598882/21075208/824e86cc-bf0c-11e6-858c-80ebe9ebc447.jpg)
![photo_2016-12-10_19-11-13](https://cloud.githubusercontent.com/assets/598882/21075209/8251fac8-bf0c-11e6-8af3-d503c1962d4c.jpg)
![photo_2016-12-10_19-11-15](https://cloud.githubusercontent.com/assets/598882/21075210/8256d778-bf0c-11e6-8146-a2235351639f.jpg)


You can also launch the action going to:
`Menu -> Tools -> External Tools`

![photo_2016-12-10_19-11-22](https://cloud.githubusercontent.com/assets/598882/21075212/82629766-bf0c-11e6-9689-a30716c968a8.jpg)

