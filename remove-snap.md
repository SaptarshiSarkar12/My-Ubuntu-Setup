# Remove Snap and install Flatpak
## Remove Snap
Run the following commands :
- See which snap packages are installed and remove them completely via the commands given in the 3rd step
    ```bash
    snap list
    ```
- Stop **snap services** -
    ```bash
    sudo systemctl disable snapd.service
    sudo systemctl disable snapd.socket
    sudo systemctl disable snapd.seeded.service
    ```
- Remove snap packages
    ```bash
    sudo snap remove --purge firefox
    sudo snap remove --purge snap-store
    sudo snap remove --purge gnome-3-38-2004 # Check for the version
    sudo snap remove --purge gtk-common-themes
    sudo snap remove --purge snapd-desktop-integration
    sudo snap remove --purge bare
    sudo snap remove --purge core20
    sudo snap remove --purge core22 # Other core packages might be there, uninstall them
    sudo snap remove --purge snapd
    ```
- Clear snap caches
    ```bash
    sudo rm -rf /var/cache/snapd/
    ```
- Remove snapd package
    ```bash
    sudo apt autoremove --purge snapd
    ```
- Remove snap directories
    ```bash
    rm -rf ~/snap
    ```
- To prevent snap coming back, create a new file via ```sudo nano /etc/apt/preferences.d/nosnap``` and enter the below text in it :
    ```md
    Package: snapd
    Pin: release a=*
    Pin-Priority: -10
    ```
- Run ```sudo apt update``` to update your system
- Snap gone :relieved:!
- Proceed to install Flatpak

## Install flatpak
Run the below commands to install flatpak and flathub
```bash
sudo apt install flatpak
sudo add-apt-repository ppa:flatpak/stable
sudo apt update
sudo apt install flatpak
sudo apt install gnome-software-plugin-flatpak
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```
Restart the system and then delete launchpad ppa of flatpak (as it does not contain releases) via software updater
