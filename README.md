# Sublime-Text-Preferences
Useful Sublime-Text-3 User Preferences and Keymappings

Some of the best worlflows I'd have to say it's the "save on focus lost" and my keymap "cmd+delete" that deletes the entire line. Similar to Workflow in [IntelliJ IDEA](https://www.jetbrains.com/idea/)

Please send pull requests or suggestions. 

I use Sublime Text for general-purpose configuration files editting. Scripting in Python. Etc. This README.md was composed in [dillinger.io](http://dillinger.io/)

## How to Configure
Under **Preferences** -> **Key Bindings- User** overrides the system defaults. 
*For MacOSX* Users -> "super" means the Apple(CMD) Key. 

## Useful Preferences
Here's my **[User Preferences](Preferences.sublime-settings)**

```
// Saves the file when you lose focus
"save_on_focus_lost": true
```

## Useful Key Mappings
Here's my **[Default (OSX).sublime-keymap](Default.sublime-keymap)**
```
// Delete a line with cmd+delete
{ "keys": ["super+backspace"], "command": "run_macro_file", "args": {
    "file": "Packages/Default/Delete Line.sublime-macro"
}}
```
```
// Duplicate Line
{ "keys": ["super+d"], "command": "duplicate_line" }
```
```
// Expanding Selections
{ "keys": ["alt+up"], "command": "expand_selection", "args": {"to": "scope"} }
```
    
## Useful Packages
Here's my ** [Installed Packages](Package Control.sublime-settings) 
You can install packages with Shift+Cmd+P: Install Packge
+ Jedi - Python Autocompleter is awesome!
+ SideBarEnhancements is necessary
+ All Autocomplete will remember your history and complete based on those entries

## System Integration

To get your Terminal to recognize `subl` as a command you can create a symbolic link and put it on your path:

In Sublime Text 3:
```bash
sudo ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/bin/subl
```

In Sublime Text 2:
```bash
sudo ln -s "/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl" ~/bin/subl
```

