# freebsd-pkg-list-replication
Simple bash tool to print out a list of locally installed packages to a remote server.

Must have bash installed on the machines to run. Place in your local bin and run:

``` pkg-replication [remote server username] [remote server ip] [port (optional, default 22)]```

The output will be a txt file called _pkg-replication.txt_. SSH into the remote machine and run ```pkg install -y `cat pkg-replication.txt` ``` to begin installing the packages.

I made this to make replicating new FreeBSD machines easier for my production environment, I hope it will help you.
