# Pi-Kiosk

> Example files with the changes required to make a Pi boot cleanly, directly into fullscreen browser

## Files/changes
  **browser.desktop goes in ~/.config/autostart**
- **/boot/cmdline.txt**
  - console=tty3
  - loglevel=3
  - vt.global_cursor_default=0
  - silent
  - logo.nologo
- **/boot/config.txt**
  - disable_splash=1
  - disable_overscan=1
  - this file also includes some nerdy attempts to enforce 59.94 for use with ATEM video switcher
- **etc/xdg/lxsession/LXDE-pi/desktop.conf**
  - maybe no changes needed?
- **/etc/lightdm/lightdm-gtk-greeter.conf**
  - [greeter] background=#000000
- **rc.download**
  - nerdy attempts to enforce 59.94 for use with ATEM video switcher