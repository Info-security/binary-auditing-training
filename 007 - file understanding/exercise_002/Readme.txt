It's not really an easy one as you need to understand and inverse the processus of the save of a file, to be able to implement the open of it :). But, as it will be easy for you all, i decided to complicate things a bit. Here are the good news :

1) You can modify *ONLY* the PE of the file, more exactly just everything before the first section.


HINTS:
- You can do what you want at runtime, so, have fun with WriteProcessMemory :)
- if you invoke GetCurrentProcessId, then you have a valid process handle to play with.
- I suggest you to write a dll. :)
- I repeat that you can play with the space between the .pe and the first section.


