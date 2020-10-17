# rtp

rtp.version.ver
rtp.flag.ext
rtp.csrcs
rtp.flag.marker
rtp.payload_type.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

rtp.payload_type.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

rtp.seq_num
rtp.timestamp
rtp.ssrc
rtp.csrc []

rtp.interval

rtp.payload.codec
rtp.payload.clockrate

rtp.bytes
rtp.packets
rtp.flows

rtp.packets_ooo
rtp.packets_ooo_total

text
RTP Fixed Header Fields

   The RTP header has the following format:

    0                   1                   2                   3
    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |V=2|P|X|  CC   |M|     PT      |       sequence number         |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |                           timestamp                           |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |           synchronization source (SSRC) identifier            |
   +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
   |            contributing source (CSRC) identifiers             |
   |                             ....                              |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

   0                   1                   2                   3
   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  |      defined by profile       |           length              |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  |                        header extension                       |
  |                             ....                              |
