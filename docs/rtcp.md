# `rtcp`

rtcp.version.ver
rtcp.records
rtcp.cntrl_packet_type.id
rtcp.cntrl_packet_type.name
rtcp.size
rtcp.ssrc


rtcp.sr.ntp.timestamp
rtcp.sr.timestamp
rtcp.sr.packets
rtcp.sr.bytes

rtcp.report []
rtcp.report.ssrc
rtcp.report.loss_rate
rtcp.report.packets_lost
rtcp.report.highest_seq_num
rtcp.report.jitter
rtcp.report.jitter_avg
rtcp.report.jitter_max
rtcp.report.jitter_min
rtcp.report.jitter_samples
rtcp.report.jitter_sum
rtcp.report.lsr
rtcp.report.dlsr

rtcp.sdes []
rtcp.sdes.ssrc_csrc
rtcp.sdes.items
rtcp.sdes.item_type.id
rtcp.sdes.item_type.name
rtcp.sdes.item_size
rtcp.sdes.endpoint.id
rtcp.sdes.endpoint.user.name
rtcp.sdes.endpoint.host.name
rtcp.sdes.user.fullname
rtcp.sdes.user.email
rtcp.sdes.subscriber.msisdn
rtcp.sdes.location
rtcp.sdes.app.name
rtcp.sdes.note
rtcp.sdes.priv.prefix_size
rtcp.sdes.priv.prefix
rtcp.sdes.priv.value
rtcp.sdes.h323_caddr
rtcp.sdes.apsi
rtcp.sdes.rgrp
rtcp.sdes.stream_id
rtcp.sdes.stream_id_repaired
rtcp.sdes.ccid
rtcp.sdes.mid

rtcp.xr.block_type.id
rtcp.xr.block_type.name
rtcp.xr.block_size
rtcp.xr.thinning

rtcp.xr.loss_rle.thinning
rtcp.xr.loss_rle.ssrc
rtcp.xr.loss_rle.seq.begin
rtcp.xr.loss_rle.seq.end

rtcp.xr.dup_rle.thinning
rtcp.xr.dup_rle.ssrc
rtcp.xr.dup_rle.seq.begin
rtcp.xr.dup_rle.seq.end

rtcp.xr.packet_rx_time.thinning
rtcp.xr.packet_rx_time.ssrc
rtcp.xr.packet_rx_time.seq.begin
rtcp.xr.packet_rx_time.seq.end

rtcp.xr.dlrr.ntp.timestamp

rtcp.xr.dlrr. []
rtcp.xr.dlrr.ssrc
rtcp.xr.dlrr.lrr
rtcp.xr.dlrr.delay

rtcp.xr.stat_summ.ssrc
rtcp.xr.stat_summ.seq.begin
rtcp.xr.stat_summ.seq.end
rtcp.xr.stat_summ.packets_lost
rtcp.xr.stat_summ.packets_dup
rtcp.xr.stat_summ.jitter_min
rtcp.xr.stat_summ.jitter_max
rtcp.xr.stat_summ.jitter_mean
rtcp.xr.stat_summ.jitter_stddev
rtcp.xr.stat_summ.ttl_min
rtcp.xr.stat_summ.ttl_max
rtcp.xr.stat_summ.ttl_mean
rtcp.xr.stat_summ.ttl_stddev

https://tools.ietf.org/html/rfc3611
rtcp.xr.voip.size
rtcp.xr.voip.ssrc
rtcp.xr.voip.loss_rate
rtcp.xr.voip.discard_rate
rtcp.xr.voip.burst.density
rtcp.xr.voip.burst.duration
rtcp.xr.voip.gap.density
rtcp.xr.voip.gap.duration
rtcp.xr.voip.network.latency (rtt)
rtcp.xr.voip.svc.latency (esd)
rtcp.xr.voip.rndtrip.latency (latency - calculated from rtt and esd)
rtcp.xr.voip.signal
rtcp.xr.voip.noise
rtcp.xr.voip.snr (calculated from signal and noise)
rtcp.xr.voip.rerl
rtcp.xr.voip.gmin
rtcp.xr.voip.r_factor
rtcp.xr.voip.r_factor_external
rtcp.xr.voip.r_total (calculated from r_factor and r_factor_external)
rtcp.xr.voip.mos
rtcp.xr.voip.mos_lq
rtcp.xr.voip.mos_cq
rtcp.xr.voip.rx.config
rtcp.xr.voip.rx.plc.id
rtcp.xr.voip.rx.plc.name
rtcp.xr.voip.rx.jba.id
rtcp.xr.voip.rx.jba.name
rtcp.xr.voip.rx.jb_rate
rtcp.xr.voip.jb_delay_nom
rtcp.xr.voip.jb_delay_max
rtcp.xr.voip.jb_delay_abs_max

