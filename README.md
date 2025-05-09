# Reliable-UDP-Protocol
Reliable UDP Protocol - A project that implements reliable file transfer protocol using UDP (inspired by TCP).

#### Overview
This project implements a reliable file transfer protocol using UDP with the following features:
- Sliding window protocol for flow control
- Selective acknowledgments for packet delivery confirmation
- Congestion control using AIMD (Additive Increase Multiplicative Decrease)
- Out-of-order packet handling
- Packet loss detection and retransmission
- Graphical interface for monitoring transmission

#### Components
##### 1. Sender Application (`sender_gui.py`)
**Features:**
- Congestion window visualization
- Packet transmission statistics
- Manual packet loss simulation
- Dynamic window size adjustment
- Real-time graph of:
  - Congestion window size
  - Receiver window size
  - Round-trip time (RTT)

##### 2. Receiver Application (`receiver_gui.py`)
**Features:**
- Packet reception visualization
- Buffer status monitoring
- ACK generation
- Real-time graph of:
  - Buffer usage
  - Throughput
  - Packet loss rate

##### 3. Shared Utilities (`shared_utils.py`)
**Contains:**
- Common constants (ports, buffer sizes)
- Packet formatting functions
- Network configuration
