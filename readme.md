**Command Line Args**:
- `--xhome`: Automatically login and start an xHome remote play session for the default console on start.
- `--xcloud=titleId`: Automatically login and start an xCloud remote play session. A list of titleIds are shown in the app 'Help' section.

**Permissions**:
- `-device=all` and `-filesystem=/run/udev:ro`: Detect and read connected game controllers.
- `-filesystem=/home/deck/.local/share/Steam/userdata` and `-filesystem=/home/deck/.steam`: Set xcloud custom shortcuts and artwork in steam library.

Prod
```
flatpak install flathub net.studio08.xbplay
```

Local dev
```
flatpak-builder build net.studio08.xbplay.yml --install --force-clean --user
```