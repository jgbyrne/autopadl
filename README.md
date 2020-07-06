## autopadl

`pulseaudio-dlna` is a superb utility tool which detects local DLNA receivers and generates corresponding Pulseaudio devices, facilitating seamless audio streaming.

This simple wrapper daemonises `pulseaudio-dlna`, and has a systemd unit file that allows the service to be controlled with `systemctl`.

The key facility it provides over the standalone program is the ability to dynamically allow the `pulseaudio-dlna` services through an `nftables` firewall, and then close the ports again when the service shuts down.

To install this utility, move `autopadl.rc` to `/etc/`, `autopadl.servce` to `/etc/systemd/system/` or similar, and `autopadl` to `/usr/bin/` or similar.

Feel free to package this small tool for a distribution if you wish. 
