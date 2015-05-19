## How to use VSD? ##

When running, _VSD_ lists all the running processes in a the _list-view_, then, you can use any of the buttons, _check-boxes_ or the _pop-up_ menu to interact with the processes. Here is the list of current features:

**Main window options:**

  * Refresh: refreshes the processes list.

  * About: displays the about window.

  * Full Dump: paste header from disk: this option is only valid when you select _"Full Dump"_ over a process. Using this, you can read the original _PE header_ of a running process from the disk and paste it in memory before dumping. This is specially useful when dealing with packers because they usually change the data in the memory of a packed program, specially the _PE header_ section, to avoid the dumping process.

  * Full Dump: fix header: this option is only valid when you select _"Full Dump"_ over a process. Using this, you can fix the _Raw Offset_ and _Virtual Offset_ of a process, in other words, _Raw Offset_ == _Virtual Offset_.

  * Exclude x64 processes: (Only in the x86 version) when running on Windows 7 (x64), _VSD_ can show you the x64 processes although you can't do too much with them. If you don't want to see these processes you can use this options to filter them from the list.
You can use this feature **ONLY** when running with **Administrative privileges** (Vista/Seven/Server 2008 on both platforms, _x86_ and _x64_), if not, _VSD_ will show you all the running processes. This is due to _VSD_ can't obtain a handle via _OpenProcess_ to interact with the processes (note: if you know what I'm talking about and you have an idea on how to improve/solve this problem, just email me).

  * Total number of processes: prints the total number of running processes.

  * Sort process by Name, PID, ImageBase or ImageSize: you can sort the list of processes by doing click in the top of every column.

**Pop-up menu options:**

  * Select All: selects all the processes on the list.

  * Copy to Clipboard: copies the selected items to the clipboard.

  * Dump:
    1. Full: dumps the entire process' memory to disk.
    1. Partial: dumps a partial memory region to disk. You must enter a valid address and size.
    1. Regions: displays the regions windows where you can interact with all the virtual sections of the process.

  * View:
    1. Modules: displays all the loaded modules in the process.
    1. Handles: displays all the opened handles by the process.
    1. Threads: displays all threads in the process.

  * Patch: displays a new dialog with the patch process options.

  * Kill Process: terminates the execution of the selected process.

  * Refresh: refreshes the process list.

**Patch window options:**

  * No. Bytes to patch: indicates the number of bytes to patch.
  * Address to Patch: indicates the address in the process memory region to patch.
  * New Bytes: are the bytes to write to the process memory.
  * Bytes: displays the original bytes in the process memory.
  * Search: when 'No. Bytes to patch' and 'Address to Patch' are set, the user can use this button to look for the original bytes in the process. The original bytes are displayed in the 'Bytes' edit-box.
  * Patch: starts the process of patching the process memory.
  * Close: closes the 'Patch' window.

**View Modules window options:**

  * Select All: select all the items in the list.
  * Copy to Clipboard: copy the selected item/s in the list-view to the clipboard.
  * Dump (Full/Partial): Dumps full/partial memory of the selected module to disk.

**View Handles window options:**

  * Select All: select all the items in the list.
  * Copy to Clipboard: copy the selected item/s in the list-view to the clipboard.

**View Threads window options:**

  * Resume: resumes the thread's execution.
  * Suspend: suspends the thread's execution.
  * Terminate: terminates the thread's execution.
  * Select All: select all the items in the list.
  * Copy to Clipboard: copy the selected item/s in the list-view to the clipboard.
  * Refresh: refreshes the thread's list-view.

**Dump Regions window options:**

  * Sort virtual sections by Address, Size, Protect, State or Type: by clicking on the top of every column, you can sort the data listed in the list-view.

  * Dump: dumps the selected virtual section. Not all sections can be dumped, for example, a section marked as free can't be dumped.

  * Refresh: refreshes the sections list.

  * Close: closes the sections window.

## Project Information ##

_VSD_ was tested under Windows XP Professional SP3, Windows 7 Ultimate (x86 & x64), wine under Ubuntu 11.04 x64.
