# tmux_and_screen
## Tmux and screen cheatsheet

| Action	| tmux	| screen |
| --------|:-----:|-------:|

start a new session	tmux OR
tmux new OR
tmux new-session	screen
re-attach a detached session	tmux attach OR
tmux attach-session	screen-r
re-attach an attached session (detaching it from elsewhere)	tmux attach -d OR
tmux attach-session -d	screen -dr
re-attach an attached session (keeping it attached elsewhere)	tmux attach OR
tmux attach-session	screen -x
detach from currently attached session	^b d OR
^b :detach	^a ^d OR
^a :detach
rename-window to newname	^b , <newname> OR
^b :rename-window <newn>	^a A <newname>
list windows	^b w	^a w
list windows in chooseable menu		^a "
go to window #	^b #	^a #
go to last-active window	^b l	^a ^a
go to next window	^b n	^a n
go to previous window	^b p	^a p
see keybindings	^b ?	^a ?
list sessions	^b s OR
tmux ls OR
tmux list-sessions	screen -ls
toggle visual bell		^a ^g
create another window	^b c	^a c
exit current shell/window	^d	^d
split window/pane horizontally	^b "	^a S
split window/pane vertically	^b %	^a |
switch to other pane	^b o	^a <tab>
kill the current pane	^b x OR (logout/^D)	
collapse the current pane/split (but leave processes running)		^a X
close other panes except the current one	^b !	
cycle location of panes	^b ^o	
swap current pane with previous	^b {	
swap current pane with next	^b }	
show time	^b t	
show numeric values of panes	^b q	
toggle zoom-state of current pane (maximize/return current pane)	^b z	
break the current pane out of its window (to form new window)	^b !	
re-arrange current panels within same window (different layouts)	^b [space]	
Kill the current window (and all panes within)	^b killw [target-window]	
