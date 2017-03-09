# systemd-suspend-prevent
A few files you can install to prevent system suspend/sleep when connected to AC.

This is only slightly modified from this post: https://nrocco.github.io/2014/06/05/suspend-prevent-systemd.html.

## INSTALL
* Put `suspend-prevent` in `/usr/local/bin` and make it executable.
* Put `suspend-prevent.service` in `/etc/systemd/system`.
* Put `50-suspend-prevent.rules` in `/etc/udev/rules.d`.
* Run `systemctl daemon-reload` and `udevadm control --reload-rules`.
