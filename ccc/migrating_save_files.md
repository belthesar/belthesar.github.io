# Migrating Save Files

## Introduction

If you scrounge around the Steam forums or other places on the internet, folks, including the developers of the game, will say you can migrate a world from Peer to Peer to a Dedicated Server, but your saves are out of luck. 

![I disagree!](https://media.giphy.com/media/Uqj3pYhSgS7eTspLUw/giphy-downsized.gif)

This does take a little bit of work to make this happen, but I promise we'll get through it together. 

## Migration Steps
1. We need to get to where save games for The Forest are stored on your computer. This is usually in the following location: `C:\Users\<your username>\AppData\LocalLow\SKS\TheForest\<your Steam ID>\`. Here's a quick and easy way to get to that location:
    1. Open up a File Explorer window. (This may be a Folder icon on your Taskbar, or you can hit the Windows key + E)
    2. In the address bar, type `%appdata%\..\LocalLow\SKS\TheForest` and hit enter.
    3. In this folder, there should be at least one, potentially more folders. These folders are named after your Steam ID. If there are more than one folder with numbers as the name, you may 
    4. In the File Explorer window that opens, navigate to `LocalLow\SKS\TheForest\<your Steam ID>\Multiplayer\cs`. (this will be a bunch of numbers, and likely the only folder like it in the `TheForest` folder)
    ![The Forest Saves Folder - Source](/ccc/img/theforest-saves-folder-source.png)
2. There may be one or more files in this folder, depending on if you've played The Forest with other people. The file we're interested in should have the name `5e824930-c76a-481b-841d-c7594818e7ba`. Right click and Copy this file. 
3. From here, we need to go up three levels to the `TheForest` folder. You should be able to do this by clicking on the `TheForest` folder in the address bar.
4. In this folder, there may or may not be a folder named `ds`, depending on if you've ever played on a Dedicated Server before. If there is, open it up. If not, you'll need to create it. You can Right Click on an empty space in this folder, and select New -> Folder. Name this folder `ds`.
![The Forest - Save Root Folder](/ccc/img/theforest-root-folder.png)
5. Open up the `ds` folder. If you've played on a Dedicated Server before, there may be a folder named `Multiplayer` in here. If not, use the same steps above to create it. Once you've verified there is a folder named `Multiplayer` in the `ds` folder, open it up.
6. In the `Multiplayer` folder, there should be a folder named `cs`. If there is not, create it using the same steps above. Once you've verified there is a folder named `cs` in the `Multiplayer` folder, open it up.
7. Once we're in the `cs` folder, we need to paste the file we copied earlier. You can do this by Right Clicking in the folder, and selecting Paste.
8. You should now see the file `5e824930-c76a-481b-841d-c7594818e7ba` in the `cs` folder. 

If you've done everything correctly, you should be able to follow the directions in [How to Connect](/ccc/how_to_connect) to connect to the Dedicated Server, and when you join the server, you should pick up right back where you left off on the Peer to Peer server.