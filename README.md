# ShellCodeLoaderDlang
A class to load shellcode in memory written in D

How does it work ?

It uses NTApi to load and call the shellcode if loaded. For demo, I use a simple csharp app displaying a messagebox converted in shellcode with https://github.com/TheWover/donut.

Functions Added :

* NtAllocateVirtualMemory
* NtWriteVirtualMemory
* NtProtectVirtualMemory
* GetCurrentProcess

What is the difference between 'Call' and 'CallFromAthread' ?

* 'Call' :<br>
![Image description](https://i.postimg.cc/jSFg9Y3n/Capture-d-cran-91.png)

* 'CallFromAthread' :<br>
![Image description](https://i.postimg.cc/4yfQyWFT/Capture-d-cran-96.png)

Sources : 
* https://docs.microsoft.com/en-us/windows/win32/api/processthreadsapi/nf-processthreadsapi-createthread
* https://github.com/secrary/InjectProc/blob/master/InjectProc/injection.cpp
* https://github.com/3gstudent/Inject-dll-by-Process-Doppelganging/blob/master/inject.c
* https://github.com/3gstudent/Inject-dll-by-Process-Doppelganging/blob/master/ntos.h
* https://github.com/arsium/ShellCodeLoader/blob/main/ShellCodeLoader/ShellCodeLoader.cs
* https://tour.dlang.org/tour/en/basics/basic-types
* https://doxygen.reactos.org/
