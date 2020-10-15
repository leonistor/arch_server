# Arch Linux Server Setup

## Config

### Console font

```sh
pacman -S terminus-font
setfont ter-132n
echo "FONT=ter-132n" >> /etc/vsconsole.conf
```
[wiki](https://wiki.archlinux.org/index.php/Linux_console#Fonts)

### Logs on tty12

[wiki: Forward journald to /dev/tty12](https://wiki.archlinux.org/index.php/Systemd/Journal#Forward_journald_to_/dev/tty12)
Activate console on screen: `sudo chvt 2`, works from ssh connection.

[How To Switch Between TTYs Without Using Function Keys In Linux](https://ostechnix.com/how-to-switch-between-ttys-without-using-function-keys-in-linux/)

---

## Setup

[So You Want to Setup Arch Linux Server, Eh?](https://angrysysadmins.tech/index.php/2019/04/grassyloki/so-you-want-to-setup-arch-linux-server-eh/)
[HowtoForge](https://www.howtoforge.com/tutorial/install-arch-linux-server/)

---


## Basics

[pacman tldr](https://itsfoss.com/pacman-command/). Pacman has a color option! Uncomment the Color line in `/etc/pacman.conf.`

[Keep A Command Running After You Log Out Of The SSH Session](https://ostechnix.com/4-ways-keep-command-running-log-ssh-session/)
[Search The Arch Wiki Website From Commandline](https://ostechnix.com/search-arch-wiki-website-commandline/)

[yay](https://ostechnix.com/yay-found-yet-another-reliable-aur-helper/)

Startup scripts: [here](https://stackoverflow.com/a/30956893) and [here](https://arashmilani.com/post?id=86) plus [wiki](https://wiki.archlinux.org/index.php/Systemd#Writing_unit_files)

Python PIP: `yay -S python-pip`

---

## Maintenance

[Cylon – The Arch Linux Maintenance Program For Newbies](https://ostechnix.com/cylon-arch-linux-maintenance-program/)
[Check Disk Space Usage In Linux Using Ncdu](https://ostechnix.com/check-disk-space-usage-linux-using-ncdu/)

[Network Bandwidth Utilization](https://ostechnix.com/display-network-bandwidth-utilization-using-bandwhich-tool/)

---

## Networking

[wiki: OpenSSH](https://wiki.archlinux.org/index.php/OpenSSH)

[Configure Static And Dynamic IP Address In Arch Linux](https://ostechnix.com/configure-static-dynamic-ip-address-arch-linux/)
[Which Service Is Listening On A Particular Port](https://ostechnix.com/how-to-find-which-service-is-listening-on-a-particular-port/)

### Public IP Address:

```sh
curl ipinfo.io/ip
curl eth0.me
```

---

## Security

[Find Vulnerable Packages In Arch Linux](https://ostechnix.com/find-vulnerable-packages-arch-linux/)


---

## Elixir apps

[Quick VPS Setup for Phoenix Web Framework Beginners](https://elixirforum.com/t/quick-vps-setup-for-phoenix-web-framework-beginners/20987)

