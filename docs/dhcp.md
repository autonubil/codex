# `dhcp`

dhcp.op.id
dhcp.op.name
dhcp.hw_type.id
dhcp.hw_type.name
dhcp.hw_addr.size
dhcp.relay_hops
dhcp.id
dhcp.duration
dhcp.flags
dhcp.flag.bcast
dhcp.client.ip.addr
dhcp.client.mac.addr
dhcp.client.host.name
dhcp.offer.ip.addr
dhcp.next_server.ip.addr
dhcp.server.name
dhcp.relay.ip.addr
dhcp.file

dhcp.pool.id
dhcp.pool.name
dhcp.pool.size.config
dhcp.pool.size.actual
dhcp.leases.in_grace
dhcp.leases.active
dhcp.leases.expire
dhcp.leases.grace_expire
dhcp.leases.renew
dhcp.leases.max
dhcp.leases.min
dhcp.leases.avg
dhcp.offers.sent
dhcp.offers.accept
dhcp.reqs.grant
dhcp.reqs.decline
dhcp.reqs.timeout

dhcp.opt.id
dhcp.opt.name
dhcp.opt.msg_type.id
dhcp.opt.msg_type.name
dhcp.opt.subnet.mask
dhcp.opt.time_offset
dhcp.opt.router.ip.addr[]
dhcp.opt.time_server.ip.addr[]
dhcp.opt.name_server.ip.addr[]
dhcp.opt.domain_server.ip.addr[]
dhcp.opt.log_server.ip.addr[]
dhcp.opt.quotes_server.ip.addr[]
dhcp.opt.lpr_server.ip.addr[]
dhcp.opt.impress_server.ip.addr[]
dhcp.opt.rlp_server.ip.addr[]
dhcp.opt.host.hostname
dhcp.opt.class_id
dhcp.opt.param_list
dhcp.opt.local_domain
dhcp.opt.ip_lease_time

