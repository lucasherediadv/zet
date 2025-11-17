The core philosophy is that you are speaking a language to the editor, rather than just hitting commands. This allows for concise and powerful text manipulation.

Commands that perform an action:

* `y` (yank/copy)
* `d` (delete/cut)
* `c` (change)

The range/target of the action. Any movement command can follow a verb:

* `w`, `b`, `e` (word movements)
* `{`, `}` (paragraph movements)
* `(`, `(` (sentence movements)
* `'` (mark movements)
* `/pattern` or `?pattern` (search movements)

Repeat a command or movement a specified number of times:

* `3J` (join the next 3 lines)
* `d5}` (delete through the end of the 5th paragraph down)

Marks and registers.

Set a location in the text using a lowercase letter.

* `ma`: Set mark 'a' at the cursor
* `'a`: Move to the line containing mark `a`

Registers(`"`): Named copy buffers (26 named, plus the anonymous register)

* `"add`: delete the current line into the 'a' register
* `"by/foo`: yank to the next line containing 'foo' into the 'b' register
* `"ap`: paste the contets of the 'a' register
