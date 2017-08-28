## Useful Commands
### terminal (mac)
```
!! ... rewrite, appending previous command onto your new command.
!$ ... rewrite, appending last argument of previous command to new command.
cd - ... did you accidently `cd /` use cd - to quickly get back to your last cd.
```
### Emacs (mac terminal)
Have fun messing with these in a mac terminal! 🙂
terminal commands like "ctrl a" and "ctrl e" (a subset of emac commands) also work in other applications 
like slack or google chrome. this is different from vim. 

`ctrl A` beginning of line
<br>`ctrl E` end of line
<br>`ctrl -` undo
<br><b>I probably wont use...</b> `ctrl k` kill remainder of the line.
<br>`ctrl w` remove word backward.


`optn b` backward word. (same note as below)
<br>`optn f` forward word. 
* <b>note, the above two commands require option enabled as metacharacter. contact mike or look at this post. <br>and search chris page: [enable_option_as_meta_and_move_forward_word_emacs](https://stackoverflow.com/questions/81272/is-there-any-way-in-the-os-x-terminal-to-move-the-cursor-word-by-word) </b>

`ctrl a` + `ctrl k` could be a lethal combination!
### Vim!! (Im always using vi just because it is one character less to type for program start)
#### escape mode ... esc
```
note: commands follow action number noun format.

gg, 1G ... jump to beginning
G      ... jump to end
ctrl b ... page up
ctrl f ... page down
d5d    ... delete 5 lines
d5w    ... delete 5 words
p      ... paste what was deleted  -- this is a different paste from command c and command v which is convenient.
u      ... each u is an undo
ctrl r ... ctrl r is an redo
j      ... josh plicque likes this one.. ive still got to figure it out.
   shift i ... enter insert mode from escape mode at beginning of line.
   shift a ... enter insert mode from escape mode at end of line.
   i       ... enter insert mode from escape mode at current position of cursor.
:wq    ... write and quit from escape mode.
:q!    ... quit and overide changes.
:wq!   ... write and quit with overide.
:5     ... jump to line #5


:%s/foo/bar/g
Find each occurrence of 'foo' (in all lines), and replace it with 'bar'.
``` 
#### visual block mode ... from escape mode type ctrl v 
```
scroll a number of lines
x   -- delete and enter insert mode can be put back in excape mode with p or undo
shift i -- insert mode at beginning ... type info. then, escape will put to beginning of all lines selected in visual mode.
shift a -- insert mode at the end   ... type info. then, escape will put to end of all lines selected in visual mode.
```
