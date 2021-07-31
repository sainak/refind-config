## rEFInd-clean


Copy the `themes` folder and `refind.conf` in your `esp/EFI/refind-directory`

```shell
git clone --depth=1 https://github.com/sainAk/refind-config.git
sudo cp -r refind-config/{themes, refind.conf} /boot/efi/EFI/refind/
```

Remember to verify UUIDs and paths before installing this conf file.
to get the PARTUUID use this command:

```shell
lsblk -p -o NAME,LABEL,PARTUUID
```

### preview

![screenshot](.github/refind.png)

credits: https://github.com/bobafetthotmail/refind-theme-regular