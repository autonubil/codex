# `tcp`

tcp.seq_num
tcp.ack_num
tcp.header_size

tcp.flags.bits
tcp.flags.tags
tcp.flags.label
tcp.flags.ns
tcp.flags.cwr
tcp.flags.ece
tcp.flags.urg
tcp.flags.ack
tcp.flags.psh
tcp.flags.rst
tcp.flags.syn
tcp.flags.fin

tcp.flags_init
tcp.flags_init
tcp.flags_init

tcp.flags_union
tcp.flags_union
tcp.flags_union

tcp.window_size
tcp.window_size_min
tcp.window_size_max
tcp.window_size_avg
tcp.window_size_sum
tcp.window_size_effective

tcp.checksum
tcp.urgent_pointer

tcp.max_seg_size

tcp.options
tcp.option.window_scale
tcp.option.max_segment_size

tcp.syns
tcp.syn_total
tcp.fins
tcp.fin_total
tcp.rsts
tcp.rst_total
tcp.pshs
tcp.psh_total
tcp.acks
tcp.ack_total
tcp.urgs
tcp.urg_total
tcp.synacks
tcp.synack_total
tcp.bad_flags
tcp.bad_flags_total
tcp.bad_xmas
tcp.bad_synfin
tcp.bad_rst
tcp.bad_noack
tcp.bad_urg
tcp.bad_noflag
tcp.frags
tcp.frags_total

tcp.bytes_retrans
tcp.packets_retrans
tcp.packet_rate_retrans
tcp.packets_ooo

tcp.syn_size
tcp.syn_ttl

tcp.flows

tcp.handshake. (SYN to SYN/ACK to ACK)
tcp.handshake.latency
tcp.handshake.latency_sum
tcp.handshake.latency_avg
tcp.handshake.latency_min
tcp.handshake.latency_max
tcp.handshake.latency_stddev
tcp.handshake.latency_sumsqrs
tcp.handshake.latency_var
tcp.handshake.samples

tcp.handshake.snd. (SYN to SYN/ACK)
tcp.handshake.snd.latency
tcp.handshake.snd.latency_sum
tcp.handshake.snd.latency_avg
tcp.handshake.snd.latency_min
tcp.handshake.snd.latency_max
tcp.handshake.snd.latency_stddev
tcp.handshake.snd.latency_sumsqrs
tcp.handshake.snd.latency_var
tcp.handshake.snd.samples

tcp.handshake.cnd. (SYN/ACK to ACK)
tcp.handshake.cnd.latency
tcp.handshake.cnd.latency_sum
tcp.handshake.cnd.latency_avg
tcp.handshake.cnd.latency_min
tcp.handshake.cnd.latency_max
tcp.handshake.cnd.latency_stddev
tcp.handshake.cnd.latency_sumsqrs
tcp.handshake.cnd.latency_var
tcp.handshake.cnd.samples

tcp.req. (network client to server)
tcp.req.latency
tcp.req.latency_sum
tcp.req.latency_avg
tcp.req.latency_min
tcp.req.latency_max
tcp.req.latency_stddev
tcp.req.latency_sumsqrs
tcp.req.latency_var
tcp.req.samples

tcp.resp. (network server to client)
tcp.resp.latency
tcp.resp.latency_sum
tcp.resp.latency_avg
tcp.resp.latency_min
tcp.resp.latency_max
tcp.resp.latency_stddev
tcp.resp.latency_sumsqrs
tcp.resp.latency_var
tcp.resp.samples

tcp.svc. (service/application server-side)
tcp.svc.latency
tcp.svc.latency_sum
tcp.svc.latency_avg
tcp.svc.latency_min
tcp.svc.latency_max
tcp.svc.latency_stddev
tcp.svc.latency_sumsqrs
tcp.svc.latency_var
tcp.svc.samples

tcp.rndtrip. (round-trip client to server+app to client)
tcp.rndtrip.latency
tcp.rndtrip.latency_sum
tcp.rndtrip.latency_avg
tcp.rndtrip.latency_min
tcp.rndtrip.latency_max
tcp.rndtrip.latency_stddev
tcp.rndtrip.latency_sumsqrs
tcp.rndtrip.latency_var
tcp.rndtrip.samples

tcp.transact. (initial client req to final resp)
tcp.transact.latency
tcp.transact.latency_sum
tcp.transact.latency_avg
tcp.transact.latency_min
tcp.transact.latency_max
tcp.transact.latency_stddev
tcp.transact.latency_sumsqrs
tcp.transact.latency_var
tcp.transact.samples

CHECK THAT THESE ARE DELETED
----------
tcp.handshake_rtt
tcp.rtt
  tcp.srt
  tcp.crt
tcp.rtt_avg
tcp.resp_time