13:  "Boot File Size",                    // Size of boot file in 512 byte chunks [RFC2132]
14:  "Merit Dump File",                   // Client to dump and name the file to dump it to [RFC2132]
15:  "Domain Name",                       // The DNS domain name of the client [RFC2132]
16:  "Swap Server",                       // Swap Server address [RFC2132]
17:  "Root Path",                         // Path name for root disk [RFC2132]
18:  "Extension File",                    // Path name for more BOOTP info [RFC2132]
19:  "IP Forward On/Off",                 // Enable/Disable IP Forwarding [RFC2132]
20:  "Source Routing On/Off",             // Enable/Disable Source Routing [RFC2132]
21:  "Routing Policy Filter",             // Routing Policy Filters [RFC2132]
22:  "Max DG Assembly",                   // Max Datagram Reassembly Size [RFC2132]
23:  "Default IP TTL",                    // Default IP Time to Live [RFC2132]
24:  "Path MTU Timeout",                  // Path MTU Aging Timeout [RFC2132]
25:  "Path MTU Plateau",                  // Path MTU Plateau Table [RFC2132]
26:  "MTU Interface",                     // Interface MTU Size [RFC2132]
27:  "MTU Subnet",                        // All Subnets are Local [RFC2132]
28:  "Broadcast Address",                 // Broadcast Address [RFC2132]
29:  "Mask Discovery",                    // Perform Mask Discovery [RFC2132]
30:  "Mask Supplier",                     // Provide Mask to Others [RFC2132]
31:  "Router Discovery",                  // Perform Router Discovery [RFC2132]
32:  "Router Request",                    // Router Solicitation Address [RFC2132]
33:  "Static Route",                      // Static Routing Table [RFC2132]
34:  "Trailers",                          // Trailer Encapsulation [RFC2132]
35:  "ARP Timeout",                       // ARP Cache Timeout [RFC2132]
36:  "Ethernet",                          // Ethernet Encapsulation [RFC2132]
37:  "Default TCP TTL",                   // Default TCP Time to Live [RFC2132]
38:  "Keepalive Time",                    // TCP Keepalive Interval [RFC2132]
39:  "Keepalive Data",                    // TCP Keepalive Garbage [RFC2132]
40:  "NIS Domain",                        // NIS Domain Name [RFC2132]
41:  "NIS Servers",                       // NIS Server Addresses [RFC2132]
42:  "NTP Servers",                       // NTP Server Addresses [RFC2132]
43:  "Vendor Specific",                   // Vendor Specific Information [RFC2132]
44:  "NETBIOS Name Servers",              // NETBIOS Name Servers [RFC2132]
45:  "NETBIOS Datagram Distribution",     // NETBIOS Datagram Distribution [RFC2132]
46:  "NETBIOS Node Type",                 // NETBIOS Node Type [RFC2132]
47:  "NETBIOS Scope",                     // NETBIOS Scope [RFC2132]
48:  "X Window Font Server",              // X Window Font Server [RFC2132]
49:  "X Window Display Manager",          // X Window Display Manager [RFC2132]
50:  "Requested IP",                      // Requested IP Address [RFC2132]
52:  "Overload",                          // Overload "sname" or "file" [RFC2132]
54:  "DHCP Server ID",                    // DHCP Server Identification [RFC2132]
56:  "DHCP Message",                      // DHCP Error Message [RFC2132]
57:  "DHCP Max Message Size",             // DHCP Maximum Message Size [RFC2132]
58:  "DHCP Renewal Time",                 // DHCP Renewal (T1) Time [RFC2132]
59:  "DHCP Rebinding Time",               // DHCP Rebinding (T2) Time [RFC2132]
61:  "Client ID",                         // Client Identifier [RFC2132]
62:  "NetWare/IP Domain",                 // NetWare/IP Domain Name [RFC2242]
63:  "NetWare/IP Sub_Option",             // NetWare/IP sub Options [RFC2242]
64:  "NIS+ Client Domain",                // NIS+ v3 Client Domain Name [RFC2132]
65:  "NIS+ Server",                       // NIS+ v3 Server Addresses [RFC2132]
66:  "TFTP Server Name",                  // TFTP Server Name [RFC2132]
67:  "Boot File Name",                    // Boot File Name [RFC2132]
68:  "Home Agent",                        // Home Agent Addresses [RFC2132]
69:  "SMTP Server",                       // Simple Mail Server Addresses [RFC2132]
70:  "POP3 Server",                       // Post Office Server Addresses [RFC2132]
71:  "NNTP Server",                       // Network News Server Addresses [RFC2132]
72:  "WWW Server",                        // WWW Server Addresses [RFC2132]
73:  "Finger Server",                     // Finger Server Addresses [RFC2132]
74:  "IRC Server",                        // Chat Server Addresses [RFC2132]
75:  "StreetTalk Server",                 // StreetTalk Server Addresses [RFC2132]
76:  "STDA Server",                       // ST Directory Assist. Addresses [RFC2132]
77:  "User Class Info",                   // User Class Information [RFC3004]
78:  "Directory Agent",                   // directory agent information [RFC2610]
79:  "Service Location Agent Scope",      // service location agent scope [RFC2610]
80:  "Rapid Commit",                      // Rapid Commit [RFC4039]
81:  "Client FQDN",                       // Fully Qualified Domain Name [RFC4702]
82:  "Relay Agent Info",                  // Relay Agent Information [RFC3046]
83:  "iSNS",                              // Internet Storage Name Service [RFC4174]
85:  "NDS Servers",                       // Novell Directory Services [RFC2241]
86:  "NDS Tree Name",                     // Novell Directory Services [RFC2241]
87:  "NDS Context",                       // Novell Directory Services [RFC2241]
88:  "BCMCS Controller Domain Name List", // [RFC4280]
89:  "BCMCS Controller Address",          // [RFC4280]
90:  "Authentication",                    // Authentication [RFC3118]
91:  "Client Last Transaction Time",      // [RFC4388]
92:  "Associated IP",                     // [RFC4388]
93:  "Client System",                     // Client System Architecture [RFC4578]
94:  "Client NDI",                        // Client Network Device Interface [RFC4578]
95:  "LDAP",                              // Lightweight Directory Access Protocol [RFC3679]
97:  "UUID/GUID",                         // UUID/GUID_based Client Identifier [RFC4578]
98:  "User_Auth",                         // Open Group's User Authentication [RFC2485]
99:  "GEOCONF_CIVIC",                     // [RFC4776]
100: "PCode",                             // IEEE 1003.1 TZ String [RFC4833]
101: "TCode",                             // Reference to the TZ Database [RFC4833]
108: "IPv6_Only Preferred",               // Number of seconds before retrying DHCPv4 [draft_ietf_dhc_v6only_03]
109: "DHCP4O6_S46_SADDR",                 // DHCPv4 over DHCPv6 Softwire Source Address Option [RFC8539]
112: "NetInfo Parent Address",            // NetInfo Parent Server Address [RFC3679]
113: "NetInfo Parent Tag",                // NetInfo Parent Server Tag [RFC3679]
114: "DHCP Captive_Portal",               // DHCP Captive_Portal [RFC_ietf_capport_rfc7710bis_10]
116: "DHCP Auto_Config",                  // DHCP Auto_Configuration [RFC2563]
117: "Name Service Search",               // Name Service Search [RFC2937]
118: "Subnet Selection",                  // Subnet Selection Option [RFC3011]
119: "DNS Domain Search",                 // DNS domain search list [RFC3397]
120: "SIP Servers DHCP",                  // SIP Servers DHCP Option [RFC3361]
121: "Classless Static Route",            // Classless Static Route Option [RFC3442]
122: "CCC",                               // CableLabs Client Configuration [RFC3495]
123: "GeoConf",                           // GeoConf Option [RFC6225]
124: "V_I Vendor Class",                  // Vendor_Identifying Vendor Class [RFC3925]
125: "V_I Vendor_Specific Info",          // Vendor_Identifying Vendor_Specific Information [RFC3925]
128: "TFTP Server",
129: "Call Server",
130: "Ethernet Interface", // Variable length string.
131: "Remote Stats Server",
132: "IEEE 802.1Q VLAN ID",
133: "IEEE 802.1D/p Layer_2 Priority",
134: "DSCP",
135: "HTTP Proxy",
136: "PANA_AGENT",                    // [RFC5192]
137: "V4_LOST",                       // [RFC5223]
138: "CAPWAP_AC_V4",                  // CAPWAP Access Controller addresses [RFC5417]
139: "IPv4_Address_MoS",              // A series of suboptions [RFC5678]
140: "IPv4_FQDN_MoS",                 // A series of suboptions [RFC5678]
141: "SIP UA Config Service Domains", // List of domain names to search for SIP User Agent Configuration [RFC6011]
142: "IPv4_Address_ANDSF",            // ANDSF IPv4 Address Option for DHCPv4 [RFC6153]
143: "V4_SZTP_REDIRECT",              // This option provides a list of URIs for SZTP bootstrap servers [RFC8572]
144: "GeoLoc",                        // Geospatial Location with Uncertainty [RFC6225]
145: "FORCERENEW_NONCE_CAPABLE",      // Forcerenew Nonce Capable [RFC6704]
146: "RDNSS Selection",               // Information for selecting RDNSS [RFC6731]
150: "TFTP Server",                   // [RFC5859]
151: "status_code",                   // Status code and optional N byte text message describing status. [RFC6926]
152: "base_time",                     // Absolute time (seconds since Jan 1, 1970) message was sent. [RFC6926]
153: "start_time_of_state",           // Number of seconds in the past when client entered current state. [RFC6926]
154: "query_start_time",              // Absolute time (seconds since Jan 1, 1970) for beginning of query. [RFC6926]
155: "query_end_time",                // Absolute time (seconds since Jan 1, 1970) for end of query. [RFC6926]
156: "dhcp_state",                    // State of IP address. [RFC6926]
157: "data_source",                   // Indicates information came from local or remote server. [RFC6926]
158: "V4_PCP_SERVER",                 // Variable; the minimum length is 5. Includes one or multiple lists of PCP server IP addresses; each list is treated as a separate PCP server. [RFC7291]
159: "V4_PORTPARAMS",                 // This option is used to configure a set of ports bound to a shared IPv4 address. [RFC7618]
161: "MUD_URL_V4",                    // Manufacturer Usage Descriptions [RFC8520]
175: "Etherboot",
176: "IP Telephone",
177: "Etherboot",
208: "PXELINUX Magic",           // magic string = F1:00:74:7E [RFC5071][Deprecated]
209: "Configuration File",       // Configuration file [RFC5071]
210: "Path Prefix",              // Path Prefix Option [RFC5071]
211: "Reboot Time",              // Reboot Time [RFC5071]
212: "6RD",                      // 6RD with N/4 6rd BR addresses [RFC5969]
213: "V4_ACCESS_DOMAIN",         // Access Network Domain Name [RFC5986]
220: "Subnet Allocation",        // Subnet Allocation Option [RFC6656]
221: "Virtual Subnet Selection", // [RFC6607]
255: "End",