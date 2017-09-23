# Boss10 Config Files

LinuxCNC Config files for Bridgeport Boss 10 CNC mill.


## Basic GIT Instructions

To clone this configuration via HTTPS, open a terminal in ```~linuxcnc/configs``` and run

```git clone https://github.com/KurtJacobson/Boss10_config.git```

or if you are using SSH run

```git clone git@github.com:KurtJacobson/Boss10_config.git```

To update the local config run

```git pull origin master```

To push changes to the remote (i.e. github) run

```git push origin master```


## Setting Up SSH

Using SSH alows you to push to GitHub without having to enter a password each time, which is highly conveniant.


#### Generate a new SSH key pair

Generate public/private rsa key pair, using your GitHub email as a label.

```ssh-keygen -t rsa -b 4096 -C "your_email@example.com"```

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.
You will then be prompted to "Enter passphrase", this is not really necessary so simply press Enter again to skip.


#### Add the SSH key to the ssh-agent

Start the ssh-agent in the background.

```eval "$(ssh-agent -s)"```

Add your SSH private key to the ssh-agent.

```ssh-add ~/.ssh/id_rsa```

Add the public key to GitHub in **Settings** > **SSH and GPG Keys**
