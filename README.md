# mosu - my osu or how to set up [osu!](https://osu.ppy.sh) for the best experience on Mac

## My setup
- MacBook Pro 13" from 2018 in the base configuration
    - macOS Mojave (10.14)
- Apple Magic Keyboard
- One by Wacom (CTL-472)

### Why not upgrade to the latest OS?
- macOS Catalina (10.15) has dropped the support for 32-bit applications meaning the osu! stable that is running on Wine is not working (at least there were no ports for Wine to 64-bit when I was trying it out)

## Running the game
#### there are two official versions of the osu! game:

- osu! stable
  - this is the old osu! client that is still the main one (at the time of writing this)
  - emulated using Wine
- [osu! lazer](https://github.com/ppy/osu)
  - completely rewritten in C# .NET Core to support all major platforms natively

### Tweaks for the best performance
- disable mouse acceleration (if you want to play with mouse)
  - [Mouse Acceleration](https://github.com/petak5/mosublob/master/resources/mouseaccelerationpref13-rc.zip) is an easy to use System Preferences plugin tool
- disable VSync / BeamSync (inspired by [this]() and [this]())
  - when playing on dual monitors, the framerate is locked to 60FPS (the monitor's refresh rate)
  - disabling VSync always gives you less input lag
  - download [Graphics Tools](https://developer.apple.com/download/more/?name=Graphics%20Tools) for your version of Xcode (will install many tool, all we need is Quatz Debug)
    - launch Quartz Debug
    - go to `Window` -> `Quartz Debug Settings` (or press `command+1`)
    - under `Vertical Sync`, uncheck `Enable Vertical Sync`
    - when you close the app (`command+q` or right-click the app in the dock and choose `quit`) the VSync will be re-enabled and so you have to open the app again and disable VSync when you want to play (unless you keep the app running all the time)


Created on 8. April 2020  
Updated on 4. May 2020  
By [petak5](https://github.com/petak5)
