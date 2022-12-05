# Layer-2-Light-Clients

##Abstract
Ethereum light clients are known to suffer from a probabilistic security model, but they are widely assumed to be secure under normal operating conditions. [^1]: Saanteri Paavolainen & Christopher Carr, "Security Properties of Light Clients on the Ethereum Blockchain", https://uwe-repository.worktribe.com/OutputFile/6764897, June 2020
The idea is to have RPC-based wallet completely trustless by first syncing to the latest header of the beacon chain and then use the eth_getProof endpoint to get the balance plus a proof that it is actually part of the root hash that we obtained. Using Merkle Inclusion proofs to the latest block header allows us to verify that the data is correct. 


##Scope
Identification of risk factors and vulnerabilities of current light clients  and how to mitigate them and provide secured solutions while further promoting better decentralization practices for all Layer 2 chains and bridges. Create an interoperable secured Light client solution for all Layer 2 chains and bridges.

##Goals 
At bare minimum to be able to build a light client that can verify on each individual layer 2 chains as well as implementing a verification using the consensus protocol of the beacon ETH mainnet chain

Another success factor is we can allow the light client to contribute to the gossip network and therefore able to help persistently validate the other requests in the network

##Problem trying to solve
Will full nodes, the network participants are required to evaluate every transaction starting from the genesis block, which requires a large amount of network, computing, and storage resources. This is impractical for many devices with either limited computing resources or intermittent network connectivity. Light clients attempt to solve this but there's still lack of information on how to use light clients especially on later 2's. Moreso we're looking to solve the problem of verying bothe the trasactions on each respective layer 2 chains as well as against the transaction that they'd be writing in the ethereum mainnet. 

##How does this project benefit the greater Ethereum ecosystem?
Since the research would be open-source, developers would be able to utilize these layer 2 light clients to build better and more secured dapps. Users would be able to would be able to verify transactions more easily and securely without having to utilized alot of resources for a full node or even to rely on "sort of central" light protocol servers. Also the ethereum ecosystem would be able to benefit on light clients not just verifying the transactions only for themeselves but maybe able to pass on those log messages to other users and contribute to a more decentralized system. 
