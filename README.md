# Update-Sources-Kali

So, you installed Kali 2018 and now you want to (a) update it and (b) install `open-vm-tools`?

### Step 1

Open a terminal and type

`sudo gedit /etc/apt/sources.list`

### Step 2

In the `sources.list` file, add the following lines:

`
deb http://httpredir.debian.org/debian jessie main
deb-src http://httpredir.debian.org/debian jessie main

deb http://httpredir.debian.org/debian jessie-updates main
deb-src http://httpredir.debian.org/debian jessie-updates main

deb http://security.debian.org/ jessie/updates main
deb-src http://security.debian.org/ jessie/updates main
`

Then, press SAVE and close the file.

### Step 3

In the terminal, type `sudo apt update` and wait until the update is finished.

### Step 4

In the terminal, type `sudo apt install open-vm-tools`, press Enter, and wait until the the package is installed.
