

GALLIFREY GAMING SERVER DOCUMENTATION


On-server docs meant to get you started with managing the Abstraction
Gaming Evironment.


Getting Started

The best way to manage this server is remotely. If you are reading this,
you are either using the VMWare vSphere client or SSH. For vSphere, we
have set-up ports to allow internal connections to be forwarded to the
system. If you want external vSphere access, you will need to talk to
Calvin IT about opening ports 443 and 902 to the outside world. This is
_not_ reccomended, instead, you should use SSH from remote sites (i.e.
off-campus).

Allowing SSH Access

This server has been "hardened" to a degree for SSH. In order to allow a
user to access the server via SSH, you will need to add them to the
sshd_config file. you can do this by typing

    sudo nano /etc/ssh/sshd_config

to open the ssh config file for editing. At the bottom of the file, add
the line

    AllowUsers [user]@[host]

to enable access. If you only want them to access the server from
on-site, make host 153.106.*, otherwise just use * to allow access from
anywhere.

Managing Minecraft

When I (Quentin) was gaming admin, I decided to start this server from
scratch. When I did, I switched from a homebrew managment panel to an
open-source manager called "Mark2". The code may be found on github if
you want to see more.

The main command to get mark2 up and running is simple:

    mark2 start [server name]

If you are in the directory of a specific minecraft server (e.g.
/home/gamer/default/) you don't need to specify the server name. Once
the server is running, you can go to the management interface by typing

    mark2 attach

which will bring up the control panel. In here, you can switch between
servers using the top tab just by clicking on them. In each server, you
can click on users from a list on the right of the screen to bring up
kick/mute/ban options.

At the bottom of the screen, you can communciate directly with the
server. By default, the prompt silently inserts a / before your text, so
"foo" becomes "/foo" in the server. This means you don't need a leading
slash for minecraft commands. If you want to just talk as the server,
type

    say [text]

to just dump text into the chat.

Mark2 also accepts specific commands for the mark2 interface through
this prompt. You prepend any mark2 commands with a tilde (~), like so:

    ~restart 2m

To detact from the control panel, just use Ctrl+C.

Managing TF2

TODO: Get TF2 to work on this system.

--Last Updated Fri 15 Dec 2017 01:12:06 PM EST by qrb2--
