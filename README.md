# Cemu Language repository
This repository hosts the UI translation files for Cemu emulator.  
Want to contribute? [Read here](http://compat.cemu.info/wiki/Tutorial:How_to_translate_Cemu_UI) on how to do that.

### Use
For ease of use, I compiled all language packs into .mo files. You just need to download and replace it.
The current 'Cemu MacOS' version has a 'Bug' where some language packs do not work. You can do this by creating an 'en' folder in the Cemu language pack directory and downloading the latest language pack for your region into the 'en' folder.
You can quickly install the language pack you need through the following script, and modify the variable 'LANG' to the name of the language pack you need before using it.
```zsh
#!/bin/zsh
LANG="zh"
LANG_DIR="/Applications/Cemu.app/Contents/SharedSupport/resources"
mkdir -p "$LANG_DIR/en"
curl -# -o "$LANG_DIR/en" "https://raw.githubusercontent.com/kailous/Cemu-Language/master/resources/${LANG}/cemu.mo"
echo "Succeeded！"
```