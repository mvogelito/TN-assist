
### To update version:

#### Repack extension (.crx)
New version should have new version number in manifest (and teh folder name, how I'm organizing things).
In Chrome, go to "Manage Extensions" (the version of extension doesn't even have to be installed),  then "Pack extension" button; select folder; select the .pem file in Code/ChromeExtensions/TN_Assist.
Upload here on Github (at home for this project there's an upload files button).  Right-click file for download link, AND BE SURE TO APPEND `?raw=true` to end to get a true download lilnk.
Then update the XML file (can do it right here) with the new version number and the link to the new version.  Should just be changing a number in both spots.
Be sure to "Commit" after both of the above changes.
That should be it.  No need to change anything in Workspace Admin console (as long as XML filename does not change).

App ID: cnjnlmeknckcmejjkjbhnalcgbabbimc

Reminder to get link to file: 
  1. Right-click file for download link.
  2. Append `?raw=true` to any file URL on Github to get the direct link.

How to Host Files on Github: https://www.labnol.org/?p=29092

Note: Developer inspect is disabled for force-installed inspections.  Change that with registry key:
https://stackoverflow.com/questions/64954532/cant-open-inspect-in-forced-installed-chrome-extension
