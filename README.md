# Microsoft Visual Studio 2022 Off-Line-Installer
Builds a Visual Studio 2022 Offline Installer for local intranet use.

NOTE - Needs some config.

1. Install IIS
2. Add MimeType for .ps1 (See Diagram below)
3. Double click the VHD to mount it (Appears as an extra drive in file explorer. Right click the drive and eject to unmount)
4. Copy inetpub\wwwroot\*.* on VHD to your "Default Web Site" directory
5. Run the GetVisualStudio.bat (Using a high bandwidth connection it's about 24 hours as it downloads Visual Studio 2022 in all languages - So run overnight)
6. After you get a green line saying successful make sure the Response.json on the VHD overwrites the Response.json under C:\VS2022\VisualStudio directory.
7. Install PowerShell x64
8. NOTE - Make SURE you use the associated ps1 script or you'll use up your ONE SHOT with the VS2022 installer and need to download it again!!!
9. goto http://localhost to start the installer it will download the ps1 script and there are some instruction on http://localhost to run so that the ps1 content runs as remotesigned.
10. ALL GOOD!!!


![AddMimeType](https://github.com/user-attachments/assets/11af6051-4448-4359-ac01-5066eed2e023)
