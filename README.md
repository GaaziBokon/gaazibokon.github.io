# GaaziBokon
## Turn your computer into gaming console and your smartphones into gamepads!

**It's still a Work in progress!**

The idea of GaaziBokon is simple:
 - You have got a Linux computer connected to some network with [GaaziBokon server](https://github.com/gaazibokon/gaazibokon_server) installed and running on it.
 - You have got one or more smartphones with GaaziBokon client installed on them.
 - You have the computer and and smartphones connected to the same network.
 - Smartphones using the GaaziBokon client act as keyboard inputs for your computer so that you can play multi or single player games on your computer with almost no need for an external keyboard, mouse or gamepad.

## How to setup client?

The KaiOS, Android and iOS clients are to be written.

## How to setup server?

Assuming you've got `python3` installed:

 - `git clone https://github.com/gaazibokon/gaazibokon_server`
 - `cd gaazibokon_server`
 - Edit `layouts.json` to your need.
 - Put a password in `password` file so that the server will require the clients to have one if they want to connect. Possibly leave the file empty or delete it if you don't want to set a password.
 - `python3 main.py bind_address port`
 - Optionally change priority of this process
 - Optionally use something like systemd to manage it.