rtcp.xr.xnq.seq.begin
rtcp.xr.xnq.seq.end
rtcp.xr.xnq.vmaxdiff
rtcp.xr.xnq.vrange
rtcp.xr.xnq.vsum
rtcp.xr.xnq.cycles
rtcp.xr.xnq.jbevents
rtcp.xr.xnq.tdegnet
rtcp.xr.xnq.tdegjit
rtcp.xr.xnq.es
rtcp.xr.xnq.ses

rtcp.xr.post_repair_loss.thinning
rtcp.xr.post_repair_loss.ssrc
rtcp.xr.post_repair_loss.seq.begin
rtcp.xr.post_repair_loss.seq.end
rtcp.xr.post_repair_loss.packets_lost
rtcp.xr.post_repair_loss.packets_repaired

rtcp.xr.mcast_acq.ma_method.id
rtcp.xr.mcast_acq.ma_method.name
rtcp.xr.mcast_acq.ssrc
rtcp.xr.mcast_acq.ma_status.id
rtcp.xr.mcast_acq.ma_status.name

rtcp.xr.idms.spst.id
rtcp.xr.idms.spst.name
rtcp.xr.idms.payload_type.id
rtcp.xr.idms.payload_type.name
rtcp.xr.idms.media_stream_corr_id
rtcp.xr.idms.ssrc
rtcp.xr.idms.packet_rx.ntp_timestamp
rtcp.xr.idms.packet_rx.rtp_timestamp
rtcp.xr.idms.packet_present.ntp_timestamp

rtcp.xr.ecn.ssrc
rtcp.xr.ecn.ect0
rtcp.xr.ecn.ect1
rtcp.xr.ecn.ecn_ce
rtcp.xr.ecn.non_ect
rtcp.xr.ecn.packets_lost
rtcp.xr.ecn.packets_dup

rtcp.xr.burst_gap.ssrc
rtcp.xr.burst_gap.gmin
rtcp.xr.burst_gap.burst.duration_sum
rtcp.xr.burst_gap.burst.duration_sumsqrs
rtcp.xr.burst_gap.burst.duration_avg
rtcp.xr.burst_gap.burst.duration_var
rtcp.xr.burst_gap.burst.packets_discard
rtcp.xr.burst_gap.burst.packets_discard_rate
rtcp.xr.burst_gap.burst.packets_lost
rtcp.xr.burst_gap.burst.packet_loss_rate
rtcp.xr.burst_gap.burst.packets_expected
rtcp.xr.burst_gap.bursts
rtcp.xr.burst_gap.gap.packet_loss_rate
rtcp.xr.burst_gap.gap.packet_discard_rate

rtcp.xr.meas_info.ssrc
rtcp.xr.meas_info.seq_num.first
rtcp.xr.meas_info.seq_num.first_ext
rtcp.xr.meas_info.seq_num.last_ext
rtcp.xr.meas_info.meas_duration.interval
rtcp.xr.meas_info.meas_duration.cumulative

rtcp.xr.pdv.type.id
rtcp.xr.pdv.type.name
rtcp.xr.pdv.ssrc
rtcp.xr.pdv.pos_pdv.thresh
rtcp.xr.pdv.pos_pdv.pct
rtcp.xr.pdv.neg_pdv.thresh
rtcp.xr.pdv.neg_pdv.pct
rtcp.xr.pdv.mean

rtcp.xr.delay.meas_type.id
rtcp.xr.delay.meas_type.name
rtcp.xr.delay.ssrc
rtcp.xr.delay.rtt_avg
rtcp.xr.delay.rtt_min
rtcp.xr.delay.rtt_max
rtcp.xr.delay.esd

rtcp.xr.frame_impairment.ssrc
rtcp.xr.frame_impairment.seq.begin
rtcp.xr.frame_impairment.seq.end
rtcp.xr.frame_impairment.frames_discard
rtcp.xr.frame_impairment.frames_dup
rtcp.xr.frame_impairment.frames_lost_full
rtcp.xr.frame_impairment.frames_lost_part

