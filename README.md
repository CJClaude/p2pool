A "clone and go" repository for creating a YACCoin P2Pool system.

Change the link to point to your local wallet.  Note this should be empty, its just a transfer
point.

Change the .yaccoin/yaccoin.conf if you want, but leave in all the parameters.  Since this is a
localhost only configuration, changing the passwords is pretty optional, but probably a good idea.

If your going to mess with ports, be careful.  Two main files:

p2pool/p2pool/bitcoin/networks/yaccoin.py - contains the coins RPC and regular port
p2pool/p2pool/networks/yaccoin.py - contains worker_port - the port people will connect to

Probably best not to mess with anything else in those files.

Note you will need to port forward port 10099 in order to have your p2pool work with the others.
