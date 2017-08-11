# Introduction
By Chris Le Roy (@brompwnie) chris@sensepost.com

Rattler is a tool that automates the identification of DLL's which can be used for DLL preloading attacks. More information can be found in this blogpost https://sensepost.com/blog/2016/rattleridentifying-and-exploiting-dll-preloading-vulnerabilities/.

Rattler's associated research was presented @bsides Cape Town and the talk can be found here, https://www.youtube.com/watch?v=xvluwoPM8v8.


# What does it do?
Rattler automatically enumerates an applications DLL's to identify and exploit DLL's which can be hijacked via a DLL preloading attack.


# Getting the code

Firstly get the code:
```
git clone https://github.com/sensepost/rattler.git
```

# Building the code

Rattler was developed using C++ with Microsoft Visual Studio 2015 using the default console application project settings.

# Getting the binaries

Rattler compiled binaries can be found in the Releases section, https://github.com/sensepost/rattler/releases.

# Usage

Depending on the target executable location, Rattler may need to be run with elevated permissions.

ratter_32.exe "c:\path\to\target\application.exe" 1

* "c:\path\to\target\application.exe" =path to the executable you want to enumerate.
* 1 = Enumeration mode, only one at this point.

```
C:\Users\User\Desktop>Rattler_32.exe "C:\Users\User\Downloads\NDP462-KB3151800-x86-x64-AllOS-ENU.exe"  1
[+] RATTLER
[*] TARGET APPLICATION: C:\Users\User\Downloads\NDP462-KB3151800-x86-x64-AllOS-ENU.exe
[+] STARTING UP...
[*] TARGET PROCESS ID: 3504
[+] IMPLEMENTING EXECUTABLE TEST

[*] TARGETING DLL-> C:\Windows\SYSTEM32\CRYPTSP.dll
[*] INFO: DLL IS VULNERABLE TO EXECUTABLE TEST-> C:\Windows\SYSTEM32\CRYPTSP.dll

[*] TARGETING DLL-> C:\Windows\system32\rsaenh.dll
[*] TARGET DLL IS NOT VULNERABLE TO EXECUTABLE TEST

[*] TARGETING DLL-> C:\Windows\SYSTEM32\ntmarta.dll
[*] TARGET DLL IS NOT VULNERABLE TO EXECUTABLE TEST

[*] TARGETING DLL-> C:\Windows\SYSTEM32\feclient.dll
[*] TARGET DLL IS NOT VULNERABLE TO EXECUTABLE TEST

[*] TARGETING DLL-> C:\Windows\system32\uxtheme.dll
[*] TARGET DLL IS NOT VULNERABLE TO EXECUTABLE TEST

[*] TARGETING DLL-> C:\Windows\System32\MSCTF.dll
[*] TARGET DLL IS NOT VULNERABLE TO EXECUTABLE TEST

[*] TARGETING DLL-> C:\Windows\system32\dwmapi.dll
[*] TARGET DLL IS NOT VULNERABLE TO EXECUTABLE TEST

[+] EXECUTABLE TEST TOTAL DLL's IDENTIFIED: 43
[+] EXECUTABLE TEST TOTAL VULN COUNT: 1
[*] EXECUTABLE TEST VULNERABLE DLL-> C:\Windows\SYSTEM32\CRYPTSP.dll

```


# Information

Rattler was developed using C++ using Microsoft Visual Studio 2015. Rattler can be used to test 64 and 32 bit applications. Rattler's default "payload" is a DLL (payload.dll) which invokes calc.exe. The default payload is 32bit. A 64bit payload can be used in conjunction with the 64bit executable to enumerate 64bit executables.

# License

Rattler is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (http://creativecommons.org/licenses/by-nc-sa/4.0) Permissions beyond the scope of this license may be available at http://sensepost.com/contact.
