# Simple Byzantine Fault Tolerance (BFT) Consensus Protocol
This repository contains a Python implementation of a simplified Byzantine Fault Tolerance (BFT) consensus protocol, often used in blockchain networks.

## Overview
The BFT consensus protocol allows a network of nodes to reach agreement on a proposed block, despite the potential presence of faulty nodes. This simulation models the flow of message exchange between nodes and the steps taken in the process of reaching consensus.

## The main components in this code include:

1. **Message:** This is a generic class representing a message sent between nodes in the system. It contains a sender, receiver, and content.

2. **BlockProposal, Prevote, Precommit:** These classes, each a subclass of Message, represent specific types of messages that can be sent during the consensus process.

3. **Node:** This class represents a node in the system. Each node has a name and methods to propose a block (propose) and receive a message (receive_message).

4. **Messaging Queue:*** This global list simulates a messaging system between nodes.

## Execution Flow
1. A list of nodes is created.
2. One node proposes a block.
3. Nodes process incoming messages in a loop until all nodes have committed the block.
4. Running the Code

## Limitations
This is a simplified implementation for learning purposes and does not include several features of a real BFT consensus protocol, such as:

- Handling Byzantine nodes (nodes that can act arbitrarily).
- Network latency.
- Asynchronous communication.
- Persistence of the blockchain state.
- Some parts of the Node class are not fully implemented.

## Future Work
There are plans to improve upon this simplified implementation to more accurately model a real BFT consensus protocol, including addressing its current limitations.

License
This project is licensed under the MIT License. See the LICENSE file for details.
