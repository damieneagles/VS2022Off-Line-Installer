# Microsoft Visual Studio 2022 Off-Line-Installer
Builds a Visual Studio 2022 Offline Installer for local intranet use.

NOTE - Needs some config.

1. Install IIS
2. Double click the VHD to mount it (Appears as an extra drive in file explorer. Right click the drive and eject to unmount)
3. Copy inetpub\wwwroot\*.* on VHD to your "Default Web Site" directory
4. Run the GetVisualStudio.bat
5. After you get a green line saying successful make sure the Response.json overwrites the Response.json under C:\VS2022\VisualStudio directory.
6. Install PowerShell x64
7. goto http://localhost to start the installer it will download the ps1 script and there are some instruction on http://localhost to run so that the ps1 content runs as remotesigned.
8. ALL GOOD!!!


