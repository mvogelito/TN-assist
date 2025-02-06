
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

To force-install a local extension (not from Chrome store): see local folder ChromeManagementFiles.  Windows users need to add registry key with token.  Mac users ?can? text file to specific location `/Library/Google/Chrome/` (though this doesn't seem necessary; 2 tx haven't needed that step).

Note: Developer inspect is disabled for force-installed inspections.  Change that with registry key: (? does it work??)
https://stackoverflow.com/questions/64954532/cant-open-inspect-in-forced-installed-chrome-extension

#### To update version
Before doing this: Update manifest.json.  If this will be a LIVE version, then change the icon from red DEV icon to LIVE blue.  AND fix the version number.  Note *no* leading zeros on version numbers!  version 0.3.01 is seen as 0.3.1
In any chrome instance (extension doesn't need to be installed; can be any profile): manage extensions, upper-left button to pack extension.  Choose correct folder of extension, and choose the correct .PEM file (in PackagedFiles/ and choose either the LIVE or DEV one, depending on which version you're putting up).  This creates CRX file.  Rename CRX file (correct the version number and add "_DEV" if necessary.
Then upload that file to this directory (soon to be relocated).  And edit the appropriate .XML file (DEV or plain (LIVE)): just change version number and the filename (version number).
That should be it.
