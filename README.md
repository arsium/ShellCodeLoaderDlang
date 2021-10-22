# ShellCodeLoaderDlang
A class to load shellcode in memory written in D

How does it work ?

It uses NTApi to load and call the shellcode if loaded.

Functions Added :

* NtAllocateVirtualMemory
* NtWriteVirtualMemory
* NtProtectVirtualMemory
* GetCurrentProcess

What is the difference between 'Call' and 'CallFromAthread' ?

* 'Call' :
![Image description](https://i.postimg.cc/jSFg9Y3n/Capture-d-cran-91.png)

* 'CallFromAthread' :
![Image description](https://i.postimg.cc/4yfQyWFT/Capture-d-cran-96.png)
