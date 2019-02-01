# RSA Key for the SSH server
Original info https://superuser.com/questions/8077/how-do-i-set-up-ssh-so-i-dont-have-to-type-my-password
## Generate Generate a SSH key (if you don't have one)
run ``ssh-keygen -t RSA`` to generate a keypair
The program will ask you for a passphrase and a location where to save the new key. Using the suggested default path is recommended because all other tools will look for it there.
## Upload the public key to the remote server
run  ``ssh-copy-id -i ~/.ssh/id_rsa.pub remote-user@remote-host`` in the terminal.
## Load the key into the ssh agent
Loading the key is a simple matter of executing ssh-add and giving it the pass phrase.
## Conclusion 
If everything was done correctly, using ssh user@server will not prompt you for a password. If something is wrong with the agent and not the key, you will be asked to type in the pass phrase for the key, and not the password for the user account.

Anything that uses ssh for communication will work without entering the user account password when the correct key is loaded in the agent. Programs such as scp, sftp and rsync make use of this.   

If you want to read more on this topic here is a wiki with more info  https://wiki.archlinux.org/index.php/SSH_keys 
