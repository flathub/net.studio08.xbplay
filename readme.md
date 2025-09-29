**Command Line Args**:
- `--xhome`: Automatically login and start a xHome remote play session for the default console on start.
- `--xcloud=titleId`: Automatically login and start an xCloud remote play session. A list of titleIds are shown in the app 'Tips' section.

**Permissions**:
- `-device=all` and `-filesystem=/run/udev:ro`: Detect and read connected game controllers.
- `-filesystem=/home/deck/.local/share/Steam/userdata`: Set steam deck game artwork and icons.

Prod
```
flatpak install flathub net.studio08.xbplay
```


Local dev
```
flatpak-builder build net.studio08.xbplay.yml --install --force-clean --user
```
