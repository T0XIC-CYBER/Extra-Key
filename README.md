____
```   TERMUX   EXTRA   KEYBOARD ```
————
💻
___
#### see documentation: https://wiki.termux.com/wiki/Touch_Keyboard

##### trying to match most physical keys, some optional keys replaced
___
**installation**

* make sure your quest is in developer mode
* download latest termux apk file (https://f-droid.org/en/packages/com.termux/)
* open adb connection to headset and push files to /sdcard
  * ```adb shell mkdir /sdcard/termux && adb push *.properties /sdcard/termux/```
* sideload apk using adb (or sidequest for the lazy ppl)
  * ```adb install -g com.termux_$ver.apk```
* open termux app in headset under 'unknown sources' 
* create directory ```.termux``` in termux home
* run ```termux-setup-storage``` to set permissions for /sdcard access
* copy files from ```/sdcard/termux/``` to ```/data/data/com.termux/files/home/.termux/```
* ```colors.properties``` is optional, adjust to your preference
  
  (uses manjaro green '#1aab9b' as terminal foreground color)
___
session handling, see (https://wiki.termux.com/wiki/Terminal_Settings)

* ```CTRL + t``` create new session
* ```CTRL + n``` rename current session
* ```CTRL + 1``` switch to previous session
* ```CTRL + 2``` switch to next session
___

**long press popup keys**
___
* long press ```ESC``` for ```CTRL + d``` (end session)
* long press ```TAB``` for ```ALT```
* long press ```CTRL``` for ```SHIFT```
* long press ```SPACE``` for ```DRAWER``` (open termux sessions)
* long press ```UP``` for ```PGUP```
* long press ```DOWN``` for ```PGDN```
* long press ```LEFT``` for ```HOME```
* long press ```RIGHT``` for ```END```
* long press ```M◂``` for ```#CMD``` (see below)
___
**helpful bash shortcuts using macros**
___
| modifier | action |
|--:|:--|
|```UPPER``` | transform word in front of cursor to UPPER case (ALT + u) |
|```LOWER``` | transform word in front of cursor to lower case (ALT + l) |
| ```#CMD``` | comment current line(command) and start new line (ALT + #) |
|  ```ARG``` | yank last argument (CTRL + SHIFT + y) |
|   ```C◂``` | backward move one word |
|   ```C▸``` | forward move one word |
|   ```M◂``` | backward delete word |

