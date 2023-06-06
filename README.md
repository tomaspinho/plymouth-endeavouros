# plymouth-theme-endeavouros

A Plymouth theme that uses a EndeavourOS wallpaper and color scheme. Supports a password dialog, boot progress, capslock state, etc.

## Installation
The recommended way to use this in EndeavourOS is to use this theme with the `plymouth-git` AUR package which is newer and has more features (including capslock state support).

Run:

```
# Install theme and the recommended version of Plymouth
yay -Sy plymouth-git plymouth-theme-endeavouros

# Add the "splash" kernel parameter so Plymouth is shown on boot
sudo sed -i '$ s/$/ splash/' /etc/kernel/cmdline

# So Plymouth and theme are immediately installed in your initramfs for next boot. Future kernel upgrades will include Plymouth and this theme automatically.

sudo reinstall-kernels
```