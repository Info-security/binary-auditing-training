
- Injecting your Dll into the target at runtime -

GOAL:
-----

You must insert a MenuItem called "Detour" into the menu of the
ReverseMe. When clicking this MenuItem, it should call a function inside
a Dll that you will have to code yourself. This function should show the
RunDialog-box (like the one in the Windows "Start"-menu.... Hint: call by
Ordinal in Shell32.dll). When executed, the RunDialog should show the Icon
of the ReverseMe. You MUST do this by pushing the handle of the Icon to the
call of your function inside your DLL. The OK-button of the RunDialog must
be disabled when the RunDialog opens (and enabled when entering something in
the editbox of the dialog). Afterwards the code-execution will have to 
return to the ReverseMe without exiting the program.

And now the fun part of it all............


RESTRICTIONS:
-------------

All of the patches that you apply will have to be done AT RUNTIME
(hint: WriteProcessMemory). So, you will have to leave the ReverseMe
itself totally unpatched/unchanged.