## What's VSD? ##

_VSD (Virtual Section Dumper)_ is intented to be a tool to visualize and dump the memory regions of a running 32 bits or a 64 bits process in many ways. For example, you can dump the entire process and fix the _PE Header_, dump a given range of memory or even list and dump every virtual section present in the process.

Usage of VSD can be found [here](http://code.google.com/p/virtualsectiondumper/wiki/Usage)

## Latest changes ##

### VSD x86 ###

**Version: 2.1 (18/11/2012)**

  * Added "Ignore unnamed objects" in the window handles.
  * Added "Set Priority" feature in order to set the priority of a given process. ~~[issue 8](http://code.google.com/p/virtualsectiondumper/issues/detail?id=8)~~
  * Added "Suspend process" and "Resume process" features. ~~[issue 10](http://code.google.com/p/virtualsectiondumper/issues/detail?id=10)~~
  * Added "Suspend all threads before dumping". Using this option you can suspend the execution of a given process before to dump it. ~~[issue 5](http://code.google.com/p/virtualsectiondumper/issues/detail?id=5)~~
  * Added updatevsd.exe. More information can be found [here](http://code.google.com/p/virtualsectiondumper/wiki/UpdateVSD)

**Version: 2.0 (01/04/2012)**

  * Added a menu bar.
  * Added a module list viewer.
  * Added Dump Full and Dump Partial over a specific module.
  * Added sorting feature in the module list viewer.
  * Added a handle list viewer.
  * Added sorting feature in the handle list viewer.
  * Added a thread list viewer.
  * Added Resume, Terminate and Suspend functions in the thread list viewer.
  * Added the "Patch" feature.
  * Bugfixes in some functions.
  * Code refactoring in some functions. The code still needs a lot of improvements :P

**Version: 1.1**

  * Fixed a bug in the _PastePEHeader()_ function when calculating the offset of the original PE Header.

**Version: 1.0**

  * First stable release (I hope so :)

### VSD x64 ###

**Version: 1.0**

  * First stable release.

## Greetings ##

As always, I have to thank a lot of people without whom this tool had not seen the light.

Many, many thanks to:
  * **marciano**: for being my friend, beta tester and for reporting a lot of bugs and features.
  * **UlisesSoft**: for UpdateVSD.
  * **MCKSys Argentina**: for being my other beta tester.
  * **Guan De Dio**: for his opinions to improve each of my tools :P
  * **Nacho\_dj**: for being a friend in ARTeam and for supporting me.
  * **Shub-Nigurrath**: for being an amazing friend, for teaching me with his tutorials and for supporting me.
  * **j00ru**: becase he is a good friend and is always answering my questions and teaching me a lot about RE.
  * **deroko**: for being an old friend and for teaching me a lot of stuffs during all this years.
  * **deepzero**: for helping me with the clipboard issue.
  * To all my friends in _CLS_, _ARTeam_, _SnD_, _B@S_, _OpenRCE_, _exetools_ and _Woodmann_.

## Screenshots ##

### VSD x86 ###

**Main window**

https://lh5.googleusercontent.com/-7n84DDmz4XI/T3kfMKmH7SI/AAAAAAAAAFQ/aT4TMRrUjGI/s545/vsd2_main.JPG

**Loaded modules**

https://lh6.googleusercontent.com/-dv3I347RegQ/T3kfMDTAq4I/AAAAAAAAAFU/iYDyF_W9zII/s609/vsd2_modulelist.JPG

**Handles**

https://lh6.googleusercontent.com/-n-XttJuDKuk/T3kfNOzML1I/AAAAAAAAAFs/QqeRVKb62G4/s533/vsd2_handleslist.JPG

**Threads**

https://lh4.googleusercontent.com/-nvIXr_SMs1Q/T3kfNJjWKTI/AAAAAAAAAFo/OGXtmhW5JRU/s547/vsd2_threadslist.JPG

**Patch**

https://lh6.googleusercontent.com/-MlNoD4UjkWk/T3kfMiTK7YI/AAAAAAAAAFg/q3WXs-UiEZQ/s480/vsd2_patchwnd.JPG

### VSD x64 ###

![https://lh5.googleusercontent.com/-VlqHVpcI5vM/T0Qu7MqM7lI/AAAAAAAAAEw/KOD8a5s-hng/s626/vsd_x64.png](https://lh5.googleusercontent.com/-VlqHVpcI5vM/T0Qu7MqM7lI/AAAAAAAAAEw/KOD8a5s-hng/s626/vsd_x64.png)