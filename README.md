# MCCMenuPatcher


UE4 4.21 project which serves as an example on how to implement blueprint code through a single asset replacement for Halo the Master Chief Collection.
The pak is created with u4pak: https://github.com/panzi/u4pak

This works for both the Steam and Windows Store version. For the Windows Store version there's additional steps required which isn't covered here.

In order to create a pak that can be used in MCC:

GENERATING THE PATCH
1. Open the project with UE4 4.21
2. Under file -> Cook Content for Windows
3. When content is cooked, go to Saved/Cooked/WindowsNoEditor/MCC/
4. Remove everything in said MCC folder except the content folder
5. Run the MCC folder through u4pak
6. Rename the pak file to whatever you want but add "_p" to the end of the name

APPLYING THE PATCH
1. Browse to the folder where you can find MCC's pak file (Halo the Master Chief Collection/MCC/Content/Paks/)
2. Create a new folder named ~mods (it can be any name as long as it's precedes the pak file in alphabetical order)
3. Paste the generated pak file in the ~mods folder
4. Run MCC with EAC disabled
