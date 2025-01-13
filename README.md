
### To update version:

#### Repack extension (.crx)

A new version should have a new version number in the manifest (and the folder name, based on how I'm organizing things/handling versioning).

Before deploying: Make sure to chanhge icon back to `TN_Icon.png` instead of `TN_Icon_RED.png`!

In Chrome, go to "Manage Extensions" (the version of extension doesn't have to be installed),  then "Pack extension" button; select folder; select the .pem file in Code/ChromeExtensions/TN_Assist.
Upload here on Github (at home for this project there's an upload files button).  Right-click file for download link, AND BE SURE TO APPEND `?raw=true` to end to get a true download link (based on ` https://www.labnol.org/?p=29092`)
Then update the XML file (can do it right here) with the new version number and the link to the new version.  Should just be changing a number in both spots.
Be sure to "Commit" after both of the above changes.
That should be it.  No need to change anything in Workspace Admin console (as long as XML filename does not change).

Settings in Workspace admin console (shouldn't have to change): Devices > Chrome > Apps & Extensions > Groups: TN extension > yellow button to add extension
App ID: cnjnlmeknckcmejjkjbhnalcgbabbimc
Custom URL: https://github.com/mvogelito/TN-assist/blob/main/TN_Assist.xml?raw=true
Installation policy: Force install and pin

To force-install a local extension (not from Chrome store): see local folder ChromeManagementFiles.  Windows users need to add registry key with token.  Mac users add text file to specific location `/Library/Google/Chrome/` (? or do they?  1xTx couldn't find the right folder but it was force-installed anyway).

Note: Developer inspect is disabled for force-installed inspections.  Change that with registry key: (? does it work??)
https://stackoverflow.com/questions/64954532/cant-open-inspect-in-forced-installed-chrome-extension
