# Arc Fix Tutorial

1. Download the .ps1 file (arc_fix.ps1 > ••• > Download) and close Arc Browser.
2. Move the file on C:\ [^1]
3. Open the task scheduler and create a new simple task.
4. Give the task a name (for example, *ArcFix*) and proceed.
5. Select "**When logging in**" and proceed.
6. Check "**Start a program**" and proceed.
7. In program/script put: `powershell.exe`
8. In argument put: `-NoProfile -ExecutionPolicy Bypass -WindowStyle Hidden -File "C:\close_arc.ps1"` (where *C:\close_arc.ps1* is the location of the .ps1 file).
9. Press *Next* and *Finish*.
10. To avoid having to restart the machine, you can right-click on the *task* created in the list, and click on "**Execute**".

[^1]: This is not neccesary, however, the script is made for the case when file is located in C:\. You may change the script manually.
