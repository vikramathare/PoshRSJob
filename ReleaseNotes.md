---------
|1.7.0.0|
---------
* Remove need for DLL file for building out the classes. Using pure PowerShell (mostly) via means of here-strings and Add-Type for PowerShell V2-4 and the new Classes keywords for PowerShell V5 which includes PowerShell Core/Nano.
* Remove the prefixes for custom objects so they no longer start with PoshRS.PowerShell.. Now they are V2UsingVariable, RSJob and RSRunspacePool.

---------
|1.6.2.1|
---------
* Add support for PowerShell Core on Linux/MacOS (this still needs more work but should load types within a runspace now!)

---------
|1.6.1.0|
---------
* Fixed Issue #75 (Feature Request: Add RunspaceID handling to Start-RSJob for better throttling support)
* Fixed Issue #82 (Exception setting "RunspacePool" in 1.6.0.0 build)

---------
|1.5.7.7|
---------
* Fixed Issue #69 (Module produces error if imported more than once (PS v2 only))
* Fixed Issue #64 (HadErrors in PoshRS.PowerShell.RSJob throws errors in PowerShell V2)
* Fixed Issue #67 (Converted Add-Type code for C# classes to be created via Reflection for Nano server support) <- Created custom dll
* Fixed Issue #61 (Receive-RSJob not allowing -Job parameter input)
* Fixed Issue #63 (Replaced Global variables with Script scope)
* Fixed Issue #66 (Parameters don't work with PowerShell V2)
* Fixed Issue #65 (Bug with v2 variable substitution - single-quoted strings get $var references replaced)
* Fixed Issue #68 (ApartmentState Does Not Exist in Nano)
* Fixed Issue #76 (Jobs don't have output when using ADSI WinNT provider (Receive-RSJob))