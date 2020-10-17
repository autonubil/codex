# Media Metrics

latency

packets_lost
packets_dup
jitter_min
jitter_max
jitter_mean
jitter_stddev
ttl_min
ttl_max
ttl_mean
ttl_stddev

rtcp.xr.xnq.vmaxdiff
rtcp.xr.xnq.vrange
rtcp.xr.xnq.vsum
rtcp.xr.xnq.cycles
rtcp.xr.xnq.jbevents
rtcp.xr.xnq.tdegnet
rtcp.xr.xnq.tdegjit
rtcp.xr.xnq.es
rtcp.xr.xnq.ses

packets_lost
packets_repaired

ecn.packets_ect0
ecn.packets_ect1
ecn.packets_ecn_ce
ecn.packets_non_ect
ecn.packets_lost
ecn.packets_dup

media.burst.duration_sum
media.burst.duration_sumsqrs
media.burst.duration_avg
media.burst.duration_var
media.burst.packets_discard
media.burst.packets_discard_rate
media.burst.packets_lost
media.burst.packet_loss_rate
media.burst.packets_expected
media.bursts
media.gap.packet_loss_rate
media.gap.packet_discard_rate

rtcp.xr.pdv.type.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

rtcp.xr.pdv.type.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

rtcp.xr.pdv.pos_pdv.thresh
rtcp.xr.pdv.pos_pdv.pct
rtcp.xr.pdv.neg_pdv.thresh
rtcp.xr.pdv.neg_pdv.pct
rtcp.xr.pdv.mean

rndtrip.latency
rndtrip.latency_avg
rndtrip.latency_min
rndtrip.latency_max
endpoint_delay

frames_discard
frames_dup
frames_lost_full
frames_lost_part
frames_per_packet
frame_size

jitter_buffer.delay_nom
jitter_buffer.delay_nom_high
jitter_buffer.delay_nom_low
jitter_buffer.delay_max

packets_discard_dup
packets_discard_early
packets_discard_late
bytes_discard_dup
bytes_discard_early
bytes_discard_late

rtcp.xr.rfisd.delay_init_sync

rtcp.xr.rfso.sync_offset

audio.duration_playout
audio.duration_conceal
audio.duration_conceal_buff_adj
audio.playout_interrupts
audio.playout_interrupt_duration_avg
audio.unimpair_secs
audio.conceal_secs
audio.severe_conceal_secs
audio.scs_thresh
audio.packets_unimpair
audio.packets_conceal
audio.packets_severe_conceal
audio.packets_silent
audio.packets_conceal_ratio

voice.packet_loss_rate
voice.packet_discard_rate
voice.burst.density
voice.gap.density
voice.burst.duration
voice.gap.duration
voice.rtt
voice.endpoint_delay
voice.latency (calculated from rtt and endpoint_delay)
voice.signal
voice.noise
voice.snr (calculated from signal and noise)
voice.residual_echo_return_loss
voice.gap_thresh
voice.r_factor
voice.r_factor_external
voice.r_factor_total (R total = RTP R factor + ext. R factor - 94)
voice.mos
voice.mos_lq
voice.mos_cq
voice.jitter_buffer.adjust_rate
voice.jitter_buffer.delay_nom
voice.jitter_buffer.delay_max
voice.jitter_buffer.delay_abs_max
voice.jitter_buffer.packets_discard

video.impaired_duration
video.conceal_duration
video.frame_freeze_duration_avg
video.frame_impair_proportion_avg
video.frame_conceal_proportion_avg
video.frame_conceal_ratio

video.decode.ts_sync_losses
video.decode.errors_sync_byte
video.decode.errors_continuity
video.decode.errors_transport
video.decode.errors_pcr
video.decode.errors_pcr_repetition
video.decode.errors_pcr_discontinuity
video.decode.errors_pcr_accuracy
video.decode.errors_pts
video.decode.errors_pat
video.decode.errors_pat2
video.decode.errors_pmt
video.decode.errors_pmt2
video.decode.errors_pid
video.decode.errors_crc
video.decode.errors_cat

interval
cumulative
sampled


```text
ITU-T G.107

R:  R Factor
Ro:  Signal-to-Noise Ratio
Is:  Simultaneous Impairment Factor
Id:  Delay Impairment Factor
SLR:  Send loudness rating (dB)
RLR:  Receive loudness rating (dB)
STMR:  Sidetone masking rating (dB)
LSTR:  Listener sidetone rating (dB)
Ds:  D-Value of telephone, send side
Dr:  D-Value of telephone, receive side
TELR:  Talker echo loudness rating (dB)
WEPL:  Weighted echo path loss (dB)
T:  Mean one-way delay of the echo path (ms)
Tr:  Round-trip delay in a 4-wire loop (ms)
Ta:  Absolute delay in echo-free connections (ms)
sT:  Delay sensitivity
mT:  Minimum perceivable delay (ms)
qdu:  Number of quantization distortion units
Ie:  Equipment impairment factor
Bpl:  Packet-loss robustness factor
Ppl:  Random packet-loss probability (%)
BurstR:  Burst ratio
Nc:  Circuit noise referred to 0 dBr-point (dBm0p)
Nfor:  Noise floor at the receive side (dBmp)
Ps:  Room noise at the send side (dB(A))
Pr:  Room noise at the receive side (dB(A))
A:  Advantage factor

GoB:  Good or Better
MOS:  Mean Opinion Score
MNRU:  Modulated Noise Reference Unit
OLR:  Overall Loudness Rating
OPINE:  Overall Performance Index model for Network Evaluation
PLC:  Packet Loss Concealment
PoW:  Poor or Worse
```
