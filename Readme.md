## Useful Commands
### terminal (mac)
```
!!     ... rewrite, appending new commands onto previous command.
ctrl a ... move to beginning of line
ctrl e ... move to end of line.

terminal commands like "ctrl a" and "ctrl e" (a subset of emac commands) also work in other applications 
like slack or google chrome. this is different from vim. 
I found this link useful for experimenting to see if works on terminal:
http://www.rgrjr.com/emacs/emacs_cheat.html
```
### vim
```
esc    ... escape mode.
note: commands follow action number noun format.
gg, 1G ... jump to beginning
G      ... jump to end
ctrl b ... page up
ctrl f ... page down
d5d    ... delete 5 lines
d5w    ... delete 5 words
p      ... paste what was deleted  -- this is a different paste from command c and command v which is convenient.
u      ... each u is an undo
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

I go to this command often... <br>
http://vim.wikia.com/wiki/Search_and_replace<br>
this looked useful<br>
http://www.radford.edu/~mhtay/CPSC120/VIM_Editor_Commands.htm
http://vim.wikia.com/wiki/All_the_right_moves
```
(pending double checking all commands)
visual mode
   from escape mode type v

scroll a number of lines
x   -- delete and enter insert mode can be put back in excape mode with p or undo
shift i -- insert mode at beginning ... type info. then, escape will put to beginning of all lines selected in visual mode.
shift a -- insert mode at the end   ... type info. then, escape will put to end of all lines selected in visual mode.

```
