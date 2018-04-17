# wsl-translinux

This is an apt repository for packages specific to the Windows Subsystem for Linux.

## Usage

To use this repository, add a new file (`wsl-translinux.list` might be a good name) to your `/etc/apt/sources.list.d` folder containing the following line (preferred), or else edit your `/etc/apt/sources.list` file to contain the following line:

`deb https://cerebrate.github.io/wsl-translinux/ xenial main`

Then install the wsl-translinux.key repository signing key. You can do this with the command:

`wget -qO - https://github.com/cerebrate/wsl-translinux/blob/master/wsl-translinux.key\?raw\=true | sudo apt-key add -`

Then run the following:

`sudo apt-get update`

After that, you can use apt-get to install packages from this repository as normal.

## Package authors

If you would like to have your WSL-specific apt package included in this repository, just send us a pull request against the `gh-pages` branch with your .deb included in the incoming folder, and we'll get right on that.

Thanks!
