# UniEditor

What kind of editor do coders all over the world want most? It should be "I want to unify the syntax highlighting theme and the editing hotkey".

So everyone will think

- "Why is there no unified editor style"
- "How to form a unified editor style"
- "Why change an editor, need to draw for a long time, be familiar with hotkeys, and toss the theme"
- "I can't find my favorite topic in the new editor, so I have to study it for a long time."
- "For the theme I made, I changed an editor, but I couldn't find a way to import it"
- "I haven't used this editor for a while. I've forgotten what hotkeys to press when copying lines."


## Syntax highlighting theme unification

> Syntax highlighting topics is actually a subset of software topics.

- Choose an intermediate conversion format for a topic, such as XML.
- Provides a way to set the theme of the web page without the editor. For example, http://tmtheme-editor.herokuapp.com 。
- Various editors use plug-ins to convert XML settings into the format they need, so as to reproduce syntax and highlight topics.

## Edit hotkey unification

> Editing hotkeys is actually just a subset of software hotkeys.

- Hotkeys can be unified, because there are only common parts due to the differences in editor functions. Usually only Ctrl-C/V/X/Z/Y/F/H/G/N/O/S/W/Q/A.
- In view of different history and habits, the hotkeys of common functions will also form several styles.
- If the style can be reduced to 2-3, the memory cost of developers will be greatly reduced.
- VIM is a big man. It does not participate in such competition and continues to maintain.
- Draw a hotkey comparison list. In fact, it is found that a slight adjustment can form a basic consensus of style.

Let me first propose a set of common hotkeys:

Function | geany | gedit | vscode
--|--|--|--
\* Move Multiline Up/Down |`Alt`-`FN`- ⬆/⬇, `Alt`-`PageUp`/`PageDown`|`Alt`- ⬆/⬇|<- SAME
\* Duplicate Multiline |`Ctrl`-`d`|-|-
\* Delete Multiline |`Ctrl`-`k`|`Ctrl`-`d`|-
\* Copy/Cut Multiline |`shift`-`Ctrl`-`c`/`x`|-|-
Delete to the BOL / EOL |`shift`-`Ctrl`-`backspace`/`delete`| <-SAME|-
\* Toggle Multiline Comment |`Ctrl`-`e`| [`shift`-]`Ctrl`-`m`| `Ctrl`-`/`
Single line Indent | `Ctrl`-`u`/`i`| none /`shift`-`tab`|-
\* Multiline Indent | [`shift`]`tab`| <-SAME | <-SAME
\* Search Last/Next word|Ctrl-⬆/⬇|-|-
\* Find all Reference|Ctrl-Shift-D(in Document)/E(All)|-|Alt-Shift-F12(only recognized)
\* Mark and Jump |`Ctrl`-`m`/`,` |`Ctrl`+`Alt`+`B`, [`shift`]`Ctrl`-`B`|-
Adjust selection |`shift`- ⬅/➡|<- SAME |`Alt`-`shift`- ⬅/➡
Jump between last two positions|`Alt`- ⬅/➡ ？？？|-|-
Jump to BOW/EOW |`Ctrl`- ⬅/➡|<- SAME|<-SAME
Words before and after jump |`Ctrl`-`/`/`\`|-|-
Zoom text | `Ctrl`-`-/+/0`| <-SAME | none 0
Split window|`shift'-`Ctrl`-⬇/➡|-|-
Swap words left and right |-|`Alt`- ⬅/➡|-


> Let editors around the world unify `syntax highlight themes` and `hotkeys`.
