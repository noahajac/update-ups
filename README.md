# GNOME Automatic UPS Status Update

I've noticed that it often takes a long time for my UPS's actual status to be reflected in GNOME. The script [update-ups](update-ups).

There is also a [service](update-ups.service) and [timer](update-ups.timer) file for systemd. Place these files in `/etc/systemd/system/` and run `systemctl enable update-ups.timer`. This will run the update command every 6 seconds after bootup.
