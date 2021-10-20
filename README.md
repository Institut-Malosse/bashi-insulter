# bashi-insulter
Randomly insults the user when typing wrong command.

Change insults as needed :)

French insults support is currently in dev.

```bash
noob@barkshi:~ $ sl

  Y u no speak computer???

-bash: sl: command not found
noob@barkshi:~ $ gti status

  This is why nobody likes you.

-bash: gti: command not found
noob@barkshi:~ $ sp aux

  Go outside.

-bash: sp: command not found
```

# Compatibility / Dependencies
* Bash or Zsh
* wget


# Installation

    sudo wget -O /etc/bash.command-not-found https://raw.githubusercontent.com/Institut-Malosse/bashi-insulter/main/src/bash.command-not-found
* Bash : Then source the file automatically for new logins by adding the following to `/etc/bash.bashrc` or any of the other locations where you can configure your shell automatically during login:
```
if [ -f /etc/bash.command-not-found ]; then
    . /etc/bash.command-not-found
fi
```
Login again and type some invalid commands for the effects to be visible.

* Zsh : You will have to add the script to `.zshrc` at the end of the file if you are using `zsh` :

```
if [ -f /etc/bash.command-not-found ]; then
    . /etc/bash.command-not-found
fi
```
Login again and type some invalid commands for the effects to be visible.
