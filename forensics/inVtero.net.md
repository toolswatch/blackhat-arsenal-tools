# [inVtero.net](https://github.com/ShaneK2/inVtero.net)

## Description
inVtero.net: A high speed (Gbps) Forensics, Memory integrity & assurance. Includes offensive & defensive memory capabilities.
Find/Extract processes, hypervisors (including nested) in memory dumps using microarchitechture independent Virtual Machiene Introspection
techniques 

Supports: VMWare (client/servers), XEN and physical systems (PAGEDUMP).

#### Integrity
Users can manage their own "golden images" of secure hashes used to ensure no byte slipps through the cracks
of a forensic, reverse engineering, sandbox analysis or host integrity monitoring operation.

We've recently added cloud hosted bitmaps and are expanding this to allow users to use the integrity funtionality without having to construct
a database first.

The block based integrity checks occur at a configurable size and will isolate very small code patches quickly.

Integrity checking provides confidence to useres that they have analyzed "everything" and they have not wasted 
time looking in the wrong plaes.

#### Memory Hacking
An IronPython shell is able to use native type reflection that allwos for reading and writing physical memory dumps.  Test a new 
kernel patch or improve inVtero itself.  (e.g. edit _EPROCESS objects from python and write them back to a VM image then resume
exection to observe DMA style hacking with very easy scripts that map 1:1 to known symbol sources)

Recent modules include a Gargoyle detection mechanism that uses the type information extracted from the systems to allow for
an exhaustive verification of thread stack states that can detect the preseanse of RoP type _weird machienes_.

#### Performance
A goal of the project is to provide high quality assurace as quickly as possiable.  To avoid the common pitfall of many debuggers 
and forensic platforms that are trivially compromised.  

### Categories
* Forensics
* Debugger (Passive memory debugging/hacking)
* Malware HIDS (Integrity Monitoring) 
* Reverse Engineering

### Black Hat sessions
[![Arsenal](https://rawgit.com/toolswatch/badges/master/arsenal/usa/2017.svg)](http://www.toolswatch.org/2017/06/the-black-hat-arsenal-usa-2017-phenomenal-line-up-announced/)
 
### Code 
https://github.com/ShaneK2/inVtero.net

### Lead Developer
K2 - https://github.com/K2

### Social Media 
* [Twitter](https://twitter.com/ktwo_K2)
----
![In Vtero](https://raw.githubusercontent.com/ShaneK2/inVtero.net/gh-pages/images/inVtero.jpg)
