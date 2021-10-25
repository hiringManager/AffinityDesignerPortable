# Affinity Designer Portable

If you're lazy like I am and need to move around **Assets, Brushes, Styles, Application Preferences, Workspace Layout** etc - and find Designer's ability to actually handle this objectively poor, then here's how to deal with it in a functional (albeit hacky) way. You just have to know about the magic of Windows 'Roaming Files.'   
This also /most likely/ applies to Affinity Photo and Affinity Publisher, but I haven't tested them.

This is my personal method and guide, and I am not accountable if you break something. You should have backups, and you should make sure that this works before deleting anything.

![image](https://user-images.githubusercontent.com/64992493/132263307-cd59f141-9cc8-41ef-b3d4-4e14ccc35d4d.png)

## Backup Old Files
1) Open File Manager  
2) Ctrl+L and type %APPDATA% (This should open C:\Users\YourName\AppData\Roaming)  
3) Navigate to 'Affinity'  
4) Copy Every folder and put it somewhere. 

## Paste New Files
(With new user, install, or OS. (Windows 10 to Windows 11 in my case))    
1) Open new %APPDATA% Affinity folder
2) Make backups of these new folders just in case
3) Paste and overwrite
4) Launch Designer

You should know that I also accidentally deleted 'C:\Users\...\AppData\Roaming\Affinity\Designer\1.0\preferences.dat' when my Affinity stalled on first launch. **This may or may not be relevant.** However, deleting it didn't seem to affect anything and the file was regenerated the next time it was opened.

## Information:
- The username/path seemingly doesn't matter, as I went from 'oldUser' to 'newUser'.
- Expect that the first few times loading will be /slow/. This is most likely because the large files need to be indexed or whatever, and Affinity/Windows are working at it during these first few starts. This disappears after a few launches. See above if you encounter this.
- Seemingly all of the objectsyles, brushes, etc are stored in 'C:\Users\...\AppData\Roaming\Affinity\Designer\1.0\user' so you could /maybe/ circumvent some potential issues by strictly copying those. For preferences 'C:\Users\...\AppData\Roaming\Affinity\Designer\1.0\Settings'. I have not tested this. 
- If you wanted a fully portable install, then you could copy C:\Program Files\Affinity into X:\Users\You\"" and run the .exe from there.
- If I run into any issues, I will update this - But I doubt it. If you run into any issues though, let me know.
- If someone would like to test symlinking this for a multi-user environment(or organization) and letting me know and I'll add it here.

## Update 10-25-21  

These are the files I copied over on my recent install, and it's seemingly less problematic. Note that this is for assets, brushes, etc, and not for settings.  
![image](https://user-images.githubusercontent.com/64992493/138753811-c05b1583-cfe0-4ca6-bba8-73c35016b359.png)  
