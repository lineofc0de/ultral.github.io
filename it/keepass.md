# Keepass & SSH

I use ssh keys & have forgotten about typing passwords & accidental locking of my account.

my scheme is:

1. The ssh private key is stored in the [keepass](https://keepass.info/).
2. Keepass works as ssh-agent. It exports the ssh-key via [keeagent plugin](https://keepass.info/plugins.html#keeagent). Keeagent has to be configured in accordance to the [guide](https://keeagent.readthedocs.io/en/stable/usage/quick-start.html).
3. In the plugin I've configured "*enable agent for windows openssh*"
4. In the VSCode with the [Remote-SSH extension](https://code.visualstudio.com/docs/remote/ssh-tutorial) I set *Remote.SSH.path*  to *C:\Windows\System32\OpenSSH\ssh.exe*
5. Installed public ssh key at AWS, github, etc
