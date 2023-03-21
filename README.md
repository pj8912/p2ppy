# p2ppy
Peer-to-Peer Network in Python


## Boot Node
A boot node in a peer-to-peer (P2P) network is a node that serves as an initial point of contact for other nodes to join the network.

When a new node wants to join a P2P network, it needs to know the IP address and port number of at least one existing node in the network. The new node can then connect to the boot node and request a list of other nodes in the network. This allows the new node to establish connections to multiple nodes in the network and start participating in the P2P network.



## Working


- When a node starts, it acts as a client and connects to the bootnode to request the peer list.
- The bootnode sends the current peer list to the connecting node.
- After receiving the peer list, the node updates its local peer list and starts acting as a server, listening for incoming connections.
- The server component of the node periodically connects to the bootnode to update its local peer list and also to notify the bootnode about its presence in the network.
- The bootnode maintains an updated peer list based on the information it receives from the nodes in the network.


## Configuration

- Configure address based on where you run your bootnode



