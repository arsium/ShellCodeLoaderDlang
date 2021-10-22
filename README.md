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
