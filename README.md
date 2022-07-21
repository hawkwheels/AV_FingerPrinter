# AV_FingerPrinter
A small C# code to get running AVs in a machine based on various AV process names 

We have predefined a list of well-known AV applications in the AV_Check array within our code, which is taken from the previous section, where we discussed fingerprinting AV software (table above). Then, we use the Windows Management Instrumentation Command-Line (WMIC) query (select * from win32_process) to list all currently running processes in the target machine and store them in the processList variable. Next, we go through the currently running processes and compare if they exist in the predefined array. If a match is found, then we have AV software installed.

To compile the C# program in the Microsoft Visual Studio, select Build from the bar menu and choose the Build Solution option. Then, if it complied correctly, you can find the path of the compiled version in the output section.
