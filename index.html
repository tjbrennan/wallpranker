#!/bin/bash

url="https://tjbrennan.github.io/wallpranker/images/img1.jpg"
tmpfile=$(mktemp "/tmp/wallpranker_img.XXXXXX")

function wallpaper_osx () {
osascript <<END
  tell Application "System Events"
  set theDesktops to a reference to every desktop
  repeat with theItem in theDesktops
    set the picture of theItem to POSIX file "$1" as alias
  end repeat
  end tell
END
}

function wallpaper_linux () {
  gsettings set org.gnome.desktop.background picture-uri file://"$1";
}

wget -q -O "$tmpfile" "$url" || curl -s -o "$tmpfile" "$url" || exit 1

if [[ "$OSTYPE" == "darwin"* ]]; then
  wallpaper_osx "$tmpfile"
elif [[ "$OSTYPE" == *"linux"* ]]; then
  wallpaper_linux "$tmpfile"
else
  echo "$OSTYPE not supported"
fi

clear