rtcp.xr.mpeg2_decode.ssrc
rtcp.xr.mpeg2_decode.seq.begin
rtcp.xr.mpeg2_decode.seq.end
rtcp.xr.mpeg2_decode.ts_sync_losses
rtcp.xr.mpeg2_decode.errors_sync_byte
rtcp.xr.mpeg2_decode.errors_continuity
rtcp.xr.mpeg2_decode.errors_transport
rtcp.xr.mpeg2_decode.errors_pcr
rtcp.xr.mpeg2_decode.errors_pcr_repetition
rtcp.xr.mpeg2_decode.errors_pcr_discontinuity
rtcp.xr.mpeg2_decode.errors_pcr_accuracy
rtcp.xr.mpeg2_decode.errors_pts
rtcp.xr.mpeg2_decode.errors_pat
rtcp.xr.mpeg2_decode.errors_pat2
rtcp.xr.mpeg2_decode.errors_pmt
rtcp.xr.mpeg2_decode.errors_pmt2
rtcp.xr.mpeg2_decode.errors_pid
rtcp.xr.mpeg2_decode.errors_crc
rtcp.xr.mpeg2_decode.errors_cat

rtcp.xr.djb.meas_type.id
rtcp.xr.djb.meas_type.name
rtcp.xr.djb.buffer_type.id
rtcp.xr.djb.buffer_type.name
rtcp.xr.djb.ssrc
rtcp.xr.djb.delay_nom
rtcp.xr.djb.delay_nom_high
rtcp.xr.djb.delay_nom_low
rtcp.xr.djb.delay_max

rtcp.xr.discard.meas_type.id
rtcp.xr.discard.meas_type.name
rtcp.xr.discard.discard_type.id
rtcp.xr.discard.discard_type.name
rtcp.xr.discard.timing.id
rtcp.xr.discard.timing.name
rtcp.xr.discard.ssrc
rtcp.xr.discard.discards
rtcp.xr.discard.bytes

rtcp.xr.drle.timing.id
rtcp.xr.drle.timing.name
rtcp.xr.drle.ssrc
rtcp.xr.drle.seq.begin
rtcp.xr.drle.seq.end

rtcp.xr.rfisd.ssrc
rtcp.xr.rfisd.delay_init_sync

rtcp.xr.rfso.meas_type.id
rtcp.xr.rfso.meas_type.name
rtcp.xr.rfso.ssrc
rtcp.xr.rfso.sync_offset

rtcp.xr.mos.meas_type.id
rtcp.xr.mos.meas_type.name
rtcp.xr.mos.ssrc
rtcp.xr.mos.type.id
rtcp.xr.mos.type.name
rtcp.xr.mos.caid.id
rtcp.xr.mos.caid.name
rtcp.xr.mos.payload_type.id
rtcp.xr.mos.payload_type.name
rtcp.xr.mos.mos
rtcp.xr.mos.channel

https://tools.ietf.org/html/rfc7294
rtcp.xr.audio_conceal.meas_type.id
rtcp.xr.audio_conceal.meas_type.name
rtcp.xr.audio_conceal.conceal_method.id
rtcp.xr.audio_conceal.conceal_method.name
rtcp.xr.audio_conceal.ssrc
rtcp.xr.audio_conceal.playout_duration
rtcp.xr.audio_conceal.conceal_duration
rtcp.xr.audio_conceal.conceal_duration_buff_adj
rtcp.xr.audio_conceal.playout_interrupts
rtcp.xr.audio_conceal.playout_interrupt_duration_avg
rtcp.xr.audio_conceal.unimpaired_secs
rtcp.xr.audio_conceal.concealed_secs
rtcp.xr.audio_conceal.severe_concealed_secs
rtcp.xr.audio_conceal.scs_thresh
rtcp.xr.audio_conceal.packets_unimpaired
rtcp.xr.audio_conceal.packets_concealed
rtcp.xr.audio_conceal.packets_severe_concealed
rtcp.xr.audio_conceal.packets_silent

rtcp.xr.video_conceal.meas_type.id
rtcp.xr.video_conceal.meas_type.name
rtcp.xr.video_conceal.conceal_method.id
rtcp.xr.video_conceal.conceal_method.name
rtcp.xr.video_conceal.ssrc
rtcp.xr.video_conceal.impaired_duration
rtcp.xr.video_conceal.conceal_duration
rtcp.xr.video_conceal.frame_freeze_duration_avg
rtcp.xr.video_conceal.mifp
rtcp.xr.video_conceal.mcfp
rtcp.xr.video_conceal.ffsc

rtcp.xr..

rtcp.xr..

rtcp.xr..

rtcp.xr..



























BYE: Goodbye RTCP Packet

       0                   1                   2                   3
       0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
      +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
      |V=2|P|    SC   |   PT=BYE=203  |             length            |
      +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
      |                           SSRC/CSRC                           |
      +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
      :                              ...                              :
      +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
