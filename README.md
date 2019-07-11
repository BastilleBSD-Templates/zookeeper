# perl
Bastille Template to create a Zookeeper Jail

After the jail is built and this template applied you need to do the following:

Edit the zookeeper config:

	vi /usr/local/etc/zookeeper/zoo.cfg

And modify the config accordingly:

    # The number of milliseconds of each tick
    #tickTime=2000
    # The number of ticks that the initial
    # synchronization phase can take
    #initLimit=10
    # The number of ticks that can pass between
    # sending a request and getting an acknowledgement
    #syncLimit=5
    # the directory where the snapshot is stored.
    # do not use /tmp for storage, /tmp here is just
    # example sakes.
    dataDir=/var/db/zookeeper
    # the port at which the clients will connect
    clientPort=2181
    #clientPortAddress=192.168.1.100

    # specify all zookeeper servers
    #server.1=192.168.1.101:2888:3888
    #server.2=192.168.1.102:2888:3888
    #server.3=192.168.1.103:2888:3888

