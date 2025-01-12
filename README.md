Github Tutorial

Reminder to get link to file: 
  1. Right-click file for download link.
  2. Append `?raw=true` to any file URL on Github to get the direct link.

How to Host Files on Github: https://www.labnol.org/?p=29092

Note: Developer inspect is disabled for force-installed inspections.  Change that with registry key:
https://stackoverflow.com/questions/64954532/cant-open-inspect-in-forced-installed-chrome-extension

### To update version:

#### Repack extension (.crx)
New version should have new version number in manifest (and possibly in the folder name).
In Chrome, manage extensions, make sure the latest version is installed (necessary step??).  Then "Pack extension" button; select folder; select the .pem file in Code/ChromeExtensions/TN_Assist.
Check in future, but this new CRX should have same ID cnjnlmeknckcmejjkjbhnalcgbabbimc as previous versions.
Upload here (upload files button).  See above for getting link , and append `?raw=true` to get a true download lilnk.
Then update the XML file with the new version number and the link to the new version.
That should be it.  No need to change anything in Workspace Admin console (as long as XML filename does not change).