(opt) |     length    |               reason for leaving            ...
      +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

APP: Application-Defined RTCP Packet

	  0                   1                   2                   3
	  0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	 |V=2|P| subtype |   PT=APP=204  |             length            |
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	 |                           SSRC/CSRC                           |
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	 |                          name (ASCII)                         |
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	 |                   application-dependent data                ...
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+




SR: Sender Report RTCP Packet

	   0                   1                   2                   3
	   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
header |V=2|P|    RC   |   PT=SR=200   |             length            |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                         SSRC of sender                        |
	  +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
sender |              NTP timestamp, most significant word             |
info   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |             NTP timestamp, least significant word             |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                         RTP timestamp                         |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                     sender's packet count                     |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                      sender's octet count                     |
	  +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
report |                 SSRC_1 (SSRC of first source)                 |
block  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 1    | fraction lost |       cumulative number of packets lost       |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |           extended highest sequence number received           |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                      interarrival jitter                      |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                         last SR (LSR)                         |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	  |                   delay since last SR (DLSR)                  |
	  +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
report |                 SSRC_2 (SSRC of second source)                |
block  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 2    :                               ...                             :
	  +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
	  |                  profile-specific extensions                  |
	  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+


RR: Receiver Report RTCP Packet

        0                   1                   2                   3
        0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
header |V=2|P|    RC   |   PT=RR=201   |             length            |
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
       |                     SSRC of packet sender                     |
       +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
report |                 SSRC_1 (SSRC of first source)                 |
block  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  1    | fraction lost |       cumulative number of packets lost       |
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
       |           extended highest sequence number received           |
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
       |                      interarrival jitter                      |
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
       |                         last SR (LSR)                         |
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
       |                   delay since last SR (DLSR)                  |
       +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
report |                 SSRC_2 (SSRC of second source)                |
block  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  2    :                               ...                             :
       +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
       |                  profile-specific extensions                  |
       +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+


SDES: Source Description RTCP Packet

	    0                   1                   2                   3
	    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
	   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
header |V=2|P|    SC   |  PT=SDES=202  |             length            |
	   +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
chunk  |                          SSRC/CSRC_1                          |
  1    +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	   |                           SDES items                          |
	   |                              ...                              |
	   +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+
chunk  |                          SSRC/CSRC_2                          |
  2    +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	   |                           SDES items                          |
	   |                              ...                              |
	   +=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+=+

CNAME: Canonical End-Point Identifier SDES Item

	  0                   1                   2                   3
	  0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	 |    CNAME=1    |     length    | user and domain name        ...
	 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

NAME: User Name SDES Item

	 0                   1                   2                   3
	 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
	+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
	|     NAME=2    |     length    | common name of source       ...
	+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

EMAIL: Electronic Mail Address SDES Item

    0                   1                   2                   3
    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |    EMAIL=3    |     length    | email address of source     ...
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

PHONE: Phone Number SDES Item

   0                   1                   2                   3
   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  |    PHONE=4    |     length    | phone number of source      ...
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

LOC: Geographic User Location SDES Item

  0                   1                   2                   3
  0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 |     LOC=5     |     length    | geographic location of site ...
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

TOOL: Application or Tool Name SDES Item

 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|     TOOL=6    |     length    |name/version of source appl. ...
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

NOTE: Notice/Status SDES Item

    0                   1                   2                   3
    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |     NOTE=7    |     length    | note about the source       ...
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

PRIV: Private Extensions SDES Item

   0                   1                   2                   3
   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  |     PRIV=8    |     length    | prefix length |prefix string...
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  ...             |                  value string               ...
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

APSI: Application-Specific Identifier SDES Item

  0                   1                   2                   3
  0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 |    APSI=10    |     length    |application-specific identifier
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 |   ....
 +-+-+-+-+-+-+-+-+

RTCP 'RtpStreamId' SDES Extension

 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|RtpStreamId=TBD|     length    | RtpStreamId                 ...
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

RTCP 'RepairedRtpStreamId' SDES Extension

 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|Repaired...=TBD|     length    | RepairRtpStreamId           ...
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

RTCP CaptureID SDES Item

    0                   1                   2                   3
    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |   CaptId=TBA  |     length    | CaptureID                     |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |   ....        |
   +-+-+-+-+-+-+-+-+

RTCP MID SDES Item

   0                   1                   2                   3
   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  |      MID=TBD  |     length    | identification-tag          ...
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
