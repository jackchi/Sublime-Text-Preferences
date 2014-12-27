# Sublime-Text-Preferences
I use Sublime Text for general-purpose configuration files editting. Scripting in Python. Etc. This README.md was composed in [dillinger.io](http://dillinger.io/)
## How to Configure
Under **Preferences** -> **Key Bindings- User** overrides the system defaults. 
*For MacOSX* Users -> "super" means the Apple(CMD) Key. 
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
## System Integration
Useful Sublime-Text-3 User Preferences and Keymappings
