<iframe src="https://store.steampowered.com/widget/2693120/?t=Now%20available%20on%20Steam%20for%20Windows%2C%20Mac%2C%20and%20Linux!" frameborder="0" width="646" height="190"></iframe>

[![Available on Steam](https://www.dropbox.com/scl/fi/6qqguxkkxi4xp4379j5rn/Screenshot-2023-12-06-002714.png?rlkey=ycjz5dnnnw5zz32z1pxicqfa1&raw=1)](https://store.steampowered.com/app/2693120/XBPlay/?snr=1_5_1100__1100&utm_source=steamwidget)

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
