# snip

Single-click area snipping app.

* Get [Xnip](https://apps.apple.com/us/app/xnip-screenshot-annotation/id1221250572?mt=12).
* Create `Automator` -> `New` -> `Application`.

```AppleScript
    on run {input, parameters}
        
        tell application "System Events"
            # press command+shift+x (Xnip default hotkey)
            key code 7 using {command down, shift down}
        end tell
        
        return input
    end run
```

* `Command+C` -> `Command+V` any icon [like so](https://apple.stackexchange.com/a/372)
* For sharing create `.dmg` via `Disk Utility` [like so](https://gist.github.com/jadeatucker/5382343).
