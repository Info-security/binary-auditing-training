If you run the program, you will see that in the
menu there is an option to choose a directory. If
you do so and everythink is ok, you will get a
messagebox saying 'Now it's your turn'. Indeed, this
is where you, the reverser, come in. 

Your task: based on the directory selected by the user,
you are supposed to add fonts. As simple as that. Now
let me explain: you are supposed to go through all the
files in that directory and add to the listbox the files
that could be valid font files. 
Now, what is a valid font file? Quoting from the api ref:
"The filename may specify either a .FON font resource
file, a .FNT raw bitmap font file, a .TTF raw TrueType file,
 or a .FOT TrueType resource file. "

So, all you have to do is add to the listbox the files
in the directory selected by the user that correspond to the
above definition. Then, when the user presses 'Add it', add
to Windows' font table the currently selected file in the
listbox. Also, you need to enable the 'Add it' button when
there are apropriate files in the dir selected by the user.

=============================================================
This isn't a hard reme, but one that can be turned into an
usefull app. Fact is I had the idea for it when I had to
code a little exe to add some font files to Windows' table
(for an unknown reason the 'Install New Font' option wasn't
displayed in the File menu of the Fonts directory).
=============================================================
