# Not boring wallpapers
A macOS `launchd` agent downloading a new [Bing Wallpaper](https://www.microsoft.com/en-us/bing/bing-wallpaper) every day.

![Wallpapers](docs/wallpapers.png?raw=true "Wallpapers")  


# Install

1. Run in Terminal
    ```bash
    cd ~/Library/LaunchAgents && curl -fsSL https://raw.githubusercontent.com/roboxdev/not-boring-wallpapers/master/net.manapool.not-boring-wallpapers.plist -o ./net.manapool.not-boring-wallpapers.plist && launchctl load ./net.manapool.not-boring-wallpapers.plist 
    ```
   It can take a couple of minutes before a wallpaper is downloaded
2. Go to **System Preferences** › **Desktop & Screen Saver**  
![Guide](docs/installation.png?raw=true "Guide")  
3. Select **Desktop** tab
4. Add the `~/NotBoringWallpapers` folder created in step `1`
5. Select a wallpaper.
6. [Optional] Go to **Dock** › **System Preferences** › **Right Click** › **Options** › **Assign To** › **All Desktops** and  
repeat step `5` for each Space or Display  

# Uninstall
```bash
cd ~/Library/LaunchAgents && launchctl unload ./net.manapool.not-boring-wallpapers.plist && rm -f ./net.manapool.not-boring-wallpapers.plist 
```

# Credits
- [Microsoft Bing](https://www.microsoft.com/en-us/bing/bing-wallpaper) wallpapers service
- [Timothy](https://github.com/TimothyYe/bing-wallpaper) for providing beautiful REST API
