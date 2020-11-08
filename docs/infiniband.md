# infiniband

netif.infiniband.bytes.out
Total octets, divided by 4, transmitted on all VLs. This includes all octets between (and not including) the start of packet delimiter and the VCRC, and may include packets containing errors It excludes all link packets.

netif.infiniband.bytes.in
Total octets, divided by 4, received on all VLs. This includes all octets between (and not including) the start of packet delimiter and the VCRC, and may include packets containing errors It excludes all link packets.

netif.infiniband.packets.out
Total packets transmitted on all VLs from this port. This may include packets with errors and excludes link packets.

netif.infiniband.packets.in
Total packets, including packets containing errors and excluding link packets, received from all VLs on the port.

netif.infiniband.errors.symbol
The interpretation of symbols within the packet is done on the HCA/CA. If the translation or interpretation fails, it creates a minor event called a symbol error. 99% of all !SymbolErrors are hardware related. If the counts are small (small being a relative term that is up for interpretation) they can be ignored. If the numbers are large and/or the same CA is reporting this error regularly it should be looked into.

netif.infiniband.errors.recovered
Total number of times the Port Training state machine has successfully completed the link error recovery process.

netif.infiniband.link.downs
Usually associated with a node reboot. If not associated with a reboot, could be a failing connection.

netif.infiniband.errors.in
These errors can be due to local physical errors, local buffer overruns, or receiving a malformed packet.

netif.infiniband.errors.remote_phys.in
The total number of packets marked with the EBP delimiter received on the port. The idea is that an "End Bad Packet" can be used instead of EGP (End Good Packet) whenever you know there is something wrong with the packet. So, if a packet is passing through the fabric and some port notices a problem (i.e. bad CRC), it will end it with EBP instead of EGP. If the packet progress requires store-and-forward, an option would be to just drop it and not waste bandwidth sending EBP packets. The CA that reports this error is NOT where the corruption occurred. It occurred elsewhere in the fabric.

netif.infiniband.switch_relay.in
This field counts the number of packets that could not be forwarded by the switch.

netif.infiniband.discards.out
This counter tracks packets that were discarded instead of transmitted. This usually indicates congestion in the fabric. The CA this packet was supposed to be sent to cannot accept it. After so many retries and/or too many incoming packets, the packet to be transmitted gets dropped. If the fabric is being routed well, without deadlocks or credit loops, these should be transient.

netif.infiniband.errors.constaint.out
The number of packets not transmitted by a port in the fabric.

netif.infiniband.errors.constaint.in
The number of packets received and discarded on a port in the fabric.

netif.infiniband.errors.local_link_integrity
The number of times that the count of local physical errors exceeded the threshold specified by LocalPhyErrors

netif.infiniband.errors.excess_buffer_overrun
This counter tracks packets that were discarded instead of transmitted. This usually indicates congestion in the fabric. The CA this packet was supposed to be sent to cannot accept it. After so many retries and/or too many incoming packets, the packet to be transmitted gets dropped. If the fabric is being routed well, without deadlocks or credit loops, these should be transient.

netif.infiniband.drops.vl15
VL15 is the default virtual lane for management packets. They are the first to be dropped when there are resource limitations on the port. This is usually related to not enough space in the buffers. In many instances these errors can be ignored. There have been instances, however, when these messages were very closely correlated to user problems in time and fabric space. Obviously, if they are being dropped the buffers are being kept very busy with other data and therefore could indicate congestion.
