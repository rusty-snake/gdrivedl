GDriveDL-GUI (Linux only)
=========================

[![maintenance-status: as-is (as of 2021-01-08)](https://img.shields.io/badge/maintenance--status-as--is_%28as_of_2021--01--08%29-yellow)](https://gist.github.com/rusty-snake/574a91f1df9f97ec77ca308d6d731e29)

Graphical wrapper for GDriveDL using bash and zenity.

Installation
------------

1. Make sure `~/.local/bin` is in `$PATH`.
2. Clone this repo (`git clone "https://github.com/rusty-snake/gdrivedl.git" && cd gdrivedl/GDriveDL`).
3. Execute the commands below to install GDriveDL-GUI to your home.
```
install -Dm0755 GDriveDL "$HOME"/.local/bin/GDriveDL
install -Dm0755 ../gdrivedl.py "$HOME"/.local/bin/gdrivedl.py
install -Dm0644 GDriveDL.desktop "$HOME"/.local/share/applications/GDriveDL.desktop
install -Dm0644 GDriveDL.png "$HOME"/.local/share/pixmaps/GDriveDL.png
sed -i -e "s|@HOME@|$HOME|" "$HOME"/.local/share/applications/GDriveDL.desktop
```

Usage
-----

1. Start GDriveDL from the menu in your DE
2. Enter a GDrive URL
3. Wait for the download to finish
