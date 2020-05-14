# instant-clone-lookup-beta
Beta of the Horizon Instant Clone Lookup Tool

@chrisdhalstead

chalstead@vmware.com

###### Version Beta 2005.1

May 14, 2020

Lots of fixes to detection/mapping of Pools to Internal VMs - it is recommended to run this version

**Prerequisites:**

- VMware Horizon 7.0 or later with Instant Clones
- Virtual Center 5.x or later
- .NET Framework 4.6 or later
- Windows 10 or Windows Server 2012 or later to run the application

**Note**:

- The tool only works right now with Instant Clone Desktops.  I will be adding support for Instant Clone RDSH
- Orphaned Internal VM's are not currently shown - I need to format them so hid them for now.
- If you have a version installed, go to add/remove programs and remove the old version before installing the new one.

**Installation:**

1. Download the folder structure locally
2. Run setup.exe

**Usage:**

1. Enter connection server name (no https://) and click connect to server
2. Accept the certificate if prompted
3. Enter username, password and domain for the connection server and click ok
4. Enter the virtual center name (no https://) and click connect to server
5. Enter the username, password and domain for the virtual center
6. Click Populate Data
7. Instant Clone Pools will show all correlated internal VMs (Template, Replica, Parents) as well as host and datastore information
8. You can click Options | View by Master VM / Snapshot to see association of Master VM / Snapshot to instant clone pools.
