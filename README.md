# AffinityDesignerPortable

If you're lazy like I am and need to move around **Assets, Brushes, Styles, Application Preferences, Workspace Layout** etc - and find Designer's ability to actually handle this objectively poor, then here's how to deal with it in a functional (albeit hacky) You just have to know about the magic of Windows 'Roaming Files.' This also /most likely/ applies to Affinity Photo and Affinity Publisher, but I haven't tested them. 99% sure that it will.

![image](https://user-images.githubusercontent.com/64992493/132263307-cd59f141-9cc8-41ef-b3d4-4e14ccc35d4d.png)

## Backup Files
Open File Manager  
Ctrl+L and type %APPDATA% (This should open C:Users\YourName\AppData\Roaming)  
Navigate to 'Affinity'  
Copy Every folder and put it somewhere. 

## Paste New Files
(With new user, install, or OS. (Windows 10 to Windows 11 in my case))
Repeat steps but paste them into the new directory, overwriting files that are there (old files overwriting the new ones that exist). 

## Information:
- The username/path seemingly doesn't matter, as I went from 'oldUser' to 'newUser'.
- Expect that the first few times loading will be /slow/. This is most likely because the large files need to be indexed or whatever, and Affinity/Windows are working at it during these first few starts. This disappears after a few launches. Please test this before doing anything drastic.
- Seemingly all of the objectsyles, brushes, etc are stored in 'C:\Users\...\AppData\Roaming\Affinity\Designer\1.0\user' so you could /maybe/ circumvent some potential issues by strictly copying those. For preferences 'C:\Users\...\AppData\Roaming\Affinity\Designer\1.0\Settings'. I have not tested this. 
- If you wanted a fully portable install, then you could copy C:\Program Files\Affinity into X:\Users\You\"" and run the .exe from there.
- If I run into any issues, I will update this - But I doubt it. If you run into any issues though, let me know.
- If someone would like to test symlinking this for a multi-user environment(or organization) and letting me know and I'll add it here.
