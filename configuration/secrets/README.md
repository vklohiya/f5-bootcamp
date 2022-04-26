# Create a Secret containing some SSH keys:

kubectl create secret generic ssh-key-secret --from-file=ssh-privatekey=~/.ssh/id_rsa --from-file=ssh-publickey=~/.ssh/id_rsa.pub


