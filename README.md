This repo only contains a single script, used to test RemoteSigned policy for Powershell.

You can try this :
- Download the whole project as a zip and type "Get-Item <PathToDownloadZip> -Stream Zone.Identifier" : it should output something, which proves the zip has been detected as a download
- Unzip the archive, and do the same command on the extracted powershell : it should output an error, which proves the powershell script is "trusted" because you put it yourself on the disk
- Download only the GetDate.ps1 script by right click > "Save link as...", and do the same command on it : this time it has a zone identifier, so it has been detected as a download.
