#### Install instructions
Copy the theme folder into the Plymouth theme directory.

- `sudo cp -r Windows7/Plymouth/Windows7 /usr/share/plymouth/themes/`

Add to default.plymouth

- `sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/Windows7/Windows7.plymouth 100`


Choose the theme to load. (As you run the following command there will be a number assigned to each theme and located in the first column of a list. Use that number to specify the theme and press enter to continue.)

- `sudo update-alternatives --config default.plymouth`

Update initramfs

- `sudo update-initramfs -u`
