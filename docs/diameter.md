# `diameter`

diameter.version.ver
diameter.msg_size

diameter.flags.bits
diameter.flags.tags
diameter.flags.label
diameter.flags.r
diameter.flags.p
diameter.flags.e
diameter.flags.t

diameter.cmd.code

Attribute | Value
--- | ---
**IE Name** | .code
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

diameter.cmd.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

```text
AA-Request	AAR	265	Diameter NAS Application - RFC 7155
AA-Answer	AAA	265	Diameter NAS Application - RFC 7155
Diameter-EAP-Request	DER	268	Diameter EAP Application - RFC 4072
Diameter-EAP-Answer	DEA	268	Diameter EAP Application - RFC 4072
Abort-Session-Request	ASR	274	Diameter base
Abort-Session-Answer	ASA	274	Diameter base
Accounting-Request	ACR	271	Diameter base
Accounting-Answer	ACA	271	Diameter base
Credit-Control-Request	CCR	272	Diameter Credit-Control Application - RFC 8506 (Obsoletes RFC 4006)
Credit-Control-Answer	CCA	272	Diameter Credit-Control Application - RFC 8506 (Obsoletes RFC 4006)
Capabilities-Exchange-Request	CER	257	Diameter base
Capabilities-Exchange-Answer	CEA	257	Diameter base
Device-Watchdog-Request	DWR	280	Diameter base
Device-Watchdog-Answer	DWA	280	Diameter base
Disconnect-Peer-Request	DPR	282	Diameter base
Disconnect-Peer-Answer	DPA	282	Diameter base
Re-Auth-Request	RAR	258	Diameter base
Re-Auth-Answer	RAA	258	Diameter base
Session-Termination-Request	STR	275	Diameter base
Session-Termination-Answer	STA	275	Diameter base
User-Authorization-Request	UAR	283	Diameter SIP Application - RFC 4740
User-Authorization-Answer	UAA	283	Diameter SIP Application - RFC 4740
Server-Assignment-Request	SAR	284	Diameter SIP Application - RFC 4740
Server-Assignment-Answer	SAA	284	Diameter SIP Application - RFC 4740
Location-Info-Request	LIR	285	Diameter SIP Application - RFC 4740
Location-Info-Answer	LIA	285	Diameter SIP Application - RFC 4740
Multimedia-Auth-Request	MAR	286	Diameter SIP Application - RFC 4740
Multimedia-Auth-Answer	MAA	286	Diameter SIP Application - RFC 4740
Registration-Termination-Request	RTR	287	Diameter SIP Application - RFC 4740
Registration-Termination-Answer	RTA	287	Diameter SIP Application - RFC 4740
Push-Profile-Request	PPR	288	Diameter SIP Application - RFC 4740
Push-Profile-Answer	PPA	288	Diameter SIP Application - RFC 4740
User-Authorization-Request	UAR	300	Diameter base (3GPP) RFC 3589
User-Authorization-Answer	UAA	300	Diameter base (3GPP) RFC 3589
Server-Assignment-Request	SAR	301	Diameter base (3GPP) RFC 3589
Server-Assignment-Answer	SAA	301	Diameter base (3GPP) RFC 3589
Location-Info-Request	LIR	302	Diameter base (3GPP) RFC 3589
Location-Info-Answer	LIA	302	Diameter base (3GPP) RFC 3589
Multimedia-Auth-Request	MAR	303	Diameter base (3GPP) RFC 3589
Multimedia-Auth-Answer	MAA	303	Diameter base (3GPP) RFC 3589
Registration-Termination-Request	RTR	304	Diameter base (3GPP) RFC 3589
Registration-Termination-Answer	RTA	304	Diameter base (3GPP) RFC 3589
Push-Profile-Request	PPR	305	Diameter base (3GPP) RFC 3589
Push-Profile-Answer	PPA	305	Diameter base (3GPP) RFC 3589
User-Data-Request	UDR	306	Diameter base (3GPP) RFC 3589
User-Data-Answer	UDA	306	Diameter base (3GPP) RFC 3589
Profile-Update-Request	PUR	307	Diameter base (3GPP) RFC 3589
Profile-Update-Answer	PUA	307	Diameter base (3GPP) RFC 3589
Subscribe-Notifications-Request	SNR	308	Diameter base (3GPP) RFC 3589
Subscribe-Notifications-Answer	SNA	308	Diameter base (3GPP) RFC 3589
Push-Notification-Request	PNR	309	Diameter base (3GPP) RFC 3589
Push-Notification-Answer	PNA	309	Diameter base (3GPP) RFC 3589
Bootstrapping-Info-Request	BIR	310	Diameter base (3GPP) RFC 3589
Bootstrapping-Info-Answer	BIA	310	Diameter base (3GPP) RFC 3589
Message-Process-Request	MPR	311	Diameter base (3GPP) RFC 3589
Message-Process-Answer	MPA	311	Diameter base (3GPP) RFC 3589
Update-Location-Request	ULR	316	3GPP TS 29.272 [RFC 5516]
Update-Location-Answer	ULA	316	3GPP TS 29.272 [RFC 5516]
Cancel-Location-Request	CLR	317	3GPP TS 29.272 [RFC 5516]
Cancel-Location-Answer	CLA	317	3GPP TS 29.272 [RFC 5516]
Authentication-Information-Request	AIR	318	3GPP TS 29.272 [RFC 5516]
Authentication-Information-Answer	AIA	318	3GPP TS 29.272 [RFC 5516]
Insert-Subscriber-Data-Request	IDR	319	3GPP TS 29.272 [RFC 5516]
Insert-Subscriber-Data-Answer	IDA	319	3GPP TS 29.272 [RFC 5516]
Delete-Subscriber-Data-Request	DSR	320	3GPP TS 29.272 [RFC 5516]
Delete-Subscriber-Data-Answer	DSA	320	3GPP TS 29.272 [RFC 5516]
Purge-UE-Request	PER	321	3GPP TS 29.272 [RFC 5516]
Purge-UE-Answer	PEA	321	3GPP TS 29.272 [RFC 5516]
Notify-Request	NR	323	3GPP TS 29.272 [RFC 5516]
Notify-Answer	NA	323	3GPP TS 29.272 [RFC 5516]
Provide-Location-Request	PLR	8388620	3GPP-LCS-SLg (Application-ID 16777255)
Provide-Location-Answer	PLA	8388620	3GPP-LCS-SLg (Application-ID 16777255)
Routing-Info-Request	RIR	8388622	3GPP-LCS-SLh (Application-ID 16777291)
Routing-Info-Answer	RIA	8388622	3GPP-LCS-SLh (Application-ID 16777291)
AA-Mobile-Node-Request	AMR	260	Diameter Mobile IPv4 - RFC 4004
AA-Mobile-Node-Answer	AMA	260	Diameter Mobile IPv4 - RFC 4004
Home-Agent-MIP-Request	HAR	262	Diameter Mobile IPv4 - RFC 4004
Home-Agent-MIP-Answer	HAA	262	Diameter Mobile IPv4 - RFC 4004
Configuration-Information-Request	CIR	8388718	S6t per 3GPP TS 29.336
Configuration-Information-Answer	CIA	8388718	S6t per 3GPP TS 29.336
Reporting-Information-Request	RIR	8388719	S6t per 3GPP TS 29.336
Reporting-Information-Answer	RIA	8388719	S6t per 3GPP TS 29.336
NIDD-Information-Request	NIR	8388726	S6t per 3GPP TS 29.336
NIDD-Information-Answer	NIA	8388726	S6t per 3GPP TS 29.336
```