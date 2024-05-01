# arc_fix_firestore
1) The First step, download the repository and close Arc Browser;

2) Edit ArcFix.bat, change C:\Users\riica (riica must be replaced with the user's folder name);

3) Open the task scheduler and create a new simple task;

4) Give the task a name ex: ArcFix and proceed;

5) Select "when logging in" and proceed;

6) Check start a program and proceed;

7) In program/script put: powershell.exe;

8) In argument put: -NoProfile -ExecutionPolicy Bypass -WindowStyle Hidden -File "C:\close_arc.ps1" (where C:\close_arc.ps1 is the location of the .ps1 file);

9) Press Next and Finish;

10) To avoid having to restart the machine, you can right-click on the task created in the list, and click on execute.
