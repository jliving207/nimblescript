======================================================
# SSH into GPU Cloud with what ever provider you choose (must have ssh-key set up)
===============================================================================
ssh 1x1x1x1x1x-x6x6x6x6@ssh.runpod.io -i ~/.ssh/id_ed25519
======================================
# Install tmux on your GPU cloud
=======================================
/**
apt install tmux

tmux new -s nim
**\
========================================
# Launch Nimble Miner in 3 short commands
=======================================
/**
git clone https://github.com/jliving207/nimblescript.git

chmod +x nimblescript/onetrain

nimblescript/onetrain
**\
===========================================
# Detach, exit and then reconnect and attach (as many times as you want)
===========================================
CTRL-B + D (To detach)

tmux ls (list sessions)
tmux a -t nim (re attach to session)
==============================================
