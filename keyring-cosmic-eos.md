**COSMIC KEYRING**

*Needed for Brave and such apps.

>Install gnome-keyring

```
sudo pacman -S gnome-keyring seahorse
```

>Change `login` file

```
micro /etc/pam.d/login
```

>Enter

```
# my stuff
auth optional pam_gnome_keyring.so
session optional pam_gnome_keyring.so auto_start
```

>Changing this file it doesn't work

```
micro /etc/pam.d/greetd
```

LINK: https://wiki.archlinux.org/title/GNOME/Keyring#Integration_with_applications
