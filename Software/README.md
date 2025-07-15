# Software
The two documents you will need to ensure the ability to use Via are the qmk-compiled default firmware ```bcmp.uf2``` as well as the ```via.json``` file which gives Via the correct key mappings and layouts to interface with the qmk-compiled code. Note that Via may be painfully slow or unresponsive when authorizing this keyboard, but if you check the Settings tab or inspect the page or check the console, you can see that these are the correct steps. 
## Flashing the board with default firmware
1. Set the board to bootloader mode. If the board is brand new and unprogrammed, then it will automatically be in bootloader mode upon plugin, however, if there is already code, then press the *BOOT* button as the board is being plugged in. After releasing the *BOOT* button, the board will be in bootloader mode and appear as a drive called ```RPI-RP2```.
2. Copy the ```bcmp.uf2``` file into the ```RPI-RP2``` drive. After this, the board will disconnect as a drive and reappear as a keyboard, complete with the default firmware.
## Programming with Via
1. Visit ```https://usevia.app/``` on your browser.
2. Go to the Settings tab and toggle the "Show Design tab" option on. There should be a new menu option appear, and this is the Design tab.
3. Go to the Design tab and click the option to "Load Draft Definition". Find the ```via.json``` file and load this as the draft definition. The entry "Jaron's Business Card Macro Pad" should appear under the "Draft Definitions" section.
4. Go to the Configure tab and click the "Authorize device +" button. Then authorize "Jaron's Business Card Macro Pad".