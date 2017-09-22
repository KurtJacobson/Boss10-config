# Bridgeport_Boss10

LinuxCNC Config files for Bridgport Boss 10 CNC mill using AMC 25A20 servo drives.



## Setting Up SSH

### Generate a new SSH key pair

Generate public/private rsa key pair, using your GitHub email as a label.

```ssh-keygen -t rsa -b 4096 -C "your_email@example.com"```

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

Enter a file in which to save the key (/home/you/.ssh/id_rsa): [Press enter]
Enter passphrase (empty for no passphrase): [Type a passphrase]
Enter same passphrase again: [Type passphrase again]

### Add the SSH key to the ssh-agent

Start the ssh-agent in the background.

```eval "$(ssh-agent -s)"```

Add your SSH private key to the ssh-agent. 

```ssh-add ~/.ssh/id_rsa```

Add the public key to GitHub
