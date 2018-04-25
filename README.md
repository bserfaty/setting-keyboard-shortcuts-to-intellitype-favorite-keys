# setting-keyboard-shortcuts-to-intellitype-favorite-keys
A reg file that sets specific keyboard shortcuts to intellitype keyboard (such as Microsoft Egronomic 4000) favorite keys 

The following is a registry that sets up keyboard shortcuts to the favorite keys.
I am using it to switch windows 10 multiple desktop (using the peach application, this can be used also with other multiple desktop enhancers ). This means that pressing the favorite 1 button gets me to desktop 1 etc.

The peach multiple desktop:
https://www.microsoft.com/store/productId/9N2P0LJBSVNF

Inspiration for my specific change was from here:
https://gist.github.com/abatkin/2304926

Get the entry ID for the button here:
http://xahlee.info/kbd/ms_keyboard/intellitype_registry.html

Keycode reference: http://msdn.microsoft.com/en-us/library/dd375731%28VS.85%29.aspx


The registry change that I did:
===============================================================================================

[HKEY_CURRENT_USER\Software\Microsoft\IntelliType Pro\ModelSpecific\1016\EventMapping\78]
"Command"=dword:0000019c
"Keystroke"=dword:00000631
"KeystrokeText"="Ctrl + Alt + 1"
"Macro"="Escape.mhm"

[HKEY_CURRENT_USER\Software\Microsoft\IntelliType Pro\ModelSpecific\1016\EventMapping\79]
"Command"=dword:0000019c
"Keystroke"=dword:00000632
"KeystrokeText"="Ctrl + Alt + 2"
"Macro"="Escape.mhm"

[HKEY_CURRENT_USER\Software\Microsoft\IntelliType Pro\ModelSpecific\1016\EventMapping\80]
"Command"=dword:0000019c
"Keystroke"=dword:00000633
"KeystrokeText"="Ctrl + Alt + 3"
"Macro"="Escape.mhm"

[HKEY_CURRENT_USER\Software\Microsoft\IntelliType Pro\ModelSpecific\1016\EventMapping\81]
"Command"=dword:0000019c
"Keystroke"=dword:00000634
"KeystrokeText"="Ctrl + Alt + 4"
"Macro"="Escape.mhm"

[HKEY_CURRENT_USER\Software\Microsoft\IntelliType Pro\ModelSpecific\1016\EventMapping\82]
"Command"=dword:0000019c
"Keystroke"=dword:00000635
"KeystrokeText"="Ctrl + Alt + 5"
"Macro"="Escape.mhm"
===============================================================================================
Instructions to get the media keys to switch desktops:
0. Have 5 desktops
1. Install peach from the link above. Run it. Make sure that you switch desktop by Ctrl-Alt-1 ... Ctrl-Alt-5
2. Copy tha above and paste it into a file with .reg extension.
3. Open task manager and find the itype.exe. Stop it.
4. Double click the .reg file
5. press start and type itype.exe

Should be working now.





