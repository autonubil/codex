# wifi

802.11 (Wi-Fi)

wifi.ssid
wifi.channel

wifi.afd.packets_drop
wifi.afd.packets_accept
wifi.afd.bytes_drop
wifi.afd.bytes_accept

## wap

Wireless Access Points

Access Controller (AC)
Wireless Termination Points (WTPs)
Station (STA)

wifi.wap.sta.mac.addr
wifi.wap.sta.ip.addr
wifi.wap.wtp.mac.addr

netif.wifi.frags.tx
netif.wifi.frames.group.tx
netif.wifi.fails
netif.wifi.retries
netif.wifi.multi_retries
netif.wifi.frames.dup
netif.wifi.successes.rts
netif.wifi.fails.rts
netif.wifi.fails.ack
netif.wifi.frags.rx
netif.wifi.frames.group.rx
netif.wifi.errors.fcs
netif.wifi.frames.tx
netif.wifi.frames.wep.undecrypt
netif.wifi.qos.frags.discard
netif.wifi.stations.assoc
netif.wifi.qos.cf.polls.rx
netif.wifi.qos.cf.polls.rx_unused
netif.wifi.qos.cf.polls.unusable
netif.wifi.qos.cf.polls.lost



	::= { dot11CountersEntry 19 }


	::= { dot11CountersEntry 20 }

dot11TransmittedAMSDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a transmitted A-MSDU is acknowledged.

		This counter shall be incremented for an acknowledged A-MSDU frame with an individual address in the Address 1 field or an A-MSDU frame with a group  address in the Address 1 field."
	::= { dot11CountersEntry 21 }

dot11FailedAMSDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when an A-MSDU is not transmitted successfully due to the number of transmit attempts exceeding either the dot11ShortRetryLimit or dot11LongRetryLimit."
	::= { dot11CountersEntry 22 }

dot11RetryAMSDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a transmitted A-MSDU is acknowledged only after one or more retransmissions.

		This counter shall be incremented when an A-MSDU is successfully transmitted after one or more retransmissions."
	::= { dot11CountersEntry 23 }

dot11MultipleRetryAMSDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a transmitted A-MSDU is acknowledged only after more than one retransmission.

		This counter shall be incremented when an A-MSDU is successfully transmitted after more than one retransmission."
	::= { dot11CountersEntry 24 }

dot11TransmittedOctetsInAMSDUCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MSDU is transmitted.

		This counter shall be incremented by the number of octets in the frame body of an A-MSDU frame when an A-MSDU frame is successfully transmitted."
	::= { dot11CountersEntry 25 }

dot11AMSDUAckFailureCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when an acknowledgment to an A-MSDU is not received when expected. This acknowledgment can be in an Ack or BlockAck frame."
	::= { dot11CountersEntry 26 }

dot11ReceivedAMSDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MSDU is received.

		This counter shall be incremented for a received A-MSDU frame with the station's MAC address in the Address 1 field or an A-MSDU frame with a group address in the Address 1 field."
	::= { dot11CountersEntry 27 }

dot11ReceivedOctetsInAMSDUCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MSDU is received.

		This counter shall be incremented by the number of octets in the frame body of an A-MSDU frame when an A-MSDU frame is received."
	::= { dot11CountersEntry 28 }

dot11TransmittedAMPDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MPDU is transmitted.

		This counter shall be incremented when an A-MPDU is transmitted."
	::= { dot11CountersEntry 29 }

dot11TransmittedMPDUsInAMPDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MPDU is transmitted.

		This counter shall increment by the number of MPDUs in the A-MPDU when an A-MPDU is transmitted."
	::= { dot11CountersEntry 30 }

dot11TransmittedOctetsInAMPDUCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MPDU is transmitted.

		This counter shall be incremented by the number of octets in the A-MPDU frame when an A-MPDU frame is transmitted."
	::= { dot11CountersEntry 31 }

dot11AMPDUReceivedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MPDU is received.

		This counter shall be incremented when the MAC receives an A-MPDU from the PHY."
	::= { dot11CountersEntry 32 }

dot11MPDUInReceivedAMPDUCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MPDU is received.

		This counter shall be incremented by the number of MPDUs received in the A-MPDU when an A-MPDU is received."
	::= { dot11CountersEntry 33 }

dot11ReceivedOctetsInAMPDUCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an A-MPDU is received.

		This counter shall be incremented by the number of octets in the A-MPDU frame when an A-MPDU frame is received."
	::= { dot11CountersEntry 34 }

dot11AMPDUDelimiterCRCErrorCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when an MPDU delimiter has a CRC error when this is the first CRC error in the received A-MPDU or when the previous delimiter has been decoded correctly."
	::= { dot11CountersEntry 35 }

dot11ImplicitBARFailureCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when the expected BlockAck frame is not received in response to an Implicit BlockAckReq frame."
	::= { dot11CountersEntry 36 }

dot11ExplicitBARFailureCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when the expected BlockAck frame is not received in response to an Explicit BlockAckReq frame."
	::= { dot11CountersEntry 37 }

dot11ChannelWidthSwitchCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the bandwidth is switched.

		This counter shall be increment when the bandwidth used is switched from 20 to 40 or vice-versa."
	::= { dot11CountersEntry 38 }

dot11TwentyMHzFrameTransmittedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a frame is transmitted only on the primary channel.

		This counter shall be incremented when a frame is transmitted only on the primary channel."
	::= { dot11CountersEntry 39 }

dot11FortyMHzFrameTransmittedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a frame is transmitted on both control and secondary channels.

		This counter shall be incremented when a frame is transmitted on both control and secondary channels."
	::= { dot11CountersEntry 40 }

dot11TwentyMHzFrameReceivedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a frame is received only on the primary channel.

		This counter shall be incremented when a frame is received only on the primary channel."
	::= { dot11CountersEntry 41 }

dot11FortyMHzFrameReceivedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a frame is received on both the control and secondary channels.

		This counter shall be incremented when a frame is received on both the control and secondary channels."
	::= { dot11CountersEntry 42 }

dot11PSMPUTTGrantDuration OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a PSMP-UTT is granted.

		This counter contains the cumulative duration of PSMP-UTT granted to the STA, in units of 4 microseconds."
	::= { dot11CountersEntry 43 }

dot11PSMPUTTUsedDuration OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a PSMP-UTT is used.

		This counter contains the cumulative duration of transmission by the STA during its allocated PSMP-UTT, in units of 4 microseconds"
	::= { dot11CountersEntry 44 }

dot11GrantedRDGUsedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an RDG is used.

		This counter at the RD initiator shall be incremented when an allocated RDG is used by the station, apart from transmitting a response frame such as Ack or BlockAck frames."
	::= { dot11CountersEntry 45 }

dot11GrantedRDGUnusedCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an RDG is not used.

		This counter at the initiator shall be incremented when an allocated RDG is not used by the station, apart from transmitting a response frame such as Ack or BlockAck frames."
	::= { dot11CountersEntry 46 }

dot11TransmittedFramesInGrantedRDGCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an RDG is used.

		This counter at the initiator shall be incremented for every frame, other than response frames such as Ack or BlockAck frames, transmitted by the station during a granted RDG."
	::= { dot11CountersEntry 47 }

dot11TransmittedOctetsInGrantedRDGCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an RDG is used.

		This counter at the initiator shall be incremented by the number of octets in the frame body of a frame, other than response frames such as Ack or BlockAck frames, transmitted by the station during a granted RDG."
	::= { dot11CountersEntry 48 }

dot11BeamformingFrameCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a frame with beamforming parameters is sent.

		This counter shall be incremented when the transmitter sends a frame with new/updated beamforming parameters."
	::= { dot11CountersEntry 49 }

dot11DualCTSSuccessCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a dual CTS is sent.

		This counter shall be incremented when AP sends a dual CTS in response to a STA initiating TXOP in extended range."
	::= { dot11CountersEntry 50 }

dot11DualCTSFailureCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a dual CTS is not sent.

		This counter shall be incremented when AP fails to send a dual CTS in response to a STA initiating TXOP in extended range."
	::= { dot11CountersEntry 51 }

dot11STBCCTSSuccessCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when no collision is detected.

		This counter shall be incremented when AP does not detect a collision PIFS after sending a CTS to self STBC frame in extended range."
	::= { dot11CountersEntry 52 }

dot11STBCCTSFailureCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a collision is detected.

		This counter shall be incremented when AP detects a collision PIFS after sending a CTS to self STBC frame in extended range."
	::= { dot11CountersEntry 53 }

dot11nonSTBCCTSSuccessCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when no collision is detected.

		This counter shall be incremented when AP does not detect a collision PIFS after sending a CTS to self that is an non-STBC frame in extended range."
	::= { dot11CountersEntry 54 }

dot11nonSTBCCTSFailureCount OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when a collision is detected.

		This counter shall be incremented when AP detects a collision PIFS after sending a CTS to self that is an non-STBC frame in extended range."
	::= { dot11CountersEntry 55 }

dot11RTSLSIGSuccessCount OBJECT-TYPE 
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when the duration/ID field is set according to the rules of L-SIG TXOP protection in the received CTS following a transmission of RTS in L-SIG TXOP protection mode."
	::= { dot11CountersEntry 56 }

dot11RTSLSIGFailureCount OBJECT-TYPE 
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This counter shall be incremented when the duration/ID field is not set according to the rules of L-SIG TXOP protection in the received CTS following a transmission of RTS in L-SIG TXOP protection mode."
	::= { dot11CountersEntry 57 }

dot11PBACErrors OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when the condition described below occurs.

		This variable indicates the number of errors encountered in the PBAC procedures."
	::= { dot11CountersEntry 58}

dot11DeniedAssociationCounterDueToBSSLoad OBJECT-TYPE
	SYNTAX Counter32
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the SME when the condition described below occurs.
		
		This counter, available at a WNM AP, shall increment when an (re)association request is denied because the AP has insufficient bandwidth to handle the additional STA."
	::= { dot11CountersEntry 59}



dot11TransmittedMSDUOctetsCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an MSDU is successfully transmitted.
		This counter is incremented by the number of octets in the MSDU when an MSDU is successfully transmitted."
	::= { dot11CountersEntry 60 }

dot11ReceivedMSDUOctetsCount OBJECT-TYPE
	SYNTAX Counter64
	MAX-ACCESS read-only
	STATUS current
	DESCRIPTION
		"This is a status variable.
		It is written by the MAC when an MSDU is received that is addressed to the STA (either individually or globally).
		This counter is incremented by the number of octets in the MSDU."
	::= { dot11CountersEntry 61 }

